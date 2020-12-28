# Medical_Device_Network_Graph
NLP powered graph exploration of FDA's Medical Device Report database

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;This project aims to help actors in the medical drug and device field to visualize relationships between adverse medical device reports in the FDA MDR database. Patient, provider, and manufacturer reported unexpected medical occurrences, known as adverse events (AEs), will be used to identify potential device-drug interactions that result in negative outcomes. Currently, no visualization tool exists to perform this task.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Due to small clinical trial sample sizes and nearly infinite combinations of device-drug interactions, post-FDA approval safety monitoring is both a regulatory requirement and critical to developing a medical device’s safety profile. This data visualization tool will help medical device companies identify emerging safety concerns using the FDA’s post-approval report data.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Using the FDA’s medical device event report databases (https://www.fda.gov/medical-devices), free report text is parsed into lists of medical ontology concepts (such as UMLS, MEDRA, WHO or SNOMED-CT). Concepts can be anything from diseases, treatments and pharmaceuticals to symptoms, organs or biological molecules. Example concepts might include: acute chest pain, lumbar sprain, aspirin, nausea, small intestine, and hemoglobin. Each report’s concept list is tied to the associated medical device. When an end-user conducts research on a device they will be presented with a network graph of medical concepts associated with that device, with edge thickness scaled to frequency a concept is reported for that device. A second view shows devices whose reported medical concepts are related to a user input concept. Similarity between two concepts is determined using a set of pretrained medical concept co-occurrence embeddings. The dataset includes about 1.1 million AE reports representing 57,000 unique devices and 18,000 medical concepts.

<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Exploration of an Insulin Pump device and an Insulin Pump + Monitor device:
<br>
<center><img src='2x insulin pumps.png'></img></center>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Exploration of other devices with 'Hyperglycemia' concept present in MDRs:
<br>
<center><img src='hyperglycemia related devices.png'></img></center>
<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Exploratory data analysis of the FDA medical device adverse event report database:
<br>
<center><img src='MDR EDA.png'></img></center>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Results from experiments conducted to quantify app performance:
<center><img src='MDR graph exp results.png'></img></center>
