# tåg_och-trafikanalys_stockholm

Namn: Tindra von Zweigbergk

1. Mål
    Mitt mål med detta projekt är att automatisera insamling, rensning samt visualisering över riktig data för pendeltågen i Stockholm. För att förenkla programmet valde jag de viktigaste pendeltågsstationerna Stockholm Central och Odenplan.

2. Metod
    1. Hämta data från API som är tagen från Trafiklabb
    2. Analysera API-datan
    3. Använda objektorienterad programmering med en föräldrarklass (Departure) och två barnklasser (TrainDeparture och CommuterTrainDeparture).
    4. Behandla datan och tiden genom att "datetime.fromisodformat()" används i "filter_pendeltag_departures()" för att beräkna tidsskillnaden mellan "scheduled" och "expected".
    5. Funktionen "save_to_csv()" sparar avgångsdatan till filen "trafikdata.csv"
    6. "matplotlib.pyplot" skapar i "plot_delays()" ett stapebdiagram över de 10 närmaste pendel avgångarna och deras försening (om de är sena) i minuter.
    7. Programmet är en konsolbaserad "while True" meny i "main()" där användaren får välja att se avgångarna från Stockholm City eller Odenplan.

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


5. Branchanalys
    I dagens samhälle där IT och AI blir en allt större del av vårt samhälle är det viktigt att kunna ta in realtidsdata för ex. kollektivtrafik. Det här projektet jag har gjort skulle jag säga är ett litet exempel på hur en framtida AI-utvecklare kan samla in data från en källa (i detta fall en API) för att sedan skapa framtida AI-modeller som kan förutse vilka sträckor bland pendeltågen som har störst risk att bli försenade.

6. Certifikat-koll
    För mig som framtida AI-utvecklare hade jag kunnat arbeta vidare med denna typ av program och datahantering så hade exempelvis ett AWS Certified Data Engineer kunnat vara något för mig. Då bygger man kunskap inom om hru man bygger pipelines i molnet med AWS för anrop och för lagring av CSV/data.

7. Reflektion
    Jag hade från bröjan skrivit ett program för elprisanalys men bytte sedan till att analysera tågtrafiken i Stockholm. Jag behöll mycket av den logiken jag hade i förra projektet men bytte ex. API och funktioner. Projekten som helhet tyckte jag var lite otydligt om vad man skulle göra exakt och vilka rubriker som skulle vara med i denna README-fil, men annars tycker jag att projektet var ganska kul. Jag har lärt mig mycket men det finns såklart mycket mer att lära. 

8. AI-Användning
    Under skapandet av projektet har jag använt mig av AI som ett stöd för att debugga och feltesta mitt program. Den har varit ett stöd under skapandet av projektet och har hjälpt mig att förstå mer hur API-anrop fungerar, då det var det momentet jag tyckte var extra svårt.

9. GitHub-Länk
   https://github.com/tindra9800/t-g_och-trafikanalys_stockholm 