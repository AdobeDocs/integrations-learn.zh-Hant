---
title: 整合 [!DNL Analytics] 替換為 [!DNL Commerce] 教學課程
description: 瞭解如何整合 [!DNL Analytics] 替換為 [!DNL Commerce].
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
ht-degree: 1%

---

# 整合 [!DNL Analytics] 替換為 [!DNL Commerce]

## 初始入門

這些指示適用於Adobe [!DNL Commerce] 雲端託管的專案。 自行託管的情況可能會有所不同，但整體程式應該類似。

1. 在您的本機環境中檢視程式碼
1. 使用撰寫器並安裝模組
1. 請依照這裡的個別指示進行，完成後請返回，以完成其餘步驟
   [安裝及設定體驗 [!DNL Platform] 聯結器](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. 認可composer.json，如果位於雲端，則認可composer.lock檔案
1. 驗證模組是否位於中繼和/或生產環境您可以登入Adobe的「管理員」區段來執行此操作 [!DNL Commerce] 並在「系統>服務」下尋找這些新區段
   ![體驗 [!DNL Platform] 聯結器擴充功能](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. 從Adobe內使用您的憑證設定模組 [!DNL Commerce] 後台。
   * 首先 [!DNL Commerce] 服務聯結器設定，如下所示。
     ![[!DNL Commerce] 服務聯結器設定](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * 然後體驗 [!DNL Platform] 聯結器設定，如下所示。
     ![體驗 [!DNL Platform] 聯結器](./assets/analytics-commerce/experience-platform-connector.png)

如需入門流程每個階段和步驟的詳細資訊，請依照 [體驗 [!DNL Platform] 聯結器概述](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. 體驗 [!DNL Platform] 聯結器教學課程會深入涵蓋每個區段，並回答您可能會有的任何問題。 使用本教學課程瞭解其他快速設定步驟。

## Experience Edge和Adobe的設定 [!DNL Analytics]

1. 確認貴組織擁有（且您擁有）Adobe存取權 [!DNL Analytics]. 這可以透過前往 [Adobe Experience Cloud首頁](https://experience.adobe.com/) 並按一下頂端導覽列中的應用程式切換器（九點）。

1. 在Adobe中建立新的報表套裝 [!DNL Analytics]，或識別您將推送的報表套裝ID [!DNL Commerce] 資料匯入。 如需詳細資訊，請觀看上的教學課程 [建立新的報表套裝](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html?lang=zh-Hant). 您需要在下列資料流步驟中使用此報表套裝ID。

1. 導覽至 [Adobe體驗 [!DNL Platform] 介面](https://platform.adobe.com) 如果您有權存取Experience [!DNL Platform]. 如果您無法存取該介面，可以執行以下在Adobe體驗中列出的所有必要步驟 [!DNL Platform] [資料收集介面](https://experience.adobe.com/#/data-collection).

1. 透過建立或更新您的XDM結構描述 [!DNL Commerce]特定欄位群組。 如需如何建立結構描述的詳細資訊，請參閱 [&quot;建立方案&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html) 教學課程。
   * 您將需要從以下資料流步驟中的選項中選取此結構描述。 若要建立結構描述，請檢視下方左側欄中的 **資料管理** 並尋找 **方案**. 現在，在介面的右上方，按一下 **建立結構描述**. 選取XDM ExperienceEvent。
   * 建立新結構描述後，您將新增 [!DNL Commerce] 欄位群組。 在UI左側，找到「欄位」群組，然後按一下 **新增**
      * 在搜尋中，您可以輸入以下內容進行篩選 `ExperienceEvent Commerce`
      * 選取 **Adobe [!DNL Analytics] 體驗事件[!DNL Commerce]** 勾選方塊
      * 然後按一下 **新增欄位群組** 以儲存並繼續

1. 選擇性（且僅在您處於體驗時） [!DNL Platform] 介面) — 建立新資料集
   * 此步驟可讓您將 [!DNL Commerce] 將資料匯入體驗 [!DNL Platform] (與將資料帶入Adobe分開) [!DNL Analytics])。 如果您有權存取Experience，請執行此步驟 [!DNL Platform]，並計畫使用 [!DNL Commerce] 體驗中的資料 [!DNL Platform] — 支援的應用程式，例如即時客戶資料 [!DNL Platform]，客戶歷程 [!DNL Analytics]或Journey Optimizer。
   * 您將需要從下列資料流步驟中的選項中選取此資料集。
   * 在左欄下方 **資料管理** 標題在左側導覽中選取 **資料集**.
   * 按一下 **建立資料集** 右上角。 選擇 **從結構描述建立資料集** 選項。
   * 搜尋並使用您在上一步建立的綱要

1. 建立資料流以傳送 [!DNL Commerce] 要Adobe的資料 [!DNL Analytics]
   * 在 **資料彙集** 標題中，選取 **資料串流**.
   * 按一下 **新增資料串流** 在介面的右上角。
   * 提供名稱和說明（選用）。
   * 尋找並選取您在上一步中建立/識別的結構描述。
   * 新增任何需要的進階選項。 如需進階選項的詳細資訊，請造訪 [檔案](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html).
   * 按一下 **儲存** 以繼續。
   * 按一下 **新增服務** 並選擇 **Adobe[!DNL Analytics]** ，位於下拉式欄位中。
   * 按一下 **新增報表套裝** 並輸入您在上一步中建立/識別的報表套裝ID。 如果您希望資料流入多個報表套裝，可以新增多個報表套裝。
   * 或者，如果您在上一步中建立了資料集，請按一下 **新增服務** 再次選擇 **Adobe體驗[!DNL Platform]** 從下拉式欄位。 在「事件資料集」欄位中，選取您先前建立的資料集。
   * 儲存資料串流。

1. 最後，若要檢視您的 [!DNL Commerce] 資料，您必須在Adobe中導覽至Analysis Workspace [!DNL Analytics]，建立專案、選擇報表套裝，以及新增自由表格和其他視覺效果以報告及分析 [!DNL Commerce] 資料。 下圖顯示您可以在Analysis Workspace中建立的表格範例。

   ![[!DNL Analytics] 部分商務資料的熒幕擷圖](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   以下是有助於您在Analysis Workspace中運作的其他資源：

   * [Analysis Workspace 概觀](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [從頭開始建立Workspace專案](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [在 Analysis Workspace 中使用表格、視覺效果和面板](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [視覺效果使用案例](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   此外，Experience League上還提供免費課程。 另請參閱 [!DNL Analytics] 可用的課程 [此處](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses).
