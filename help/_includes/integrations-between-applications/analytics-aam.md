---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 1%

---


# [!DNL Analytics] 和Audience Manager整合

{{analytics-description}}

{{audience-manager-description}}

透過轉送Adobe來啟用此整合 [!DNL Analytics] 資料伺服器端到Audience Manager，為Audience Manager提供其主要資料來源之一，即線上客戶行為資料。 然後，此資料可與其他資料（例如第一方CRM資料或第三方合作夥伴資料）結合，以建立豐富的客戶區段。 此外，Audience Manager區段隨後會傳回至網頁，以作為進一步訪客分析的回應。 以下說明這兩個極具價值的使用案例。

整合Adobe的主要優點 [!DNL Analytics] 和Audience Manager為：

+ **增強型分段**：合併Adobe [!DNL Analytics] 和Audience Manager資料，以在行銷活動中取得精確的個人化對象區段。
+ **整合式客戶設定檔**：整合資料來源以瞭解互動和行為，建立完整的客戶設定檔。
+ **廣告效益改善**：使用Adobe的資料導向鎖定目標最佳化廣告 [!DNL Analytics] 與Audience Manager整合。
+ **資料導向式決策**：透過詳細的深入分析、合併Adobe來告知選擇 [!DNL Analytics] 和Audience Manager資料。
+ **個人化的體驗**：量身打造您的內容與選件，使用兩個平台在接觸點之間讓客戶互動更豐富。

整體而言，這項整合整合彙集了寶貴的資料和對象深入分析。 它可讓企業建立更具針對性和更相關的行銷活動，同時深入瞭解客戶的偏好和行為。

## 常見整合

<table>
    <thead>
        <tr>
            <th>Experience Cloud應用程式</th>
            <th>整合，使用</th>
            <th>何時使用</th>
            <th>常見使用實例</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] 傳送資料至Audience Manager</a>
            </td>
            <td>Adobe [!DNL Analytics] 標籤擴充功能或已啟用伺服器端轉送的AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>當您要傳送Adobe時 [!DNL Analytics] 要Audience Manager的資料，用來建立可與其他Adobe Experience Cloud目的地、以人物為基礎的目的地或Audience Manager支援的其他以裝置和自訂目的地共用的區段。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>將區段共用至廣告平台，其中包含收集到的行為屬性 [!DNL Analytics].</li>
                    <li>豐富區段 [!DNL Analytics] 建立高價值、跨管道區段以用於網站上的目標定位的資料。</li>
                    <li>圖層 [!DNL Analytics] 將資料放入以雜湊識別碼（例如電子郵件）作為輸入資料的區段，以用於社群媒體平台。</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager將資料傳回 [!DNL Analytics]</a>
            </td>
            <td>Adobe [!DNL Analytics] 標籤擴充功能或已啟用伺服器端轉送的AppMeasurement.js</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>當您想要將Audience Manager的區段共用給 [!DNL Analytics] 以通知對象探索、細分和最佳化。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>在中使用包含來自協力廠商提供者之人口統計資料的Audience Manager區段 [!DNL Analytics] 報表。</li>
                    <li>在中使用包含來自廣告伺服器的行銷活動資料的Audience Manager區段 [!DNL Analytics] 報表。</li>
                    <li>使用包含已上線CRM資料的Audience Manager區段 [!DNL Analytics] 報表。</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
