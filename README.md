# DFRWS 2023 - LIFTY Forensic Validation

Dit project is uitgevoerd tijdens de Minor Digital Forensics aan Hogeschool Leiden.

## Casus

Binnen de DFRWS 2023 "*The Troubled Elevator*" challenge stond een liftincident centraal waarbij een directielid vast kwam te zitten in de lift. De oorzaak was niet direct duidelijk, er kon sprake zijn van een technische storing, menselijke fout of opzettelijke manipulatie van de PLC.

Binnen dit project hebben wij niet het oorspronkelijke incident opnieuw onderzocht, maar het eerdere forensische onderzoek van een andere groep gevalideerd. Het doel was om te controleren in hoeverre hun bevindingen reproduceerbaar waren en of de conclusies voldoende werden ondersteund door het beschikbare digitale bewijsmateriaal.

## Wat heb ik gedaan?

Binnen het validatieonderzoek heb ik meegewerkt aan het opnieuw analyseren en controleren van verschillende onderdelen van het oorspronkelijke onderzoek.

Mijn werkszaamheden bestonden onder andere uit:

- Het valideren van bevindingen uit PLC-memorydumps
- Het opnieuw analyseren van PLC-memory en vergelijken van resultaten met het oorspronkelijke onderzoekslogboek
- Het controleren van bevindingen aan de hand van hashing en reproduceerbare analyses
- Het analyseren en valideren van UMAS/Modbus-netwerkverkeer
- Het correleren van netwerkactiviteit met CCTV-timestamps
- Het uitvoeren van testcases met een fysieke PLC-opstelling
- Het vergelijken van normaal PLC-verkeer, statuswijzigingen en wijzigingen aan PLC-logica met het oorspronkelijke netwerkverkeer
- Het ondersteunen van de reconstructie en validatie van de onderzoekstijdlijn

Voor de PLC-memoryvalidatie is daarnaast gebruikgemaakt van een Python-script om memory dumps geautomatiseerd te analyseren en bevindingen reproduceerbaar te vergelijken.

## Tooling / methodieken

- Wireshark
- Schneider Modicon M221 PLC
- EcoStruxure Machine Expert Basic
- Python
- HxD
- Binwalk
- Volatility 3
- PCAP-analyse
- PLC-memoryanalyse
- Windows-memoryanalyse
- UMAS/Modbus-analyse
- hashing voor integriteitscontrole
- tijdlijnanalyse en CCTV-correlatie
- gecontroleerde testcases
- Validatie en reproduceerbaarheid van forensische bevindingen

## Resultaat

De belangrijkste technische bevindingen uit het oorspronkelijke onderzoek konden grotendeels worden gereproduceerd. Door resultaten uit netwerkverkeer, PLC-memory, Windows-memory, CCTV en gecontroleerde testcases met elkaar te vergelijken, kon worden beoordeeld welke conclusies technische voldoende werden ondersteund.

Het project liet daarbij ook zien dat niet iedere oorspronkelijke bevinding volledig kon worden bevestigd. Daarom is tijden de validatie onderscheid gemaakt tussen bevestigde, gedeeltelijk bevestigde en niet-bevestigde bevindingen.

## Afbakening

Deze repository bevat alleen een samenvatting van het uitgevoerde project. Orginele onderzoeksbestanden, PCAP-bestanden
