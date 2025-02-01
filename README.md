# Monitoraggio inquinamento Sulcis
Questo repository raccoglie i dati di **ARPA Sardegna** (Arpas) delle **contaminazioni di suole e faldi di Portoscuso** (Sud Sardegna) in formato csv. I dati sono stati ottenuti da Arpas tramite richiesta di accesso civico generalizzato (FOIA) e puliti ed elaborati da **Slow News**.

I dati sono presentati nell'inchiesta di Slow News **[Cicatrici: tutti i numeri di un disastro ambientale](https://www.slow-news.com/serie/il-cammino-del-sulcis/sulcis-portoscuso-dati-inquinanti-jtf)**, episodio finale de [Il cammino del Sulcis](https://www.slow-news.com/serie/il-cammino-del-sulcis), una serie sulle sfide della giusta transizione del Sulcis Iglesiente.

Nello specifico, sono presenti i seguenti dataset:
- contaminazioni dei suoli di Portoscuso e dintorni, anno 2022
- contaminazioni delle falde industriali di Portoscuso, anno 2020
- contaminazioni delle falde urbane di Portoscuso, anni da 2020 a 2022 a seconda del punto di monitoraggio
- coordinate geografiche dei punti di monitoraggio di suoli e falde urbane e industriali

## Contaminazioni dei suoli di Portoscuso e dintorni, anno 2022
Il file è [Contaminazioni suoli Portoscuso e dintorni 2022.csv](https://github.com/schenzio/inquinamento-Sulcis/blob/main/Contaminazioni%20suoli%20Portoscuso%20e%20dintorni%202022.csv). Contiene un'elaborazione di dati estratti dal PDF [Relazione Arpas dicembre 2023 - PIANO DI DISINQUINAMENTO PER IL RISANAMENTO DEL TERRITORIO DEL SULCIS IGLESIENTE 2022 ](https://journaliststudio.google.com/pinpoint/document-view?collection=c4fef29928882ea6&labels=0e82cdd545b79291&p=1&docid=274783dccae701af_c4fef29928882ea6&page=1). 

I dati descrivono i prelievi di diversi contaminanti nel suoli del comune di Portoscuso e dintorni e sono così strutturati:

Nome colonna | Tipo colonna | Descrizione colonna
------------ | -------------| ------------------- |
Punto di prelievo (abbr) |	string | Il nome del punto di prelievo, così come riportato nella relazione Arpas (es. P2)
Punto di prelievo | string | Il nome esteso del punto di prelievo, comprensivo del nome della località indicata nella realazione Arpas (es. PORTOSCUSO PERDAIAS P2 )
Data prelievo  | string | La data del prelievo
Comune | string | Il comune in cui è situato il punto di prelievo
Contaminante | string | Nome del contaminante prelevato
Concentrazione (mg/Kg)	| integer | La concentrazione del contaminante, espressa in milligrammi su kili
Soglia di legge (mg/Kg)	| integer | La concentrazione massima legale del contaminante in esame, espressa in milligrammi su kili
Concentrazione in eccesso (mg/Kg) | string | La concentrazione in eccesso del contaminante in esame, espressa in microgrammi su kili e calcolata come differenza tra la concentrazione e la soglia di legge
Indice superamento	| integer |  L'indice che misura quante cioè volte in un dato punto la concentrazione di un contaminante supera i limiti legali. È calcolato come rapporto tra la concentrazione e la soglia di legge. 
ID | string | Il codice identificativo di un certo prelievo, formato dal nome del punto di prelievo più il contaminante prelevato (es. P2 Zinco)

## Contaminazioni delle falde industriali di Portoscuso, anno 2020
Il file è [Contaminazioni falde industriali Portoscuso 2020.csv](https://github.com/schenzio/inquinamento-Sulcis/blob/main/Contaminazioni%20falde%20industriali%20Portoscuso%202020.csv). Contiene un'elaborazione di dati estratti dal PDF 
[Relazione Arpas dicembre 2021 - PIANO DI DISINQUINAMENTO PER IL RISANAMENTO DEL TERRITORIO DEL SULCIS IGLESIENTE 2020](https://journaliststudio.google.com/pinpoint/document-view?collection=c4fef29928882ea6&labels=0e82cdd545b79291&p=1&docid=4b49006673dff67b_c4fef29928882ea6&page=1). 

I dati descrivono i prelievi di diversi contaminanti nelle falde sotto gli impianti di Portovesme, l'area industriale di Portoscuso. Il 2020 è l'ultimo anno disponibile per questi dati. Arpas dichiara di aver interrotto il monitoraggio perché il quadro delle contaminazioni era stabile negli ultimi anni. I dati sono così strutturati:

Nome colonna | Tipo colonna | Descrizione colonna
------------ | -------------| ------------------- |
Punto di prelievo |	string | Il nome esteso del punto di prelievo indicato nella realazione Arpas, unito al nome dell'impianto industriale di appartenenza (es. Alcoa PZ 4 )
Data prelievo	| string | La data del prelievo
Contaminante | string | Nome del contaminante prelevato
Area industriale | string | L'area dell'impianto industriale in cui è situato il punto di prelievo
Concentrazione  (μg/l)		| integer | La concentrazione del contaminante, espressa in microgrammi su litri
Soglia di legge  (μg/l)		| integer | La concentrazione massima legale del contaminante in esame, espressa in microgrammi su litri
Concentrazione in eccesso  (μg/l)	 | string | La concentrazione in eccesso del contaminante in esame, espressa in microgrammi su litri e calcolata come differenza tra la concentrazione e la soglia di legge
Indice superamento	| integer |  L'indice che misura quante volte in un dato punto la concentrazione di un contaminante supera i limiti legali. È calcolato come rapporto tra la concentrazione e la soglia di legge. 
ID | string | Il codice identificativo di un certo prelievo, formato dal nome del punto di prelievo più il contaminante prelevato (es. Alcoa PZ 4 - Cadmio)

## Contaminazioni delle falde urbane di Portoscuso, anni da 2020 a 2022 
Il file è [Contaminazioni falde urbane Portoscuso 2020-2022.csv](https://github.com/schenzio/inquinamento-Sulcis/blob/main/Contaminazioni%20falde%20urbane%20Portoscuso%202020-2022.csv). Contiene un'elaborazione di dati estratti dai:
- il PDF [Relazione Arpas dicembre 2021 - PIANO DI DISINQUINAMENTO PER IL RISANAMENTO DEL TERRITORIO DEL SULCIS IGLESIENTE 2020](https://journaliststudio.google.com/pinpoint/document-view?collection=c4fef29928882ea6&labels=0e82cdd545b79291&p=1&docid=4b49006673dff67b_c4fef29928882ea6&page=1), per i punti di monitoraggio delle falde di Paringianu
- i dati della Rete regionale di monitoraggio delle acque sotterranee 2021-2022 nel Comune di Portoscuso, per tutti gli altri punti, forniti a Slow News direttamente in formato .csv da Arpas

I dati descrivono i prelievi di diversi contaminanti nelle falde urbane di Portoscuso. Gli anni vanno dal 2020 al 2022, a seconda dell'ultimo anno di monitoraggio disponibile per ciascun punto di prelievo

Nome colonna | Tipo colonna | Descrizione colonna
------------ | -------------| ------------------- |
Punto di prelievo |	string | Il nome del punto di prelievo
Data prelievo	| string | La data del prelievo
Contaminante | string | Nome del contaminante prelevato
Area industriale | string | L'area dell'impianto industriale in cui è situato il punto di prelievo
Concentrazione  (μg/l)		| integer | La concentrazione del contaminante, espressa in microgrammi su litri
Soglia di legge  (μg/l)		| integer | La concentrazione massima legale del contaminante in esame, espressa in microgrammi su litri
Concentrazione in eccesso  (μg/l)	 | string | La concentrazione in eccesso del contaminante in esame, espressa in microgrammi su litri e calcolata come differenza tra la concentrazione e la soglia di legge
Indice superamento	| integer |  L'indice che misura quante volte in un dato punto la concentrazione di un contaminante supera i limiti legali. È calcolato come rapporto tra la concentrazione e la soglia di legge. 
ID | string | Il codice identificativo di un certo prelievo, formato dal nome del punto di prelievo più il contaminante prelevato (es. Paringianu EP2 - Manganese)
