---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# [!DNL Analytics]與Audience Manager整合

{{analytics-description}}

{{audience-manager-description}}

啟用這項整合，透過將Adobe[!DNL Analytics]資料伺服器端轉送至Audience Manager，可讓Audience Manager獲得其主要資料來源之一，即線上客戶行為資料。 然後，此資料可與其他資料（例如第一方CRM資料或第三方合作夥伴資料）結合，以建立豐富的客戶區段。 此外，Audience Manager區段隨後會傳回至網頁，以作為進一步訪客分析的回應。 以下說明這兩個極具價值的使用案例。

整合Adobe[!DNL Analytics]與Audience Manager的主要優點如下：

+ **增強型細分**：結合Adobe[!DNL Analytics]和Audience Manager資料，在行銷行銷活動中取得精確的個人化對象區段。
+ **整合式客戶設定檔**：整合資料來源以瞭解互動和行為，建立完整的客戶設定檔。
+ **已改善廣告效益**：使用Adobe[!DNL Analytics]與Audience Manager整合的資料導向目標定位最佳化廣告。
+ **資料導向決定**：透過詳細的深入分析、合併Adobe[!DNL Analytics]和Audience Manager資料來告知選擇。
+ **個人化體驗**：量身打造您的內容與選件，使用兩個平台在接觸點間豐富客戶互動。

整體而言，這項整合整合彙集了寶貴的資料和對象深入分析。 它可讓企業建立更具針對性和更相關的行銷活動，同時深入瞭解客戶的偏好和行為。

## 常見整合

<table>
    <thead>
        <tr>
            <th>Experience Cloud應用程式</th>
            <th>整合，使用</th>
            <th>使用時機</th>
            <th>常見使用實例</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics]正在傳送資料給Audience Manager</a>
            </td>
            <td>Adobe[!DNL Analytics]標籤延伸或AppMeasurement.js，並啟用伺服器端轉送</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>當您想要將Adobe[!DNL Analytics]資料傳送至Audience Manager，以建立可與其他Adobe Experience Cloud目的地、以人物為基礎的目的地或Audience Manager支援的其他以裝置和自訂目的地共用的區段時。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>將區段共用至廣告平台，這些廣告平台包含在[!DNL Analytics]中收集的行為屬性。</li>
                    <li>使用[!DNL Analytics]資料擴充區段，以建立高價值、跨管道的區段，以用於網站上的目標定位。</li>
                    <li>將[!DNL Analytics]資料中的圖層套用到以雜湊識別碼（例如電子郵件）作為輸入資料的區段，以便在社群媒體平台中使用。</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html?lang=zh-Hant" target="_blank" rel="noreferrer">Audience Manager將資料傳回[!DNL Analytics]</a>
            </td>
            <td>Adobe[!DNL Analytics]標籤延伸或AppMeasurement.js，並啟用伺服器端轉送</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>當您想要從Audience Manager將區段共用至[!DNL Analytics]，以告知對象探索、細分和最佳化。</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>在[!DNL Analytics]報表中使用包含協力廠商提供者人口統計資料的Audience Manager區段。</li>
                    <li>在[!DNL Analytics]報表中使用包含來自廣告伺服器的行銷活動資料的Audience Manager區段。</li>
                    <li>在[!DNL Analytics]個報表中使用包含已上線CRM資料的Audience Manager區段。</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
