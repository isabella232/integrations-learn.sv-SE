---
source-git-commit: 94b074c17e976e4f4acbb1ff41aacfc9bf74744c
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 0%

---


# Integrera Adobe [!DNL Analytics] med kunddata i realtid [!DNL Platform]

{{analytics-description}}

{{real-time-cdp-description}}

Integrerande Adobe [!DNL Analytics] med kunddata i realtid från Adobe [!DNL Platform] (Real-Time CDP) kan ge flera fördelar för företag som vill förbättra sina kundupplevelser och sin marknadsföring. Här är några av de största fördelarna:

+ **Förbättrad målgruppsanpassning och personalisering**: Exakt marknadsföring på enheter och kanaler, skräddarsydda meddelanden för optimerat engagemang.
+ **Förbättrad optimering av landningssidor**: Skräddarsydda upplevelser baserade på enhet och beteende, vilket ger nöjdare och mer konverterade användare.
+ **Smidig målgruppsaktivering**: Använd kundprofiler för effektiv målgruppsanpassning via önskade kanaler och leverera relevanta meddelanden.

Genom att kombinera Adobe [!DNL Analytics] och Real-Time CDP kan företag ta sina marknadsföringssatsningar till nästa nivå och leverera personaliserade upplevelser, öka kundengagemanget och optimera konverteringar över olika digitala kontaktytor.

<table>
    <thead>
        <tr>
            <th>Experience Cloud-program</th>
            <th>Integreras med</th>
            <th>När ska du använda</th>
            <th>Vanliga användningsfall</th>
        </tr>
    </thead>
    <tr>
        <td rowspan="2">[!DNL Analytics] med Real-Time CDP</td>
        <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-source-connector.md" target="_blank" rel="noreferrer">Upplevelse [!DNL Platform] källkoppling</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Rekommenderat tillvägagångssätt för kunder som redan har implementerat Adobe [!DNL Analytics]och vill ha det snabbaste sättet att importera dessa data till upplevelsen [!DNL Platform] som kan användas i kundprofilen i realtid.</li>
                <li>När datatillgängligheten för kundprofilen i realtid kan vara mellan 2 och 30 minuter från datainsamlingen och datasjöns tillgänglighet är upp till 90 minuter.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Direkt, användargränssnittsinitierat arbetsflöde.</li>
                <li>Mappar användargränssnittet som ska kopieras [!DNL Analytics] props och eVars till nya XDM-fält.</li>
                <li>Det snabbaste sättet att få ut värde från kundprofilen i realtid och kundresan [!DNL Analytics].</li>
            </ul>
        </td>
    </tr>
    <tr>
       <td><a href="../../integrations/tutorials/analytics-rtcdp/experience-platform-edge.md" target="_blank" rel="noreferrer">Upplevelse [!DNL Platform] Kant</a></td>
        <td>
            <ul style="margin-top: 0;">
                <li>Rekommenderat tillvägagångssätt för nya [!DNL Analytics] implementeringar eller när ni vill implementera en långsiktig strategi.</li>
                <li>Skickar data direkt från en enhet till upplevelsen [!DNL Platform] med AEP Web SDK, AEP Mobile SDK eller Edge Network Server API.</li>
                <li>Nya eller gamla kunder som behöver [!DNL Analytics] datatillgänglighet för kundprofilen i realtid för att stödja användning av samma och nästa sidas personalisering.</li>
            </ul>
        </td>
        <td>
            <ul style="margin-top: 0;">
                <li>Ger störst kontroll för data som samlats in för att stödja dina användningsfall.</li>
                <li>Data på klientsidan mappas enkelt till XDM-fält.</li>
                <li>Snabbaste datatillgänglighet för kundprofilen i realtid.</li>
            </ul>
        </td>
    </tr>            
</table>
