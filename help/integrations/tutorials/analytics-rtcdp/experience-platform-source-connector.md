---
title: 將 [!DNL Analytics] 和即時客戶資料 [!DNL Platform] 與Experience [!DNL Platform] 來源聯結器教學課程整合
description: 瞭解如何使用Experience [!DNL Platform] 來源聯結器將Adobe [!DNL Analytics] 與即時客戶資料 [!DNL Platform] 整合。
solution: Real-Time Customer Data Platform, Analytics
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="整合" type="positive"
exl-id: 1e27555d-e609-4a04-91ca-9518898ad699
TQID: https://experienceleague.adobe.com/Uct30-UadP-2Ocwslbk-dMAV0Y2unZlA339hThnofpA
product_v2: id: e55547f1-a1ff-40c6-8978-026e40ab7fa4id: fdddec33-c9cb-4459-b8b6-2664395a6f10
feature_v2: id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
subfeature_v2: id: e6c28e30-8689-4bf4-8fa8-561343d308a9
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bdid: f8a45b24-4be7-4f1b-909b-60d06b483a20id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2: id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 248
ht-degree: 11%

---

# 將Adobe [!DNL Analytics]和即時客戶資料[!DNL Platform]與體驗[!DNL Platform]來源聯結器整合

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">為要擷取的資料建立結構描述</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">建立要擷取的資料集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在結構描述</a>上設定正確的身分識別與身分識別名稱空間，以確定擷取的資料可以拼接到統一的設定檔。</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">啟用設定檔</a>的結構描述和資料集。</li>
    <li>使用<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics]來源聯結器</a>將[!DNL Analytics]資料擷取到Experience Platform。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">在體驗[!DNL Platform]中建立區段。</a> 系統會自動判斷區段是評估為批次（資料聯結器）還是串流（Edge網路）。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">設定目的地，以將設定檔屬性和對象成員資格共用至所需目的地。</a></li>   
</ol>

>[!NOTE]
>
>Adobe [!DNL Analytics]來源聯結器的標準工作流程步驟會建立用來從[!DNL Analytics] 「原樣」擷取資料的結構描述和資料集。 因此，前兩個步驟由系統處理。 對應工作流程需要建立自訂屬性；因此，請完全遵循步驟順序。
