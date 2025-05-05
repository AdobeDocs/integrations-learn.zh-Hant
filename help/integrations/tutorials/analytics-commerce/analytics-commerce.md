---
title: 將 [!DNL Analytics] 與 [!DNL Commerce] 教學課程整合
description: 瞭解如何整合 [!DNL Analytics] 與 [!DNL Commerce]。
solution: Analytics, Commerce
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="整合" type="positive"
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# 將[!DNL Analytics]與[!DNL Commerce]整合

## 初始入門

這些指示適用於Adobe[!DNL Commerce]雲端裝載的專案。 自行託管的情況可能會有所不同，但整體程式應該類似。

1. 在您的本機環境中檢視程式碼
1. 使用撰寫器並安裝模組
1. 請依照這裡的個別指示進行，完成後請返回，以完成其餘步驟
   [安裝及設定Experience [!DNL Platform] 聯結器](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html?lang=zh-Hant){target="_blank"}


1. 認可composer.json，如果位於雲端，則認可composer.lock檔案
1. 驗證模組是否位於中繼及/或生產環境中
您可以登入Adobe[!DNL Commerce]的管理員區段，並在「系統>服務」下尋找這些新區段來執行此操作
   ![體驗[!DNL Platform]聯結器延伸模組](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. 使用Adobe[!DNL Commerce]後台內的認證設定模組。
   * 首先[!DNL Commerce]服務聯結器設定，如下所示。

     ![[!DNL Commerce]服務聯結器安裝程式](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * 然後是Experience [!DNL Platform]聯結器設定，如下所示。

     ![體驗[!DNL Platform]聯結器](./assets/analytics-commerce/experience-platform-connector.png)

如需入門流程每個階段和步驟的詳細資訊，請依照[Experience [!DNL Platform] 聯結器總覽](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html?lang=zh-Hant){target="_blank"}的說明操作。 Experience [!DNL Platform]聯結器教學課程會深入涵蓋每個區段，並回答您可能遇到的任何問題。 使用本教學課程瞭解其他快速設定步驟。

## Experience Edge和Adobe[!DNL Analytics]的設定

1. 確認您的組織具有（且您擁有）Adobe[!DNL Analytics]的存取權。 您可以前往[Adobe Experience Cloud首頁](https://experience.adobe.com/)，然後按一下頂端導覽列中的應用程式切換器（九個點），確認此問題。

1. 在Adobe[!DNL Analytics]中建立新的報表套裝，或識別您將[!DNL Commerce]資料推送至的報表套裝識別碼。 如需詳細資訊，請觀看有關[建立新報表套裝](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=zh-Hant)的教學課程。 您需要在下列資料流步驟中使用此報表套裝ID。

1. 如果您有體驗[!DNL Platform]的存取權，請瀏覽至[Adobe體驗 [!DNL Platform] 介面](https://platform.adobe.com)。 如果您無法存取該介面，則可以在Adobe體驗[!DNL Platform] [資料收集介面](https://experience.adobe.com/#/data-collection)中執行下面列出的所有必要步驟。

1. 使用[!DNL Commerce]特定欄位群組建立或更新您的XDM結構描述。 如需如何建立結構描述的詳細資訊，請參閱[「建立結構描述」](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html?lang=zh-Hant)教學課程。
   * 您將需要從以下資料流步驟中的選項中選取此結構描述。 若要建立結構描述，請檢視&#x200B;**資料管理**&#x200B;下的左欄，並找到&#x200B;**結構描述**。 現在在介面的右上方，按一下&#x200B;**建立結構描述**。 選取XDM ExperienceEvent。
   * 建立新結構描述後，您將新增[!DNL Commerce]欄位群組。 在UI左側，尋找[欄位群組]，然後按一下[新增] **&#x200B;**
      * 在搜尋中，您可以輸入`ExperienceEvent Commerce`進行篩選
      * 核取方塊以選取&#x200B;**Adobe[!DNL Analytics] ExperienceEvent[!DNL Commerce]**
      * 然後按一下右上方的&#x200B;**新增欄位群組**&#x200B;以儲存並繼續

1. 選擇性（且僅當您在Experience [!DNL Platform]介面時） — 建立新資料集
   * 此步驟可讓您將[!DNL Commerce]資料帶入Experience [!DNL Platform] (與將資料帶入Adobe[!DNL Analytics]分開)。 如果您有權存取Experience [!DNL Platform]，並打算在支援Experience [!DNL Platform]的應用程式(例如Real-Time Customer Data [!DNL Platform]、Customer Journey [!DNL Analytics]或Journey Optimizer)中使用[!DNL Commerce]資料，請執行此步驟。
   * 您將需要從下列資料流步驟中的選項中選取此資料集。
   * 在左側導覽的左欄&#x200B;**資料管理**&#x200B;標題下，選取&#x200B;**資料集**。
   * 按一下右上角的&#x200B;**建立資料集**。 選擇&#x200B;**從結構描述建立資料集**&#x200B;選項。
   * 搜尋並使用您在上一步建立的綱要

1. 建立Datastream以傳送[!DNL Commerce]資料給Adobe[!DNL Analytics]
   * 在左側欄的&#x200B;**資料彙集**&#x200B;標題下，選取&#x200B;**資料串流**。
   * 按一下介面右上角的&#x200B;**新增資料流**。
   * 提供名稱和說明（選用）。
   * 尋找並選取您在上一步中建立/識別的結構描述。
   * 新增任何需要的進階選項。 如需進階選項的詳細資訊，請瀏覽[檔案](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html?lang=zh-Hant)。
   * 按一下[儲存]以繼續。**&#x200B;**
   * 按一下&#x200B;**新增服務**，然後在下拉式欄位中選擇&#x200B;**Adobe[!DNL Analytics]**。
   * 按一下&#x200B;**新增報表套裝**，然後輸入您在上一步中建立/識別的報表套裝ID。 如果您希望資料流入多個報表套裝，可以新增多個報表套裝。
   * 或者，如果您在上一步中建立資料集，請再按一下&#x200B;**新增服務**，從下拉式欄位中選擇&#x200B;**Adobe體驗[!DNL Platform]**。 在「事件資料集」欄位中，選取您先前建立的資料集。
   * 儲存資料串流。

1. 最後，若要檢視您的[!DNL Commerce]資料，您必須導覽至Adobe[!DNL Analytics]中的Analysis Workspace、建立專案、選擇報表套裝，以及新增自由表格和其他視覺效果以報告和分析您的[!DNL Commerce]資料。 下圖顯示您可以在Analysis Workspace中建立的表格範例。

   ![[!DNL Analytics]部分商務資料的熒幕擷圖](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   以下是有助於您在Analysis Workspace中運作的其他資源：

   * [Analysis Workspace 概觀](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html?lang=zh-Hant)
   * [從頭開始建立Workspace專案](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html?lang=zh-Hant)
   * [在Analysis Workspace中使用表格、視覺效果和面板](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html?lang=zh-Hant)
   * [視覺效果使用案例](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html?lang=zh-Hant)

   此外，Experience League上還提供免費課程。 檢視[這裡](https://experienceleague.adobe.com/zh-hant?lang=en&amp;Solution=Analytics#courses)可用的[!DNL Analytics]課程。
