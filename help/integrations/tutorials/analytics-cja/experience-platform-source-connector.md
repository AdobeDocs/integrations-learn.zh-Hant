---
title: 整合 [!DNL Analytics] 和客戶歷程 [!DNL Analytics] 使用體驗 [!DNL Platform] 來源聯結器教學課程
description: 瞭解如何整合Adobe [!DNL Analytics] 使用客戶歷程 [!DNL Analytics] 使用體驗 [!DNL Platform] 來源聯結器。
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
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 18%

---


# 整合Adobe [!DNL Analytics] 和客戶歷程 [!DNL Analytics] 使用體驗 [!DNL Platform] 來源聯結器

<ol>
    <li>為要擷取的資料<a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">建立結構描述</a>。</li>
    <li>為要擷取的資料<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">建立資料集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架構上設定正確的身分和身分名稱空間</a> 以確定擷取的資料可拼接到統一的設定檔。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">為設定檔啟用結構描述和資料集</a>.</li>
    <li>將資料內嵌至體驗 [!DNL Platform] 使用 <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] 來源聯結器</a></li>
    <li><i>(可選)</i>. 如果使用多個資料集，請將人員ID拼接到 <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">產生合併的資料集</a>. 若使用單一 [!DNL Analytics] 資料集，或如果您打算在Customer Journey中使用的所有資料集都存在共同識別碼 [!DNL Analytics]，略過此步驟。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">建立連線</a> 在客戶歷程中 [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">建立資料檢視</a>， <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">設定元件設定</a>、和 <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">格式化量度</a> 在客戶歷程中 [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">在Customer Journey建立專案 [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Adobe的標準工作流程步驟 [!DNL Analytics] 來源聯結器會建立用於內嵌資料的結構描述和資料集 [!DNL Analytics] 「原樣」。 因此，前兩個步驟由系統處理。 對應工作流程需要建立自訂屬性；因此，請完全遵循步驟順序。
