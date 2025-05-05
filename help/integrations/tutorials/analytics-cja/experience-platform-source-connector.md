---
title: 將 [!DNL Analytics] 和Customer Journey [!DNL Analytics] 與Experience [!DNL Platform] 來源聯結器教學課程整合
description: 瞭解如何使用Experience [!DNL Platform] 來源聯結器將Adobe [!DNL Analytics] 與客戶歷程 [!DNL Analytics] 整合。
solution: Customer Journey [!DNL Analytics], [!DNL Target]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="整合" type="positive"
exl-id: f0dbd59d-d5e5-40e6-b4a4-e4789e7dd7e3
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 2%

---

# 將Adobe[!DNL Analytics]和客戶歷程[!DNL Analytics]與體驗[!DNL Platform]來源聯結器整合

<ol>
    <li><a href="https://experienceleague.adobe.com/zh-hant?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">為要擷取的資料建立結構描述</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">建立要擷取的資料集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">在結構描述</a>上設定正確的身分識別與身分識別名稱空間，以確定擷取的資料可以拼接到統一的設定檔。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">啟用設定檔</a>的結構描述和資料集。</li>
    <li>使用<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">Adobe[!DNL Analytics]來源聯結器</a>將資料內嵌至體驗[!DNL Platform]</li>
    <li><i>（選擇性）</i>。 如果使用多個資料集，請將人員ID拼接在一起，以<a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">產生合併的資料集</a>。 如果使用單一[!DNL Analytics]資料集，或如果您打算在Customer Journey [!DNL Analytics]中使用的所有資料集都存在通用識別碼，請略過此步驟。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">在客戶歷程[!DNL Analytics]中建立連線</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">建立資料檢視</a>、<a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">設定元件設定</a>，以及<a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">在Customer Journey [!DNL Analytics]中格式化量度</a>。
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">在Customer Journey [!DNL Analytics]中建立專案。</a></li>
</ol>

>[!NOTE]
>
>Adobe[!DNL Analytics]來源聯結器的標準工作流程步驟會建立結構描述和資料集，用於從[!DNL Analytics] 「原樣」擷取資料。 因此，前兩個步驟由系統處理。 對應工作流程需要建立自訂屬性；因此，請完全遵循步驟順序。
