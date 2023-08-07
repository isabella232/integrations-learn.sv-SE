---
title: Integrera [!DNL Analytics] och kunddata i realtid [!DNL Platform] med upplevelse [!DNL Platform] självstudiekurs om källkoppling
description: Lär dig integrera Adobe [!DNL Analytics] med kunddata i realtid [!DNL Platform] använda upplevelsen [!DNL Platform] källkoppling.
solution: Real-Time Customer Data [!DNL Platform], [!DNL Analytics]
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: 13728
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrering" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---


# Integrera Adobe [!DNL Analytics] och kunddata i realtid [!DNL Platform] med upplevelse [!DNL Platform] källkoppling

<ol>
    <li><a href="https://experienceleague.adobe.com/?lang=en#dashboard/learning" _target="_blank" rel="noopener noreferrer">Skapa scheman</a> för data som ska importeras.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/data-ingestion/create-datasets-and-ingest-data.html" _target="_blank" rel="noopener noreferrer">Skapa datauppsättningar</a> för data som ska importeras.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/identities/label-ingest-and-verify-identity-data.html?lang=en" _target="_blank" rel="noopener noreferrer">Konfigurera rätt identiteter och identitetsnamnutrymmen i schemat</a> för att vara säker på att de importerade data kan sammanfogas till en enhetlig profil.</li> 
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/profiles/bring-data-into-the-real-time-customer-profile.html" _target="_blank" rel="noopener noreferrer">Aktivera scheman och datauppsättningar för profilen</a>.</li>
    <li>Ingest [!DNL Analytics] data till Experience-plattformen med <a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/sources/ingest-data-from-adobe-analytics.html" _target="_blank" rel="noopener noreferrer">Adobe [!DNL Analytics] källkoppling</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/audiences/create-audiences.html" _target="_blank" rel="noopener noreferrer">Skapa segment i upplevelsen [!DNL Platform].</a> Systemet avgör automatiskt om segmentet utvärderas som batch (dataanslutning) eller direktuppspelning (Edge-nätverk).</li>
    <li><a href="https://experienceleague.adobe.com/docs/platform-learn/tutorials/destinations/create-destinations-and-activate-data.html" _target="_blank" rel="noopener noreferrer">Konfigurera mål för delning av profilattribut och målgruppsmedlemskap till önskade mål.</a></li>   
</ol>

>[!NOTE]
>
>Standardstegen för arbetsflödet för Adobe [!DNL Analytics] källkopplingen skapa det schema och den datauppsättning som används för att importera data från [!DNL Analytics] &quot;as-is&quot;. Därför hanteras de första två stegen av systemet. Mappningsarbetsflödet kräver att du skapar anpassade attribut. Följ därför stegen helt.
