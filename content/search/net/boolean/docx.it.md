
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: it
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cerca DOCX in .NET utilizzando operatori booleani"
head_description: "L'API GroupDocs.Search for .NET consente agli sviluppatori C# di cercare il contenuto dei documenti utilizzando operatori booleani come AND, OR e NOT."

############################# Header ############################
title: "Ricerca testuale con logica boolean" 
description: "GroupDocs.Search for .NET semplifica la creazione di query di ricerca avanzate utilizzando operatori booleani (AND, OR, NOT) all'interno delle tue applicazioni .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica gratuitamente"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) è una libreria completa per la ricerca e l'indicizzazione del testo nei documenti. Supporta oltre 70 formati di file, come PDF, Word, PowerPoint, Excel, immagini e file ZIP, consentendo un'elaborazione efficiente di grandi quantità di informazioni.

############################# Steps ############################
steps:
    enable: true
    title: "Come cercare il contenuto di documenti DOCX utilizzando la logica boolean"
    content: |
      [GroupDocs.Search](/search/net/) rende la ricerca del contenuto dei documenti DOCX diretta. Fornisce condizioni di ricerca logica booleana per affinare i risultati nelle applicazioni .NET.
      
      1. Specifica la cartella in cui memorizzare l'indice di ricerca.
      2. Scegli la cartella contenente i file DOCX.
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
        // Imposta il percorso nella cartella degli indici
        Index index = new Index("c:/MyIndex");

        // Specifica la cartella contenente i documenti da cercare
        index.Add("c:/MyDocuments");

        // Esegui una ricerca utilizzando una query complessa
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Esplora funzionalità avanzate per la ricerca e l'indicizzazione dei documenti"
  description: "La libreria GroupDocs.Search for .NET semplifica la ricerca e l'indicizzazione del testo per oltre 70 formati di file. Trova e gestisci informazioni in modo efficace con strumenti di ricerca avanzati."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Funzionalità principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale potente"
      content: "Cerca testo attraverso vari tipi di file, inclusi PDF, documenti Word, presentazioni PowerPoint e fogli di calcolo. Utilizza funzionalità come corrispondenze esatte, ricerche fuzzy e caratteri jolly per affinare i risultati."

    # feature loop
    - title: "Indicizza set di dati di grandi dimensioni"
      content: "Crea e mantieni indici per ricerche più veloci. L'indicizzazione struttura e organizza i dati, rendendo più semplice la ricerca di collezioni di documenti estese."

    # feature loop
    - title: "Supporto per più lingue"
      content: "Cerca documenti in oltre 80 lingue, con supporto per diversi layout di tastiera e forme morfologiche delle parole per migliorare l'accuratezza della ricerca."

    # feature loop
    - title: "Opzioni di ricerca personalizzabili"
      content: "Regola le impostazioni di ricerca con funzionalità come distinzione tra maiuscole e minuscole, filtri per intervallo di date e la possibilità di escludere parole o dati specifici durante l'indicizzazione."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzare query di ricerca booleane avanzate"
      content: |
        Questo esempio dimostra come applicare query booleane per cercare documenti DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Imposta la cartella per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Specifica il percorso dei documenti da cercare
          index.Add("c:/MyDocuments");

          // Crea una query di ricerca utilizzando la logica booleana
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Recupera i risultati della ricerca
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.docx"
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
    title: "Scopri le caratteristiche chiave"
    exclude: "boolean"
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
    title: "Cerca tra i formati di documento più comuni"
    exclude: "DOCX"
    description: "GroupDocs.Search supporta oltre 70 formati di file. Personalizza le regole di ricerca e sfrutta l'indicizzazione per risparmiare tempo e fatica."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Formato Documento Portabile Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---