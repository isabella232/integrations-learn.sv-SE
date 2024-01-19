---
title: Integrera [!DNL Analytics] med [!DNL Commerce] självstudiekurs
description: Integrera [!DNL Analytics] med [!DNL Commerce].
solution: Analytics, Commerce
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
exl-id: ef50b6b3-1e2b-4fe9-98d5-555bc14ae8d6
source-git-commit: 46803595cf8e199e0c331ea8b82f7fe4a2afc801
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 0%

---

# Integrera [!DNL Analytics] med [!DNL Commerce]

## Inledande introduktion

Dessa instruktioner gäller Adobe [!DNL Commerce] Molnbaserade projekt. Självhanterade kan i viss utsträckning variera, men den övergripande processen bör vara likartad.

1. Ta en titt på koden i den lokala miljön
1. Använda dispositionsverktyget och installera modulen
1. Följ de enskilda instruktionerna här och returnera när du är klar för att slutföra de återstående stegen
   [Installera och konfigurera upplevelsen [!DNL Platform] koppling](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/fundamentals/install.html){target="_blank"}


1. Verkställ filen comser.json och if i molnet, Composer.lock
1. Kontrollera att modulen finns i staging- och/eller produktionsmiljöerna Du kan göra detta genom att logga in i administratörssektionen i Adobe [!DNL Commerce] och letar efter de nya avsnitten under System > Tjänster
   ![Upplevelse [!DNL Platform] anslutningstillägg](./assets/analytics-commerce/admin-view-experience-platform-commector-extension.png)

1. Konfigurera modulen med dina autentiseringsuppgifter inifrån Adobe [!DNL Commerce] back office.
   * Först den [!DNL Commerce] Konfigurationer av tjänstkopplingar, enligt nedan.
     ![[!DNL Commerce] Installation av Services Connector](./assets/analytics-commerce/commerce-services-connector-setup.png)
   * Sedan upplevelsen [!DNL Platform] anslutningsinställningar, enligt nedan.
     ![Upplevelse [!DNL Platform] koppling](./assets/analytics-commerce/experience-platform-connector.png)

