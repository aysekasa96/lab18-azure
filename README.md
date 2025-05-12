Realtime gegevensstroomverwerking met Azure Stream Analytics en Azure Synapse Analytics

📖 Beschrijving
Dit project omvat het verwerken van een gegevensstroom met Azure Stream Analytics en het overbrengen ervan naar Azure Synapse Analytics. Er wordt een realtime gegevensstroom ontvangen van Azure Event Hubs, verwerkt en geschreven naar de Synapse Analytics-omgeving.

🚀 Gebruikte technologieën
Azure Stream Analytics – Realtime datastromen verwerken

Azure Event Hubs – Gegevensstromen opnemen en routeren

Azure Synapse Analytics – Een analytisch datawarehouse maken

📌 Installatie en configuratie
1️⃣ Azure-resources voorbereiden
Maak de volgende resources op Azure:

Azure Event Hubs: bron van streaminggegevens

Azure Synapse Analytics: SQL-pool voor het analyseren van gegevens

Azure Stream Analytics: systeem voor het verwerken en routeren van gegevensstromen

2️⃣ De vereiste repositories klonen
bash
git kloon https://github.com/MicrosoftLearning/dp-203-azure-data-engineer
cd dp-203/Allfiles/labs/18
Voer de volgende opdracht uit om de installatiebestanden te installeren:

Powershell
./setup.ps1
3️⃣ Azure Stream Analytics-taken configureren
Maak een toegangspunt voor het opnemen van gegevens uit Event Hubs.

Definieer het uitgangspunt voor het verzenden van gegevens naar Synapse Analytics.

Importeer de gegevensstroom in de SQL-sink met behulp van de volgende query:

SQL
SELECT EventProcessedUtcTime ALS OrderDateTime, ProductID, Hoeveelheid
IN [FactOrder]
VAN [bestellingen]
4️⃣ Starten met streamanalysebedrijf
bash
knooppunt ~/dp-203/Allfiles/labs/18/orderclient
Met deze opdracht worden verkooporders naar Event Hubs verzonden. U kunt de query opnieuw uitvoeren om de tabel in Synapse Analytics bij te werken.

🎯 Resultaat
Dit project demonstreert de realtime-gegevensstroomverwerkingsmogelijkheden van Azure Stream Analytics en biedt tegelijkertijd gegevensanalyses met Azure Synapse Analytics.
# lab18-azure
