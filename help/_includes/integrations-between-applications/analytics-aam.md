---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---


# [!DNL Analytics] och integrering med Audience Manager

{{analytics-description}}

{{audience-manager-description}}

Aktivera integreringen genom att vidarebefordra Adobe [!DNL Analytics] data server-side till Audience Manager, ger Audience Manager en av sina viktigaste datakällor, nämligen kundbeteendedata online. Dessa data kan sedan kombineras med andra data, som CRM-data från första part eller partnerdata från tredje part, för att skapa avancerade kundsegment. Dessutom skickas segment i Audience Manager tillbaka till webbsidan som svar på ytterligare besökaranalys. Båda dessa värdefulla användningsområden beskrivs nedan.

De viktigaste fördelarna med att integrera Adobe [!DNL Analytics] och Audience Manager är:

+ **Förbättrad segmentering**: Kombinera Adobe [!DNL Analytics] &amp; Audience Manager för exakta, personaliserade målgruppssegment i marknadsföringskampanjer.
+ **Enhetliga kundprofiler**: Integrera datakällor för att förstå interaktioner och beteenden och skapa omfattande kundprofiler.
+ **Förbättrad annonseffektivitet**: Optimera annonser med datadriven målinriktning från Adobe [!DNL Analytics] och integrering med Audience Manager.
+ **Datadrivna beslut**: Infordra valmöjligheterna genom detaljerade insikter, slå samman Adobe [!DNL Analytics] &amp; Audience Manager data.
+ **Personaliserade upplevelser**: Skräddarsy innehåll och erbjudanden och berika kundinteraktioner över olika kontaktytor med båda plattformarna.

Den här integreringen sammanför värdefulla data och målgruppsinsikter. Det gör att företag kan skapa mer målinriktade och relevanta marknadsföringskampanjer och samtidigt få en djupare förståelse för kundernas preferenser och beteenden.

## Vanliga integreringar

<table>
    <thead>
        <tr>
            <th>Experience Cloud-program</th>
            <th>Integreras med</th>
            <th>När ska du använda</th>
            <th>Vanliga användningsfall</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>
                <a href="/docs/analytics-learn/tutorials/integrations/audience-manager/enable-server-side-forwarding-in-adobe-launch.html" target="_blank" rel="noreferrer">[!DNL Analytics] skicka data till Audience Manager</a>
            </td>
            <td>Adobe [!DNL Analytics] taggtillägg eller AppMeasurement.js med vidarebefordran på serversidan aktiverad</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>När du vill skicka Adobe [!DNL Analytics] data till Audience Manager för att skapa segment som kan delas med andra Adobe Experience Cloud-destinationer, personbaserade destinationer eller andra enhetsbaserade och anpassade destinationer som stöds av Audience Manager.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Dela segment till annonsplattformar som innehåller beteendeattribut som samlats in i [!DNL Analytics].</li>
                    <li>Förbättra segment med [!DNL Analytics] data för att skapa värdefulla flerkanalssegment som kan användas för målinriktning på plats.</li>
                    <li>Lager in [!DNL Analytics] data till segment som är genomskinliga av hash-kodade identifierare, t.ex. e-post, och som ska användas på plattformar för sociala medier.</li>
                </ul>
            </td>
        </tr>        
        <tr>
            <td>
                <a href="https://experienceleague.adobe.com/docs/analytics/integration/audience-analytics/mc-audiences-aam.html" target="_blank" rel="noreferrer">Audience Manager skickar tillbaka data till [!DNL Analytics]</a>
            </td>
            <td>Adobe [!DNL Analytics] taggtillägg eller AppMeasurement.js med vidarebefordran på serversidan aktiverad</td>
            <td>
                <ul style="margin-top: 0;">
                    <li>När du vill dela segment från Audience Manager till [!DNL Analytics] för att informera om identifiering, segmentering och optimering av målgrupper.</li>
                </ul>
            </td>
            <td>
                <ul style="margin-top: 0;">
                    <li>Använd Audience Manager-segment som innehåller demografiska data från tredjepartsleverantörer i [!DNL Analytics] rapporter.</li>
                    <li>Använd segment i Audience Manager som innehåller kampanjdata från annonsservrar i [!DNL Analytics] rapporter.</li>
                    <li>Använd Audience Manager-segment som innehåller onboarddata i [!DNL Analytics] rapporter.</li>
                </ul>
            </td>
        </tr>
    </tbody>
</table>
