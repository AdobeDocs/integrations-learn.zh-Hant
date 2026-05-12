---
title: 將Adobe [!DNL Analytics] 和Customer Journey [!DNL Analytics] 與Experience [!DNL Platform] Edge教學課程整合
description: 瞭解如何使用AEP Web SDK、AEP Mobile SDK或Edge Network伺服器API將Adobe [!DNL Analytics] 與客戶歷程 [!DNL Analytics] 整合。
solution: Customer Journey Analytics, Analytics
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
kt: null
thumbnail: 13728
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="整合" type="positive"
exl-id: e39dac5d-6ad5-47c8-94e8-070011233161
TQID: https://experienceleague.adobe.com/ClZddWXeWp51gWTBjRDQBZ2xNiO1bTRq-AoAdmucNEg
product_v2:
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
  - id: e98b7246-966c-4318-9e95-cad2f7a17dc7
feature_v2:
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
  - id: e75a4a9c-d354-4ca4-9b02-1afeca73fa5e
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
subfeature_v2:
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 413
ht-degree: 15%

---

# 將Adobe [!DNL Analytics]和客戶歷程[!DNL Analytics]與體驗[!DNL Platform] Edge教學課程整合

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">為要擷取的資料建立結構描述</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">建立要擷取的資料集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在結構描述</a>上設定正確的身分識別與身分識別名稱空間，以確定擷取的資料可以拼接到統一的設定檔。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">啟用設定檔</a>的結構描述和資料集。</li>
    <li>使用下列其中一種方法將資料內嵌至體驗[!DNL Platform]：</li>
        <ul>
            <li>體驗[!DNL Platform]網頁SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">教學課程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">檢查清單</a></li>
                </ul>
            <li>體驗[!DNL Platform] Mobile SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">教學課程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">檢查清單</a></li>
                </ul></li>
            <li>Edge Network伺服器API：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">教學課程</a></li>
                </ul>
       </ul>
    <li><i>（選擇性）</i>。 如果使用多個資料集，請將人員ID拼接在一起，以<a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">產生合併的資料集</a>。 如果使用單一[!DNL Analytics]資料集，或如果您打算在Customer Journey [!DNL Analytics]中使用的所有資料集都存在通用識別碼，請略過此步驟。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">在客戶歷程[!DNL Analytics]中建立連線</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">建立資料檢視</a>、<a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">設定元件設定</a>，以及<a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">在Customer Journey [!DNL Analytics]中格式化量度</a>。
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">在Customer Journey [!DNL Analytics]中建立專案。</a></li>
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics]來源聯結器的標準工作流程步驟會建立用來從[!DNL Analytics] 「原樣」擷取資料的結構描述和資料集。 因此，前兩個步驟由系統處理。 對應工作流程需要建立自訂屬性；因此，請完全遵循步驟順序。
