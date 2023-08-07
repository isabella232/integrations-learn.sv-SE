---
title: Integrera [!DNL Analytics] med [!DNL Target] självstudiekurs
description: Lär dig integrera Adobe [!DNL Analytics] med Adobe [!DNL Target].
solution: Analytics, Target
feature: Integrations
topic: Integrations
role: Leader, Architect, Admin, Developer
level: Beginner
index: true
hidefromtoc: true
kt: null
thumbnail: null
last-substantial-update: 2023-04-11T00:00:00Z
badgeIntegration: label="Integrering" type="positive"
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---


# Integrera [!DNL Analytics] med [!DNL Target]


## Integrationsvärde och konfiguration

I videofilmerna nedan visas värdet av att använda den här integreringen samt information om hur du får integreringsinställningarna.

>[!NOTE]
>
>I dessa videofilmer visas implementering och validering av [!DNL Target] at.js och [!DNL Analytics] appMeasurement.js. Läs mer i [dokumentation](https://experienceleague.adobe.com/docs/target/using/integrate/a4t/a4timplementation.html) för nödvändiga biblioteksversioner i båda verktygen.

### Konfigurera A4T ([!DNL Analytics] for [!DNL Target])

I den här videon, som är avsedd för en utvecklare, får du lära dig att:

* Förklara [!DNL Analytics] och [!DNL Target] begäranden som binds upp med SDID
* Beskriv implementeringskraven för Adobe [!DNL Analytics] med Adobe [!DNL Target] (A4T)

>[!VIDEO](https://video.tv.adobe.com/v/35146/?quality=12&learn=on)

### Använd [!DNL Analytics] som datakälla för [!DNL Target]

I den här videon, som är avsedd för yrkesverksamma, får du lära dig:

* Vad är A4T och varför skulle jag använda det?
* Hur fungerar A4T?
* Vilka är förutsättningarna för att använda A4T?

>[!VIDEO](https://video.tv.adobe.com/v/17384/?quality=12&learn=on)


## Vanliga användningsfall

I videofilmerna nedan visas olika funktioner, aktivitetstyper och fördelar med att integrera via A4T.

### [!DNL Analytics] for [!DNL Target] (A4T) Panel i Analysis Workspace

The [!DNL Analytics] for [!DNL Target] (A4T) kan du analysera Adobe [!DNL Target] aktiviteter och upplevelser, med lyft och förtroende, i Analysis Workspace.

>[!VIDEO](https://video.tv.adobe.com/v/37247/?quality=12&learn=on)

### Analysera en automatisk[!DNL Target] Aktivitet med A4T-panelen

I den här videon får du lära dig hur du använder [!DNL Analytics] for [!DNL Target] för att visualisera resultatet av en[!DNL Target] test.

>[!VIDEO](https://video.tv.adobe.com/v/333270/?quality=12&learn=on)

Vi har också två stegvisa självstudiekurser som visar hur du konfigurerar A4T-rapporter i Analysis Workspace för aktiviteter som &quot;autoallokering&quot; och &quot;automål&quot;:

## Konfigurera A4T-rapporter i Analysis Workspace för automatisk allokering av aktiviteter {#a4t-auto-allocate}

En autoallokeringsaktivitet identifierar en vinnare av två eller flera upplevelser och omfördelar automatiskt mer trafik till vinnaren medan testet fortsätter att köras och lära sig. The [!DNL Analytics] for [!DNL Target] (A4T)-integrering för automatisk allokering gör att du kan se dina rapportdata i Adobe [!DNL Analytics]och du kan även optimera för anpassade händelser eller mätvärden som definieras i [!DNL Analytics].

<a href="https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/set-up-a4t-reports-in-analysis-workspace-for-auto-allocate-activities.html" class="spectrum-Button spectrum-Button--primary spectrum-Button--sizeM" target="_blank">
  <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">Ställ in A4T-rapporter för automatisk allokering av aktiviteter</span>
</a>

## Konfigurera A4T-rapporter i Analysis Workspace för Auto-[!DNL Target] verksamhet {#a4t-auto-target}

The [!DNL Analytics] for [!DNL Target] (A4T)-integrering för Auto-[!DNL Target] aktiviteter använder Adobe [!DNL Target] algoritmer för maskininlärning (ML) för att välja den bästa upplevelsen för varje besökare utifrån deras profil, beteende och sammanhang, allt med hjälp av Adobe [!DNL Analytics] målmått.

Även om det finns omfattande analysfunktioner i Adobe [!DNL Analytics] Analysis Workspace, några ändringar i standardinställningarna [!DNL Analytics] for [!DNL Target] -panelen krävs för att tolka automatisk[!DNL Target] aktiviteter, på grund av skillnader mellan experimentella aktiviteter (manuellt A/B-test och automatisk fördelning) och personaliseringsaktiviteter (automatisk-[!DNL Target]).

<a href="https://experienceleague.adobe.com/docs/target-learn/tutorials/integrations/set-up-a4t-reports-in-analysis-workspace-for-auto-target-activities.html" class="spectrum-Button spectrum-Button--primary spectrum-Button--sizeM" target="_blank">
  <span class="spectrum-Button-label has-no-wrap has-text-weight-bold">Ställ in A4T-rapporter för Auto-[!DNL Target] verksamhet</span>
</a>