---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: it
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Soluzione di ricerca e indicizzazione documenti Java per PDF, file Office e contenuti web"
head_description: "Ricerca testo potente e indicizzazione per applicazioni Java. Cerca e organizza facilmente i dati in PDF, Word, Excel, presentazioni, email e formati web."

############################# Header ############################
title: "Ricerca e indicizzazione dei documenti efficienti con l'API Java"
description: "Potenzia le applicazioni Java con robuste funzionalità di ricerca testuale in tutti i formati di documenti popolari."
words:
  for: "per"

actions:
  main: "Scarica Maven gratuitamente"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Inizia il tuo viaggio oggi!"
  description: "Esplora le funzionalità di GroupDocs.Search gratuitamente o ottieni una licenza per sbloccare il suo pieno potenziale."

release:
  title: "Versione {0} rilasciata"
  notes: "Scopri le novità"
  downloads: "Download"

code:
  title: "Trova testo nei file utilizzando Java"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Crea un indice per i tuoi documenti
    Index index = new Index("c:/MyIndex");

    // Aggiungi documenti all'indice per ricerche efficienti
    index.add("c:/MyDocuments");
    
    // Cerca parole o frasi specifiche, come
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Search"
  description: "Scopri le potenti capacità di ricerca testuale della libreria Java Java."
  features:
    # feature loop
    - title: "Operazioni di indicizzazione e ricerca in Java"
      content: "Con GroupDocs.Search for Java, puoi raccogliere, memorizzare e analizzare i dati in modo efficiente per creare indici dettagliati per ricerche più veloci e accurate."

    # feature loop
    - title: "Ottimizza la ricerca unendo indici"
      content: "Combina facilmente più indici con GroupDocs.Search for Java per semplificare le ricerche. Riduci l'impatto degli indici delta più piccoli consolidandoli in un indice ad alte prestazioni."

    # feature loop
    - title: "Supporto per layout di tastiera multilingue"
      content: "Cerca attraverso diverse lingue e layout di tastiera con GroupDocs.Search for Java. Supporta 88 lingue e 164 configurazioni di tastiera per un'elasticità senza pari."

    # feature loop
    - title: "Capacità di ricerca morfologica"
      content: "Trova diverse forme di parole come nomi singolari/plurali o varianti dei verbi utilizzando GroupDocs.Search for Java. Personalizza le opzioni di ricerca per l'inglese e altre lingue."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Search for Java è compatibile con i principali sistemi operativi e gestori di pacchetti."
  items:
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    Lavora con un'ampia gamma di formati di file utilizzando GroupDocs.Search for Java. [Visualizza l'elenco completo](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Caratteristiche di GroupDocs.Search for Java"
  description: "Gestisci efficacemente i contenuti dei documenti con capacità di ricerca avanzate che supportano formati come PDF, DOCX, XLSX, PPTX e altro."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parametri di ricerca personalizzabili"
      content: "Affina le ricerche utilizzando intervalli di date e filtri di sensibilità al maiuscolo."

    # feature loop
    - icon: "detect"
      title: "Controllo ortografico avanzato"
      content: "Cerca in modo efficiente con controllo ortografico, caratteri jolly e ignorando caratteri speciali."

    # feature loop
    - icon: "collect"
      title: "Risultati di ricerca filtrati"
      content: "Applica filtri per focalizzare i risultati della ricerca in base a tipi di documento specifici o criteri."

    # feature loop
    - icon: "get"
      title: "Importazione ed esportazione di dati di indici"
      content: "Importa facilmente dati per indicizzazione o esporta i risultati in file per ulteriori utilizzi."

    # feature loop
    - icon: "remove"
      title: "Salta file non necessari"
      content: "Ottimizza l'indicizzazione escludendo file o parole specifiche."

    # feature loop
    - icon: "style"
      title: "Elaborazione di HTML e URL"
      content: "Estrai contenuti HTML in file e genera URL per la navigazione attraverso i risultati della ricerca."

    # feature loop
    - icon: "detect"
      title: "Ricerca veloce in grandi indici"
      content: "Accelera le operazioni di ricerca dividendo grandi indici in pezzi gestibili."

    # feature loop
    - icon: "manipulate"
      title: "Indicizzazione basata su stream"
      content: "Indicizza i dati direttamente da stream o strutture dati."

    # feature loop
    - icon: "compare"
      title: "Gestisci query con errori di battitura"
      content: "Rileva errori di ortografia e suggerisci parole alternative per un'accuratezza migliore nella ricerca."

    # feature loop
    - icon: "unreadable_characters"
      title: "Supporto completo per archivi"
      content: "Indicizza archivi annidati e recupera elenchi dettagliati di file all'interno dei file ZIP."

    # feature loop
    - icon: "hidden_print"
      title: "Indicizzazione salva spazio"
      content: "Indici compatti per risparmiare spazio su disco e elaborare file protetti da password."

    # feature loop
    - icon: "style"
      title: "Supporto per sinonimi personalizzati"
      content: "Espandi il dizionario dei sinonimi per migliorare l'accuratezza della ricerca con opzioni su misura."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Prova le funzionalità di GroupDocs.Search for Java con questi esempi di codice."
  items:
    # code sample loop
    - title: "Aumenta l'accuratezza della ricerca con il matching fuzzy"
      content: |
        Esplora la flessibilità di GroupDocs.Search for Java per gestire i contenuti con potenti capacità di ricerca fuzzy. [Scopri di più](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Come elaborare il risultato della ricerca">}}
        ```java {style=abap}
        // Crea un indice
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Configura le opzioni di ricerca
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Cerca documenti contenenti la parola 'acqua' o la frase 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Elabora il risultato della ricerca
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Affina i risultati con espressioni regolari"
      content: |
        Utilizza espressioni regolari in GroupDocs.Search for Java per creare risultati di ricerca precisi e dettagliati. [Scopri tecniche avanzate](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Come cercare utilizzando espressioni regolari">}}
        ```java {style=abap}   
        // Crea un indice
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Cerca la frase in forma di testo

        // Il primo carattere caret all'inizio indica che questa è una ricerca con espressione regolare
        String query = "^^(.)\\1{1,}";
        // Cerca due o più caratteri identici all'inizio di una parola
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
