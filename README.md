# tåg_och-trafikanalys_stockholm

Namn: Tindra von Zweigbergk

1. Mål
    Mitt mål med detta projekt är att automatisera insamling, rensning samt visualisering över riktig data för pendeltågen i Stockholm. För att förenkla programmet valde jag de viktigaste pendeltågsstationerna Stockholm Central och Odenplan.

    (Från ett AI-perspektiv kan det här projektet lösa de vanligaste problemen med datainsamling)

2. Metod
    1. Hämta data från API som är tagen från Trafiklabb
    2. Analysera API-datan
    3. Använda objektorienterad programmering med en föräldrarklass     (Departure) och två barnklasser (TrainDeparture och CommuterTrainDeparture).
    4. Behandla datan och tiden genom att "datetime_fromisdformat()" används i "filter_pendeltag_departure()" för att beräkna tidsskillnaden mellan "scheduled" och "expected".
    5. Funktionen "save_to_csv()" sparar avgångsdatan till filen "trafikdata.csv"
    6. "matplotlib.pyplot" skapar i "plot_delays()" ett stapebdiagram över de 12 närmaste pendel avgångarna och deras försening (om de är sena) i minuter.
    7. Programmet är en konsolbaserad "while True" meny i "main()" där användaren får välja att se avgångarna från Stockholm Central eller Odenplan.

3. Resultat

    Programmet ger en tydlig sammanställning av de kommande pendeltågsavgångarna, sparar datan i "trafikdara.csv" och printar ut en matplotlib stapeldiagram som visar förseningar i min/linje.

    När programmet startar ser terminalen ut såhär:

    ========================================
    Pendeltågsanalys - Huvudmeny
    ========================================
    1. Hämta pendeltåg för Stockholm City
    2. Hämta pendeltåg för Stockholm Odenplan
    3. Avsluta
    Välj ett alternativ (1-3): 

    Väljer ex. 1

    Hämtar aktuell pendeltågsdata för Stockholm City...
    --------------------------------------------------
    Klockan 12:22 | Linje 41 mot Märsta -> I tid
    Klockan 12:23 | Linje 41 mot Södertälje centrum -> I tid
    Klockan 12:37 | Linje 41 mot Märsta -> I tid
    Klockan 12:38 | Linje 41 mot Södertälje centrum -> I tid
    Klockan 12:45 | Linje 40 mot Älvsjö -> I tid
    Klockan 12:45 | Linje 40 mot Uppsala C -> I tid
    Klockan 12:52 | Linje 41 mot Märsta -> I tid
    Klockan 12:53 | Linje 41 mot Södertälje centrum -> I tid
    Klockan 13:15 | Linje 40 mot Älvsjö -> I tid
    Klockan 13:15 | Linje 40 mot Uppsala C -> I tid
    --------------------------------------------------

    Data sparades till trafikdata.csv!

    (Stapeldiagram)
    
    Alla avgångar vid Stockholm City är i tid!
   

4. Analys
    Resultatet av programmet visar hur man kan ta rådata från ett API och omvandlaa det till strukturerade mätvärden och till ett användarvänligt program. 

5. Reflektion
    Jag hade från bröjan skrivit ett program för elprisanalys men bytte sedan till att analysera tågtrafiken i Stockholm.R

6. AI-Användning
    Under skapandet av projektet har jag använt mig av AI som ett stöd för att debugga och feltesta mitt program. Den har varit ett stöd under skapandet av projektet och har hjälpt mig att förstå mer hur API-anrop fungerar, då det var det momentet jag tyckte var extra svårt.
    
7. Yrkescertifikat relevanta till projektet
    För mig som framtida AI-utvecklare

. GitHub-Länk

    