Mer information om varje fas och steg i introduktionsprocessen finns i [Upplevelse [!DNL Platform] anslutningsöversikt](https://experienceleague.adobe.com/docs/commerce-merchant-services/experience-platform-connector/overview.html){target="_blank"}. Upplevelsen [!DNL Platform] självstudiekursen för kontakter täcker alla avsnitt i detalj och besvarar eventuella frågor du har. Använd den här självstudiekursen för resten av snabbinstallationsstegen.

## Konfiguration av Experience Edge och Adobe [!DNL Analytics]

1. Verifiera att din organisation har (och att du har) åtkomst till Adobe [!DNL Analytics]. Detta kan bekräftas genom att gå till [Adobe Experience Cloud hemsida](https://experience.adobe.com/) och klicka på programväljaren (nio punkter) i den övre navigeringen.

1. Skapa en ny rapportsvit i Adobe [!DNL Analytics]eller identifiera ID:t för rapportsviten som du kommer att trycka på [!DNL Commerce] till. Titta på en självstudiekurs om du vill ha mer information [skapa en ny rapportserie](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/intro-to-analytics/analytics-basics/understanding-and-creating-report-suites.html). Du behöver detta rapportpaket-ID i datastream-steget nedan.

1. Navigera till [Adobe Experience [!DNL Platform] gränssnitt](https://platform.adobe.com) om ni har tillgång till Experience [!DNL Platform]. Om du inte har tillgång till det gränssnittet kan du utföra alla nödvändiga steg som listas nedan i Adobe Experience [!DNL Platform] [Gränssnitt för datainsamling](https://experience.adobe.com/#/data-collection).

1. Skapa eller uppdatera ditt XDM-schema med [!DNL Commerce]-specifika fältgrupper. Mer information om hur du skapar ett schema finns i [&quot;Skapa scheman&quot;](https://experienceleague.adobe.com/docs/platform-learn/tutorials/schemas/create-schemas.html) självstudie.
   * Du måste välja det här schemat bland alternativen i datastream-steget nedan. Om du vill skapa ett schema ska du titta i den vänstra kolumnen under **Datahantering** och hitta **Scheman**. Klicka på uppe till höger i gränssnittet **Skapa schema**. Välj XDM ExperienceEvent.
   * När du har skapat ett nytt schema lägger du till [!DNL Commerce] fältgrupper. Leta upp fältgrupper till vänster i användargränssnittet och klicka på **Lägg till**
      * I sökningen kan du filtrera genom att ange `ExperienceEvent Commerce`
      * Välj **Adobe [!DNL Analytics] ExperienceEvent[!DNL Commerce]** genom att markera rutan
      * Klicka sedan på **Lägg till fältgrupper** överst till höger för att spara och fortsätta

1. Alternativt (och bara om du är med i upplevelsen) [!DNL Platform] gränssnitt) - Skapa en ny datauppsättning
   * I det här steget kan du ta fram [!DNL Commerce] data till upplevelsen [!DNL Platform] (separat från uppgifterna i Adobe) [!DNL Analytics]). Gör det här steget om du har tillgång till Experience [!DNL Platform]och planerar att använda [!DNL Commerce] data i upplevelsen [!DNL Platform]-stödda applikationer, som kunddata i realtid [!DNL Platform], kundresa [!DNL Analytics]eller Journey Optimizer.
   * Du måste välja den här datauppsättningen bland alternativen i datastream-steget nedan.
   * Under den vänstra kolumnen **Datahantering** i den vänstra navigeringen väljer **Datauppsättningar**.
   * Klicka **Skapa datauppsättning** längst upp till höger. Välj **Skapa datauppsättning från schema** alternativ.
   * Sök efter och använd schemat som du skapade i det senaste steget

1. Skapa dataströmmen för att skicka [!DNL Commerce] data till Adobe [!DNL Analytics]
   * Under **Datainsamling** rubrik i den vänstra kolumnen väljer **Datastreams**.
   * Klicka **Ny datastream** längst upp till höger i gränssnittet.
   * Ange namn och valfri beskrivning.
   * Sök efter och välj det schema som du skapade/identifierade i föregående steg.
   * Lägg till önskade avancerade alternativ. Mer information om de avancerade alternativen finns på [dokumentation](https://experienceleague.adobe.com/docs/experience-platform/datastreams/configure.html).
   * Klicka **Spara** för att fortsätta.
   * Klicka **Lägg till tjänst** och välja **Adobe[!DNL Analytics]** i listrutan.
   * Klicka **Lägg till rapportsvit** och ange rapportsvitens-ID som du skapade/identifierade i ett tidigare steg. Du kan lägga till mer än en rapportserie om du vill att data ska flöda in i flera rapportsviter.
   * Om du vill kan du klicka på **Lägg till tjänst** igen, välja **Adobe Experience[!DNL Platform]** i listrutan. I fältet Händelsedatauppsättning väljer du den datauppsättning som du skapade tidigare.
   * Spara dataströmmen.

1. Äntligen kan du se [!DNL Commerce] måste du navigera till Analysis Workspace i Adobe [!DNL Analytics], skapa ett projekt, välja rapportsviten och lägg till frihandstabeller och andra visualiseringar för att rapportera om och analysera dina [!DNL Commerce] data. I följande bild visas ett exempel på en tabell som du kan skapa i Analysis Workspace.

   ![[!DNL Analytics] Skärmbild av vissa e-handelsdata](./assets/analytics-commerce/analytics-screenshot-commerce-items.png)

   Här finns ytterligare resurser som du kan använda för att arbeta i Analysis Workspace:

   * [Analysis Workspace - översikt](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/analysis-workspace-overview.html)
   * [Bygga ett arbetsyteprojekt från grunden](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/analysis-workspace-basics/building-a-workspace-project-from-scratch.html)
   * [Använda tabeller, visualiseringar och paneler i Analysis Workspace](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/using-panels/using-tables-visualizations-and-panels.html)
   * [Användningsexempel för visualisering](https://experienceleague.adobe.com/docs/analytics-learn/tutorials/analysis-workspace/visualizations/visualization-use-cases.html)

   Dessutom finns det kostnadsfria kurser i Experience League. Se [!DNL Analytics] tillgängliga kurser [HÄR](https://experienceleague.adobe.com/?lang=en&amp;Solution=Analytics#courses).
