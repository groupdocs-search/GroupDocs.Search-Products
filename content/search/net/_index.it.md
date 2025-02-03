---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: it
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: "Biblioteca di ricerca e indicizzazione documenti .NET per PDF, file Office e altro"
head_description: "Potente soluzione .NET per la ricerca di testo e indicizzazione in documenti come PDF, Word, Excel, presentazioni, email e formati web."

############################# Header ############################
title: "Ricerca avanzata e indicizzazione dei documenti con l'API .NET"
description: "Potenzia le applicazioni .NET con capacità di ricerca testuale all'avanguardia in formati di documenti popolari."
words:
  for: "per"

actions:
  main: "Scarica Nuget gratuitamente"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Licenze"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Inizia il tuo viaggio oggi!"
  description: "Esplora le funzionalità di GroupDocs.Search gratuitamente o ottieni una licenza per sbloccare il suo pieno potenziale."

release:
  title: "Versione {0} rilasciata"
  notes: "Scopri le novità"
  downloads: "Download"

code:
  title: "Cerca testo nei file di una directory"
  more: "Altri esempi"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Crea un indice per i tuoi documenti
    Index index = new Index("c:/MyIndex");

    // Aggiungi documenti all'indice per ricerche efficienti
    index.Add("c:/MyDocuments");
    
    // Cerca parole o frasi specifiche, come
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Panoramica di GroupDocs.Search"
  description: "Esplora la libreria .NET C# per una ricerca e indicizzazione robusta del testo."
  features:
    # feature loop
    - title: "Funzionalità di indicizzazione e ricerca .NET"
      content: "Indicizza, memorizza e tratta i dati documentali in modo efficiente con GroupDocs.Search for .NET per operazioni di ricerca altamente accurate e veloci."

    # feature loop
    - title: "Combina indici per una migliore velocità di ricerca"
      content: "GroupDocs.Search for .NET consente di unire più indici per ottimizzare le prestazioni. Riduci l'impatto degli indici delta unendoli in un indice completo per ricerche più fluide."

    # feature loop
    - title: "Cerca attraverso diverse layout di tastiera"
      content: "Gestisci facilmente le query di ricerca in 88 lingue e 164 layout di tastiera con il riconoscimento intelligente di GroupDocs.Search for .NET."

    # feature loop
    - title: "Ricerche morfologiche di parole"
      content: "GroupDocs.Search for .NET supporta ricerche per varianti di parole come nomi singolari/plurali e diverse forme verbali, personalizzabili per varie lingue."

############################# Platforms ############################
platforms:
  enable: true
  title: "Indipendenza dalla piattaforma"
  description: "GroupDocs.Search for .NET funziona senza problemi su principali sistemi operativi e gestori di pacchetti."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formati di file supportati"
  description: |
    Elabora un'ampia gamma di formati di file con GroupDocs.Search for .NET. [Visualizza tutti i formati supportati](https://docs.groupdocs.com/search/net/supported-document-formats/).
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
  title: "Caratteristiche principali di GroupDocs.Search for .NET"
  description: "Semplifica la gestione dei documenti con capacità avanzate di ricerca in formati popolari come PDF, DOCX, XLSX, PPTX e altro."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parametri di ricerca flessibili"
      content: "Utilizza filtri come intervalli di date e sensibilità al maiuscolo per affinare la tua ricerca."

    # feature loop
    - icon: "detect"
      title: "Controllo ortografico intelligente"
      content: "Cerca frasi con correzione ortografica, caratteri jolly e caratteri speciali ignorati."

    # feature loop
    - icon: "collect"
      title: "Risultati di ricerca filtrati"
      content: "Personalizza e filtra i risultati di ricerca per tipo o criteri di documento."

    # feature loop
    - icon: "get"
      title: "Importazione ed esportazione di indici"
      content: "Importa dati, modifica le impostazioni di indicizzazione ed esporta risultati indicizzati."

    # feature loop
    - icon: "remove"
      title: "Escludi dati irrilevanti"
      content: "Ottimizza l'indicizzazione saltando file o parole specifiche."

    # feature loop
    - icon: "style"
      title: "Estrazione URL"
      content: "Converti testi in formato HTML in file e genera link per i risultati della ricerca."

    # feature loop
    - icon: "detect"
      title: "Ricerca ad alta velocità"
      content: "Dividi grandi indici in parti più piccole per una elaborazione più veloce."

    # feature loop
    - icon: "manipulate"
      title: "Gestione dei dati semplificata"
      content: "Indicizza documenti direttamente da stream e strutture dati."

    # feature loop
    - icon: "compare"
      title: "Rilevamento di errori di battitura"
      content: "Suggerisci parole alternative e tieni traccia delle occorrenze per migliorare l'accuratezza."

    # feature loop
    - icon: "unreadable_characters"
      title: "Supporto per archivi"
      content: "Indicizza archivi ZIP annidati e recupera i dettagli dei file in essi."

    # feature loop
    - icon: "hidden_print"
      title: "Indicizzazione efficiente"
      content: "Risparmia spazio su disco con indicizzazione compatta e elabora documenti protetti da password."

    # feature loop
    - icon: "style"
      title: "Sinonimi personalizzati"
      content: "Aggiungi e gestisci sinonimi per risultati di ricerca su misura."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Esempi di codice"
  description: "Scopri le potenti capacità di GroupDocs.Search for .NET con esempi pratici."
  items:
    # code sample loop
    - title: "Aumenta la produttività con ricerca fuzzy"
      content: |
        Sfrutta GroupDocs.Search for .NET per il controllo dei contenuti flessibile e accurato attraverso algoritmi di ricerca avanzati. [Esplora di più](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Come elaborare il risultato della ricerca">}}
        ```csharp {style=abap}
        // Crea un indice
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Configura le opzioni di ricerca
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Cerca documenti contenenti la parola 'acqua' o la frase 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Elabora il risultato della ricerca
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ricerca avanzata con espressioni regolari"
      content: |
        GroupDocs.Search for .NET supporta espressioni regolari per ricerche precise. [Scopri tecniche avanzate](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Come cercare utilizzando espressioni regolari">}}
        ```csharp {style=abap}   
        // Crea un indice
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Cerca la frase in forma di testo

        // Il primo carattere caret all'inizio indica che questa è una ricerca con espressione regolare
        string query = "^^(.)\\1{1,}";
        // Cerca due o più caratteri identici all'inizio di una parola
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
