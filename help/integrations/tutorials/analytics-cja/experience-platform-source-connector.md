---
title: Integrera [!DNL Analytics] och kundresa [!DNL Analytics] med upplevelse [!DNL Platform] självstudiekurs om källkoppling
description: Lär dig integrera Adobe [!DNL Analytics] med kundresan [!DNL Analytics] använda upplevelsen [!DNL Platform] källkoppling.
solution: Customer Journey [!DNL Analytics], [!DNL Target]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13727
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrering" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---


# Integrera Adobe [!DNL Analytics] och kundresa [!DNL Analytics] med upplevelse [!DNL Platform] källkoppling

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Skapa scheman</a> för data som ska importeras.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Skapa datauppsättningar</a> för data som ska importeras.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurera rätt identiteter och identitetsnamnutrymmen i schemat</a> för att vara säker på att de importerade data kan sammanfogas till en enhetlig profil.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html" _target="_blank" rel="noopener noreferrer">Aktivera scheman och datauppsättningar för profilen</a>.</li>
    <li>Infoga data i upplevelsen [!DNL Platform] med <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] källkoppling</a></li>
    <li><i>(Valfritt)</i>. Om du använder flera datauppsättningar sammanfogar du person-ID:n till <a href="https://experienceleague.adobe.com/docs/analytics-platform/using/cja-connections/combined-dataset.html" _target="_blank" rel="noopener noreferrer">generera en kombinerad datamängd</a>. Om du använder en enda [!DNL Analytics] datauppsättning, eller om det finns en gemensam identifierare för alla datauppsättningar som du planerar att använda på kundresan [!DNL Analytics]hoppar du över det här steget.</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/connections/connecting-customer-journey-analytics-to-data-sources-in-platform.html" _target="_blank" rel="noopener noreferrer">Skapa en anslutning</a> på kundresan [!DNL Analytics].</li>
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/basic-configuration-for-data-views.html" _target="_blank" rel="noopener noreferrer">Skapa en datavy</a>, <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/configuring-component-settings-in-data-views.html" _target="_blank" rel="noopener noreferrer">konfigurera komponentinställningarna</a>och <a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/data-views/formatting-metrics-in-data-views.html" _target="_blank" rel="noopener noreferrer">formatmått</a> på kundresan [!DNL Analytics].
    <li><a href="https://experienceleague.adobe.com/docs/customer-journey-analytics-learn/tutorials/analysis-workspace/workspace-projects/build-a-new-project.html" _target="_blank" rel="noopener noreferrer">Skapa ett projekt på kundresan [!DNL Analytics].</a></li>
</ol>

>[!NOTE]
>
>Standardstegen för arbetsflödet för Adobe [!DNL Analytics] källkopplingen skapa det schema och den datauppsättning som används för att importera data från [!DNL Analytics] &quot;as-is&quot;. Därför hanteras de första två stegen av systemet. Mappningsarbetsflödet kräver att du skapar anpassade attribut. Följ därför stegen helt.
