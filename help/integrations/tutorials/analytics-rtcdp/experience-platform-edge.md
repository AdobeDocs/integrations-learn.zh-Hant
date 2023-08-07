---
title: 整合 [!DNL Analytics] 和即時客戶資料 [!DNL Platform] 使用體驗 [!DNL Platform] Edge教學課程
description: 瞭解如何整合Adobe [!DNL Analytics] 使用即時客戶資料 [!DNL Platform] 使用AEP Web SDK、AEP Mobile SDK或Edge Network Server API。
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
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 20%

---


# 整合Adobe [!DNL Analytics] 和即時客戶資料 [!DNL Platform] 使用體驗 [!DNL Platform] Edge教學課程

<ol>
    <li>為要擷取的資料<a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">建立結構描述</a>。</li>
    <li>為要擷取的資料<a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">建立資料集</a>。</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">在架構上設定正確的身分和身分名稱空間</a> 以確定擷取的資料可拼接到統一的設定檔。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">為設定檔啟用結構描述和資料集</a>.</li>
    <li>將資料內嵌至體驗 [!DNL Platform] 使用下列其中一種方法：</li>
        <ul>
           <li>體驗 [!DNL Platform] Web SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/implement-web-sdk/overview.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">教學課程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/web-sdk/overview.html" _target="_blank" rel="noopener noreferrer">檢查清單</a></li>
                </ul>
            <li>體驗 [!DNL Platform] 行動SDK：</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/data-collection/mobile-sdk/create-mobile-properties.html" _target="_blank" rel="noopener noreferrer">教學課程</a></li>
                    <li><a href="https://experienceleague.adobe.com/docs/analytics/implementation/aep-edge/mobile-sdk/overview.html" _target="_blank" rel="noopener noreferrer">檢查清單</a></li>
                </ul></li>
            <li>邊緣網路伺服器 API:</li>
                <ul>
                    <li><a href="https://experienceleague.adobe.com/docs/experience-platform/edge-network-server-api/interacting-other-adobe-solutions/interacting-adobe-analytics.html?lang=zh-Hant" _target="_blank" rel="noopener noreferrer">教學課程</a></li>
                </ul>
       </ul>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/segments/create-segments.html" _target="_blank" rel="noopener noreferrer">在體驗中建立區段 [!DNL Platform].</a> 系統會自動判斷該區段是評估為批次（資料聯結器）還是串流（邊緣網路）。</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">設定目的地，以將設定檔屬性和對象成員資格共用至所需目的地。</a></li>
</ol>

>[!NOTE]
>
>Adobe的標準工作流程步驟 [!DNL Analytics] 來源聯結器會建立用於內嵌資料的結構描述和資料集 [!DNL Analytics] 「原樣」。 因此，前兩個步驟由系統處理。 對應工作流程需要建立自訂屬性；因此，請完全遵循步驟順序。
