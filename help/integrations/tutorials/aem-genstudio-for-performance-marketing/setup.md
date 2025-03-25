---
title: 設定GenStudio for Performance Marketing和AEM Assets
description: 使用GenStudio for Performance Marketing和AEM Assets設定Adobe GenStudio以簡化內容建立並確保品牌一致性。
solution: Experience Manager, Experience Manager as a Cloud Service, GenStudio for Performance Marketing
version: Experience Manager as a Cloud Service
feature-set: Experience Manager Assets, GenStudio for Performance Marketing
topic: Content Supply Chain
role: User
level: Intermediate
doc-type: Article
duration: 416
last-substantial-update: 2024-11-19T00:00:00Z
index: true
hidefromtoc: false
jira: KT-16484
exl-id: b63cfe6e-a530-4ca4-9e8e-16c54478054f
source-git-commit: 20e988c078ee926bbcf79f581ad9a60d5c478a83
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 7%

---

# 設定GenStudio for Performance Marketing和AEM Assets

[&#39;返回AEM Assets和GenStudio for Performance Marketing概覽](./overview.md)

若要開始將Adobe GenStudio與AEM Assets as a Cloud Service和GenStudio for Performance Marketing搭配使用，請確定已布建、啟用和設定必要的產品。 具體來說，您需要存取以下專案：

* AEM Assets as a Cloud Service
* AEM Assets Content Hub
* GenStudio for Performance Marketing

整合這些產品不需要進行額外的設定，只是要確保可供使用、設定並可讓使用者存取。

## 設定指南

如果尚未設定及啟用這些Adobe產品，請參閱下列指南以瞭解詳細的設定步驟：

<!-- CARDS 

* https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view
   {title=Set up AEM Assets}
* https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up
   {title=Enable AEM Assets Content Hub}
* https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started
   {title=Set up GenStudio for Performance Marketing}
   {image=https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/media_1dd8829962c9e37e1251f3d2d92f5d72c8a58cdaf.png?width=2000&format=webply&optimize=medium}

-->
<!-- START CARDS HTML - DO NOT MODIFY BY HAND -->
<div class="columns">
    <div class="column is-half-tablet is-half-desktop is-one-third-widescreen" aria-label="Set up AEM Assets">
        <div class="card" style="height: 100%; display: flex; flex-direction: column; height: 100%;">
            <div class="card-image">
                <figure class="image x-is-16by9">
                    <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view" title="設定AEM Assets" target="_blank" rel="referrer">
                        <img class="is-bordered-r-small" src="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view./media_1e4b209baa6169af9b0aefff8a2f1f39816aa6b42.png?width=400&format=png&optimize=medium" alt="設定AEM Assets"
                             style="width: 100%; aspect-ratio: 16 / 9; object-fit: cover; overflow: hidden; display: block; margin: auto;">
                    </a>
                </figure>
            </div>
            <div class="card-content is-padded-small" style="display: flex; flex-direction: column; flex-grow: 1; justify-content: space-between;">
                <div class="top-card-content">
                    <p class="headline is-size-6 has-text-weight-bold">
                        <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view" target="_blank" rel="referrer" title="設定AEM Assets">設定AEM Assets</a>
                    </p>
                    <p class="is-size-6">透過這精選旨在提升產品知識的影片播放清單，瞭解如何在Assets檢視中導覽AEM Assets as a Cloud Service。</p>
                </div>
                <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/video-playlists/assets-view" target="_blank" rel="referrer" class="spectrum-Button spectrum-Button--outline spectrum-Button--primary spectrum-Button--sizeM" style="align-self: flex-start; margin-top: 1rem;">
                    <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">進一步瞭解</span>
                </a>
            </div>
        </div>
    </div>
    <div class="column is-half-tablet is-half-desktop is-one-third-widescreen" aria-label="Enable AEM Assets Content Hub">
        <div class="card" style="height: 100%; display: flex; flex-direction: column; height: 100%;">
            <div class="card-image">
                <figure class="image x-is-16by9">
                    <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up" title="啟用AEM Assets Content Hub" target="_blank" rel="referrer">
                        <img class="is-bordered-r-small" src="https://video.tv.adobe.com/v/3433513/?format=jpeg&nocache=1733417775065" alt="啟用AEM Assets Content Hub"
                             style="width: 100%; aspect-ratio: 16 / 9; object-fit: cover; overflow: hidden; display: block; margin: auto;">
                    </a>
                </figure>
            </div>
            <div class="card-content is-padded-small" style="display: flex; flex-direction: column; flex-grow: 1; justify-content: space-between;">
                <div class="top-card-content">
                    <p class="headline is-size-6 has-text-weight-bold">
                        <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up" target="_blank" rel="referrer" title="啟用AEM Assets Content Hub">啟用AEM Assets Content Hub</a>
                    </p>
                    <p class="is-size-6">瞭解如何在AEM as a Cloud Service上設定Adobe Experience Manager Assets Content Hub。</p>
                </div>
                <a href="https://experienceleague.adobe.com/en/docs/experience-manager-learn/assets/content-hub/set-up" target="_blank" rel="referrer" class="spectrum-Button spectrum-Button--outline spectrum-Button--primary spectrum-Button--sizeM" style="align-self: flex-start; margin-top: 1rem;">
                    <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">觀看</span>
                </a>
            </div>
        </div>
    </div>
    <div class="column is-half-tablet is-half-desktop is-one-third-widescreen" aria-label="Set up GenStudio for Performance Marketing">
        <div class="card" style="height: 100%; display: flex; flex-direction: column; height: 100%;">
            <div class="card-image">
                <figure class="image x-is-16by9">
                    <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started" title="設定GenStudio for Performance Marketing" target="_blank" rel="referrer">
                        <img class="is-bordered-r-small" src="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/media_1dd8829962c9e37e1251f3d2d92f5d72c8a58cdaf.png?width=400&format=webply&optimize=medium" alt="設定GenStudio for Performance Marketing"
                             style="width: 100%; aspect-ratio: 16 / 9; object-fit: cover; overflow: hidden; display: block; margin: auto;">
                    </a>
                </figure>
            </div>
            <div class="card-content is-padded-small" style="display: flex; flex-direction: column; flex-grow: 1; justify-content: space-between;">
                <div class="top-card-content">
                    <p class="headline is-size-6 has-text-weight-bold">
                        <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started" target="_blank" rel="referrer" title="設定GenStudio for Performance Marketing">設定GenStudio for Performance Marketing</a>
                    </p>
                    <p class="is-size-6">了解如何開始使用 GenStudio for Performance Marketing 來產生符合品牌形象的新行銷內容。</p>
                </div>
                <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/get-started" target="_blank" rel="referrer" class="spectrum-Button spectrum-Button--outline spectrum-Button--primary spectrum-Button--sizeM" style="align-self: flex-start; margin-top: 1rem;">
                    <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">進一步瞭解</span>
                </a>
            </div>
        </div>
    </div>
</div>
<!-- END CARDS HTML - DO NOT MODIFY BY HAND -->

<br/>
<br/>
