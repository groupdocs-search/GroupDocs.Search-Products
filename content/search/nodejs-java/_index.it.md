---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: it
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Library di ricerca e indicizzazione dei documenti Node.js per documenti, PDF, Office e Web"
head_description: "Soluzione avanzata di ricerca testuale per applicazioni Node.js per cercare, indicizzare e raccogliere dati da documenti: PDF, Word, Excel, presentazioni, email e formati di file web."

############################# Header ############################
title: "Cerca e indicizza documenti utilizzando l'API Node.js"
description: "Migliora le applicazioni Node.js implementando la ricerca testuale in tutti i formati di documenti popolari."
words:
  for: "per"

actions:
  main: "Download gratuito di NPM"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Inizia il tuo viaggio oggi!"
  description: "Esplora le funzionalità di GroupDocs.Search gratuitamente o ottieni una licenza per sbloccare il suo pieno potenziale."

release:
  title: "Versione {0} rilasciata"
  notes: "Scopri le novità"
  downloads: "Download"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Esegui ricerca di testo in una cartella con JavaScript"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Crea un indice per i tuoi documenti
    const index = new searchLib.Index('c:/MyIndex');

    // Aggiungi documenti all'indice per ricerche efficienti
    index.add('c:/MyDocuments');
    
    // Cerca parole o frasi specifiche, come
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Search"
  description: "Libreria Node.js JavaScript per ricerca di testo"
  features:
    # feature loop
    - title: "Operazioni di indicizzazione e ricerca Node.js"
      content: "L'indicizzazione in GroupDocs.Search for Node.js via Java raccoglie, memorizza e analizza i dati per ricerche precise ed efficienti. Questi indici sono frequentemente utilizzati per eseguire ricerche."

    # feature loop
    - title: "Unisci più indici per migliorare l'efficienza della ricerca"
      content: "L'API GroupDocs.Search for Node.js via Java consente di unire più indici in uno solo. Le modifiche frequenti creano vari indici delta, che possono rallentare le prestazioni di ricerca. La nostra soluzione unisce questi indici delta in un indice comune, contenente tutte le informazioni degli indici delta uniti, migliorando notevolmente l'efficienza della ricerca mantenendo invariati gli indici delta. Diverse funzionalità possono essere configurate per affinare questo processo."

    # feature loop
    - title: "Riconosci le query di ricerca da diversi layout di tastiera"
      content: "GroupDocs.Search for Node.js via Java riconosce le query di ricerca che non corrispondono al layout di tastiera. Attualmente sono supportate 88 lingue e 164 diversi layout di tastiera."

    # feature loop
    - title: "Cerca utilizzando forme morfologiche di parole"
      content: "Con GroupDocs.Search for Node.js via Java puoi cercare varie forme di parole, come nomi singolari e plurali o tutte le forme di un verbo. È possibile personalizzare le lingue per forme di parole specifiche."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Search for Node.js via Java supporta tutti i principali sistemi operativi e gestori di pacchetti."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    GroupDocs.Search for Node.js via Java consente di elaborare un'ampia gamma di formati di file. [Esplora l'elenco completo](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formati Office popolari
        * **Portabile:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Testo:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formati multimediali
        * **Formati di immagine popolari:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Immagini multi-pagina:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Video:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Altro
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Altro:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Caratteristiche di GroupDocs.Search for Node.js via Java"
  description: "Controlla i contenuti dei documenti aziendali utilizzando il nostro motore di ricerca avanzato, che supporta formati di file popolari inclusi PDF, DOCX, XLSX, PPTX e altro."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parametri flessibili"
      content: "Utilizza intervallo di date e sensibilità al maiuscolo come parametri di ricerca."

    # feature loop
    - icon: "detect"
      title: "Ricerca con controllo ortografico"
      content: "Usa frasi di ricerca con controllo ortografico e caratteri jolly e saltando caratteri speciali nelle query."

    # feature loop
    - icon: "collect"
      title: "Filtraggio dei risultati"
      content: "Imposta un filtro sui documenti nei risultati di ricerca."

    # feature loop
    - icon: "get"
      title: "Importazione ed esportazione"
      content: "Esegui importazione o utilizza un elenco per modificare i caratteri durante l'indicizzazione ed esporta in un file."

    # feature loop
    - icon: "remove"
      title: "Salta dati non necessari"
      content: "Salta selettivamente l'indicizzazione di file specifici e parole specifiche per indicizzare più rapidamente."

    # feature loop
    - icon: "style"
      title: "Elaborazione URL"
      content: "Estrai testo formattato HTML in un file e genera un URL per navigare nei risultati della ricerca in HTML."

    # feature loop
    - icon: "detect"
      title: "Ricerca rapida"
      content: "Dividi le ricerche in pezzi più piccoli per cercare rapidamente in grandi indici."

    # feature loop
    - icon: "manipulate"
      title: "Elaborazione basata su stream"
      content: "Indicizza documenti da stream e strutture dati."

    # feature loop
    - icon: "compare"
      title: "Gestire gli errori di battitura"
      content: "Abilita il numero esatto di occorrenze per ogni parola trovata per offrire suggerimenti di parole alternative in caso di errori di battitura."

    # feature loop
    - icon: "unreadable_characters"
      title: "Supporto per archivi"
      content: "Indicizza archivi ZIP all'interno di altri archivi ZIP e recupera l'elenco dei file indicizzati in un archivio."

    # feature loop
    - icon: "hidden_print"
      title: "Risparmio di spazio su disco"
      content: "Risparmia spazio con l'indicizzazione compatta e indicizza i documenti protetti da password."

    # feature loop
    - icon: "style"
      title: "Sinonimi personalizzati"
      content: "Aggiungi sinonimi in inglese al dizionario sinonimi predefinito."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Esplora le funzionalità di GroupDocs.Search for Node.js via Java con esempi."
  items:
    # code sample loop
    - title: "Utilizza la ricerca 'fuzzy' per aumentare la produttività"
      content: |
        Goditi la flessibile funzionalità di GroupDocs.Search for Node.js via Java per migliorare il controllo del contenuto dei documenti tramite algoritmi di ricerca sofisticati. [Scopri di più](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Come elaborare il risultato della ricerca">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Crea un indice
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Configura le opzioni di ricerca
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Cerca documenti contenenti la parola 'acqua' o la frase 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Elabora il risultato della ricerca
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Le espressioni regolari sono disponibili per scenari di ricerca avanzati"
      content: |
        GroupDocs.Search for Node.js via Java ci consente di utilizzare espressioni regolari per restringere il risultato della ricerca. [Scopri tecniche di ricerca avanzate](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Come cercare utilizzando espressioni regolari">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Crea un indice
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Cerca la frase in forma di testo

        // Il primo carattere caret all'inizio indica che questa è una ricerca con espressione regolare
        const query = '^^(.)\\1{1,}';
        // Cerca due o più caratteri identici all'inizio di una parola
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
