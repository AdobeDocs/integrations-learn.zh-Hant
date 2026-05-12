---
title: 將 [!DNL Analytics] 與 [!DNL Target] 教學課程整合
description: 瞭解如何將Adobe [!DNL Analytics] 與Adobe [!DNL Target]整合。
solution: Analytics, Target
feature: Integrations
topic: Integrations
role: Leader, Admin, Developer
level: Beginner
index: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00.000Z
badgeIntegration: label="整合" type="positive"
exl-id: 4ab6c61f-f14e-408a-a700-53f7b3d0600a
TQID: https://experienceleague.adobe.com/FrQDFw8oAkdz4NUMi9c9fXfyxqHod4-c-oL-GTb2a4Y
product_v2:
  - id: e43347a8-f2c5-4aa4-8623-6f13875d7e3a
  - id: e55547f1-a1ff-40c6-8978-026e40ab7fa4
feature_v2:
  - id: adee20bd-51f4-461d-b9db-d215f8756eeb
  - id: b069d60e-95f3-44d6-95a8-ddc862a4bc38
  - id: b3f03848-ae12-48b2-8aab-cad18567eb32
  - id: c153fd90-23e1-4614-81d3-3cc7571227f7
  - id: c93393a4-e558-47e1-992e-c91ed4d480ce
  - id: eb9732ab-8232-4b21-bc4c-89de86dbe4d7
  - id: f7c7de77-382f-4f48-8b36-61a170f06d3d
  - id: fd307ce7-56f5-4ee3-af68-a7833ff6e85e
subfeature_v2:
  - id: b3a8b8a0-1cc2-48a8-ac82-ffd9c66ccab4
  - id: ce57bdb9-8bbb-4c80-b9ab-e52598027bb9
  - id: dcae653e-62c6-4cc8-84e6-ee110b848296
  - id: df62f171-ac37-440f-8f0f-f41a72ebdd34
  - id: e38cbddc-1633-4cd5-bed5-9f289f2a6029
  - id: e6c28e30-8689-4bf4-8fa8-561343d308a9
  - id: f1f1a2d4-0976-4881-b091-c2bb8de7ffac
  - id: fd0ff162-b6d3-4a11-8aeb-e165a01c0f0a
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
  - id: f8a45b24-4be7-4f1b-909b-60d06b483a20
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
level_v2:
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
  - id: d3cdead0-685a-4489-9250-4bb709942f66
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
  - id: fd2e3797-f2ea-4b36-a9af-52acf5e90513
source-git-commit: 2a324011b3d235db3d4642c2797c4fa107267e6a
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 9%

---

# 將[!DNL Analytics]與[!DNL Target]整合


## 整合價值與設定

以下影片說明使用此整合的價值，以及有關設定整合的詳細資訊。

>[!NOTE]
>
>這些影片示範[!DNL Target] at.js和[!DNL Analytics] appMeasurement.js的實作和驗證。 請參閱[檔案](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4timplementation.html?lang=zh-Hant)，瞭解這兩種工具中所需的程式庫版本。

### 正在設定A4T （[!DNL Target]的[!DNL Analytics]）

在這段影片中，您應該瞭解開發人員如何：

* 說明如何使用SDID繫結[!DNL Analytics]和[!DNL Target]要求
* 說明搭配Adobe [!DNL Target] (A4T)的Adobe [!DNL Analytics]實作需求

>[!VIDEO](https://video.tv.adobe.com/v/35146/?quality=12&learn=on)

### 使用[!DNL Analytics]作為[!DNL Target]的資料Source

在這段專為商務從業人員提供的影片中，您將瞭解：

* 什麼是A4T以及為什麼要使用它？
* A4T如何運作？
* 使用A4T的先決條件為何？

>[!VIDEO](https://video.tv.adobe.com/v/17384/?quality=12&learn=on)


## 常見使用實例

以下影片說明透過A4T整合的不同功能、活動型別和優點。

### Analysis Workspace中[!DNL Target] (A4T)面板的[!DNL Analytics]

[!DNL Target] (A4T)面板的「[!DNL Analytics]」可讓您在Analysis Workspace中輕鬆分析Adobe [!DNL Target]活動和體驗。

>[!VIDEO](https://video.tv.adobe.com/v/37247/?quality=12&learn=on)

### 使用A4T面板分析Auto-[!DNL Target]活動

在本影片中，您將會瞭解如何使用[!DNL Target]面板的[!DNL Analytics]，以視覺效果呈現自動 — [!DNL Target]測試的結果。

>[!VIDEO](https://video.tv.adobe.com/v/333270/?quality=12&learn=on)

我們也有兩個逐步教學課程，向您說明在Analysis Workspace中為「自動分配」和「自動鎖定目標」活動設定A4T報表的詳細資料：

## 在Analysis Workspace中為自動分配活動設定A4T報表 {#a4t-auto-allocate}

自動分配活動會從兩個或多個體驗中識別獲勝者，並自動重新分配更多流量給獲勝者，同時測試會繼續執行和學習。 自動分配的[!DNL Target] (A4T)整合[!DNL Analytics]可讓您在Adobe [!DNL Analytics]中檢視報表資料，甚至針對[!DNL Analytics]中定義的自訂事件或量度進行最佳化。

<a href="https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/set-up-a4t-reports-in-analysis-workspace-for-auto-allocate-activities.html?lang=zh-Hant" class="spectrum-Button spectrum-Button--primary spectrum-Button--sizeM" target="_blank">
  <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">為自動分配活動設定A4T報告</span>
</a>

## 在Analysis Workspace中為自動[!DNL Target]活動設定A4T報表 {#a4t-auto-target}

自動[!DNL Target]活動之[!DNL Target] (A4T)整合的[!DNL Analytics]使用Adobe [!DNL Target] ensemble機器學習(ML)演演算法，根據訪客的設定檔、行為和內容來選擇每位訪客的最佳體驗，同時使用Adobe [!DNL Analytics]目標量度。

雖然Adobe [!DNL Analytics] Analysis Workspace提供豐富的分析功能，但由於實驗活動（手動A/B測試和自動分配）與個人化活動（自動[!DNL Target]）之間的差異，需要對[!DNL Target]面板的預設[!DNL Analytics]進行一些修改，才能正確解譯Auto-[!DNL Target]活動。

<a href="https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/set-up-a4t-reports-in-analysis-workspace-for-auto-target-activities.html?lang=zh-Hant" class="spectrum-Button spectrum-Button--primary spectrum-Button--sizeM" target="_blank">
  <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">為自動[!DNL Target]活動設定A4T報告</span>
</a>
