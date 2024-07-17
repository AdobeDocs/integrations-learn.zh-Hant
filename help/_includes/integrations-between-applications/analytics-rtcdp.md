---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---


# 將Adobe[!DNL Analytics]與即時客戶資料[!DNL Platform]整合

{{analytics-description}}

{{real-time-cdp-description}}

將Adobe[!DNL Analytics]與Adobe即時客戶資料[!DNL Platform] (Real-Time CDP)整合可讓想要改善客戶體驗與行銷工作的企業獲得幾項好處。 以下是一些主要優點：

+ **增強的受眾目標定位與個人化**：裝置和管道上的精確行銷，針對最佳化的參與量身打造訊息。
+ **已改善登陸頁面最佳化**：根據裝置和行為量身打造的體驗，可提升使用者滿意度和轉換率。
+ **順暢的受眾啟用**：利用客戶設定檔，透過偏好的管道進行有效目標定位，並傳送相關訊息。

結合Adobe[!DNL Analytics]和Real-Time CDP，企業可以將行銷工作提升到新的境界，提供個人化體驗、提升客戶參與度，並最佳化各種數位接觸點的轉換。

<table>
    <thead>
        <tr>
            <th>Experience Cloud應用程式</th>
            <th>整合，使用</th>
            <th>使用時機</th>
            <th>常見使用實例</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] 使用Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">體驗[!DNL Platform]來源聯結器</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>已實作Adobe[!DNL Analytics]且想要以最快方式將此資料擷取至體驗[!DNL Platform]，以便用於即時客戶設定檔的客戶，建議使用此方法。</li>
                <li>當即時客戶設定檔的資料可用性從資料收集時間開始2到30分鐘之間，並且資料湖的可用性最高可達90分鐘時。</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>直接明瞭的使用者介面啟動的工作流程。</li>
                <li>對應使用者介面以將[!DNL Analytics]個prop和eVar複製到新的XDM欄位。</li>
                <li>從Real-time Customer Profile和Customer Journey [!DNL Analytics]取得價值的最快方式。</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">體驗[!DNL Platform] Edge</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>建議新[!DNL Analytics]實作的方法，或您想要實作長期策略的方法。</li>
                <li>使用AEP Web SDK、AEP Mobile SDK或Edge Network伺服器API，將資料直接從裝置傳送至Experience [!DNL Platform]。</li>
                <li>新客戶或現有客戶需要[!DNL Analytics]即時客戶個人檔案的資料可用性，以支援相同和下一頁個人化使用案例。</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>針對收集用於支援使用案例的資料提供最嚴謹的控制。</li>
                <li>使用者端資料可輕鬆對應至XDM欄位。</li>
                <li>即時客戶個人檔案最快取得資料。</li>
            </ul>
        </td>
    </tr>            
</table>
