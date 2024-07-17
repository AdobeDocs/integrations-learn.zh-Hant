---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 1%

---


# 將Adobe[!DNL Analytics]與客戶歷程[!DNL Analytics]整合

{{analytics-description}}

{{customer-journey-analytics-description}}

將Adobe[!DNL Analytics]與客戶歷程[!DNL Analytics]整合可提供主要優點：

+ **對客戶行為和偏好的全面深入分析**。
+ **順暢的跨管道追蹤**，提供整體檢視。
+ **統一資料與報告**，以進行精確分析。
+ **加強個人化**&#x200B;並改善客戶參與度。
+ **即時資料深入分析**，用於敏捷決策。

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
            <td rowspan="2">[!DNL Analytics] 和客戶歷程 [!DNL Analytics]</td>
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-source-connector.md" target="_blank" rel="noreferrer">體驗[!DNL Platform]來源聯結器</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>已實作Adobe[!DNL Analytics]且想要以最快方式將此資料擷取至體驗[!DNL Platform]，以便用於客戶歷程[!DNL Analytics]的客戶，建議使用此方法。</li>
                    <li>客戶設定檔的資料可用性從資料收集時間起可能為2至30分鐘，而資料湖的可用性最高可達90分鐘。</li>
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
            <td><a href="../../integrations/tutorials/analytics-cja/experience-platform-edge.md" target="_blank" rel="noreferrer">體驗[!DNL Platform] Edge</a></td>
            <td>
                <ul style="margin-top: 0;">
                    <li>建議新[!DNL Analytics]實作的方法，或您想要實作長期策略的方法。</li>
                    <li>使用AEP Web SDK、AEP Mobile SDK或Edge Network伺服器API，將資料直接從裝置傳送至Experience [!DNL Platform]。</li>
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
    </tbody>          
</table>
