
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: it
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Ricerca Sensibile al Caso in DOCX Utilizzando .NET"
head_description: "L'API GroupDocs.Search for .NET consente agli sviluppatori C# di eseguire ricerche sensibili al caso su vari documenti."

############################# Header ############################
title: "Ricerca Sensibile al Caso" 
description: "GroupDocs.Search for .NET consente di creare query di ricerca avanzate sensibili al caso all'interno delle tue applicazioni .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica Gratis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Che cos'è GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) è una libreria robusta per la ricerca di testo e l'indicizzazione nei documenti. Supporta oltre 70 formati di file, inclusi PDF, Word, PowerPoint, Excel, immagini e file ZIP, garantendo una gestione efficiente di grandi volumi di dati.

############################# Steps ############################
steps:
    enable: true
    title: "Come Eseguire una Ricerca Sensibile al Caso in Documenti DOCX"
    content: |
      [GroupDocs.Search](/search/net/) semplifica la ricerca sensibile al caso in documenti DOCX. Usalo per affinare i risultati nelle applicazioni .NET.
      
      1. Definisci la cartella per memorizzare l'indice di ricerca.
      2. Scegli la cartella contenente file DOCX.
      3. Esegui la ricerca e recupera i risultati.
      4. Elabora i risultati.
   
    code:
      platform: "net"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Imposta il percorso alla cartella dell'indice
        Index index = new Index("c:/MyIndex");

        // Specifica la cartella contenente i documenti da cercare
        index.Add("c:/MyDocuments");

        // Attiva la ricerca sensibile al caso nelle opzioni
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Esegui la ricerca
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Funzionalità Avanzate per la Ricerca e l'Indicizzazione dei Documenti"
  description: "La libreria GroupDocs.Search for .NET semplifica la ricerca di testo e l'indicizzazione in oltre 70 formati di file. Trova e gestisci informazioni in modo efficace con potenti strumenti di ricerca."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Caratteristiche Principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca Testo Avanzata"
      content: "Cerca testo in vari formati di file, inclusi PDF, documenti Word, fogli di calcolo e presentazioni. Utilizza opzioni come corrispondenze esatte, ricerca fuzzy e caratteri jolly per risultati precisi."

    # feature loop
    - title: "Indicizzazione di Grandi Dataset"
      content: "Crea e mantieni indici per ricerche più rapide. Un'indicizzazione organizzata semplifica la ricerca di collezioni estese di documenti."

    # feature loop
    - title: "Supporto Multilingue"
      content: "Cerca attraverso documenti in oltre 80 lingue, con supporto per diverse tastiere e forme delle parole per risultati più accurati."

    # feature loop
    - title: "Opzioni di Ricerca Personalizzabili"
      content: "Personalizza le impostazioni di ricerca con sensibilità al caso, filtri di intervallo di date e la possibilità di escludere parole o dati specifici durante l'indicizzazione."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzo di Query di Ricerca Sensibili al Caso"
      content: |
        Questo esempio mostra come utilizzare query sensibili al caso per la ricerca di documenti DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Imposta la cartella per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Specifica il percorso ai documenti da cercare
          index.Add("c:/MyDocuments");

          // Crea una query di ricerca
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Attiva le opzioni di ricerca sensibile al caso
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Cerca testo nei documenti
          SearchResult result = index.Search(wordQuery, options);
          
          // Elabora i risultati della ricerca
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Copia"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzionalità di GroupDocs.Search gratuitamente oppure richiedi una licenza"
  items:
    #  loop
    - title: "Download di Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Scopri le Caratteristiche Chiave"
    exclude: "case-sensitive"
    description: "Esplora funzionalità di ricerca avanzate ed efficienti."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca Formati Documentali Popolari"
    exclude: "DOCX"
    description: "GroupDocs.Search supporta oltre 70 formati di file. Personalizza le regole di ricerca e utilizza l'indicizzazione per risparmiare tempo e sforzi."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Formato Documento Portabile Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---