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
   

4. Analys
    

5. Reflektion
    Jag hade från bröjan skrivit ett program för elprisanalys men bytte sedan till att analysera tågtrafiken i Stockholm.R
    

6. GitHub-Länk

    
