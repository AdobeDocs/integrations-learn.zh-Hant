---
title: 將 [!DNL Analytics] 和即時客戶資料 [!DNL Platform] 與Experience [!DNL Platform] Edge教學課程整合
description: 瞭解如何使用AEP Web SDK、AEP Mobile SDK或Adobe伺服器API，將Edge Network [!DNL Analytics] 與即時客戶資料 [!DNL Platform] 整合。
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Developer
level: Experienced
index: true
hidefromtoc: true
kt: 13732
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="整合" type="positive"
exl-id: 07c2c329-0810-4f66-a91a-e315695f3fb4
source-git-commit: d35dc06c56c117cffe70542b6713f275877e4879
workflow-type: tm+mt
source-wordcount: '202'
ht-degree: 2%

---

# 將Adobe[!DNL Analytics]和即時客戶資料[!DNL Platform]與體驗[!DNL Platform] Edge教學課程整合

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">為要擷取的資料建立結構描述</a>。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">建立要擷取的資料集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在結構描述</a>上設定正確的身分識別與身分識別名稱空間，以確定擷取的資料可以拼接到統一的設定檔。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">啟用設定檔</a>的結構描述和資料集。</li>
    <li>使用下列其中一種方法將資料內嵌至體驗[!DNL Platform]：</li>
        <ul>
           <li>體驗[!DNL Platform] Web SDK：</li>
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
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">在體驗[!DNL Platform]中建立區段。</a>系統會自動判斷區段是評估為批次（資料聯結器）還是串流(Edge網路)。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">設定目的地，以將設定檔屬性和對象成員資格共用至所需目的地。</a></li>
</ol>

>[!NOTE]
>
>Adobe[!DNL Analytics]來源聯結器的標準工作流程步驟會建立結構描述和資料集，用於從[!DNL Analytics] 「原樣」擷取資料。 因此，前兩個步驟由系統處理。 對應工作流程需要建立自訂屬性；因此，請完全遵循步驟順序。
