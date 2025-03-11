
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: it
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cerca documenti XLSX in .NET con GroupDocs.Search"
head_description: "Utilizza GroupDocs.Search for .NET per eseguire ricerche di testo efficienti in vari formati di documenti con C#."

############################# Header ############################
title: "Ricerca avanzata di testo nei documenti" 
description: "GroupDocs.Search for .NET semplifica la ricerca di testo nei formati di documento più comuni, consentendo di creare potenti query di ricerca nelle tue applicazioni .NET."
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
    title: "Che cos'è GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) è una potente libreria progettata per la ricerca e l'indicizzazione di testo completo nei documenti. Supporta oltre 70 formati di file, inclusi PDF, Word, PowerPoint, Excel, immagini e file ZIP, garantendo risultati di ricerca rapidi e accurati.

############################# Steps ############################
steps:
    enable: true
    title: "Come eseguire una ricerca di testo nei documenti XLSX"
    content: |
      [GroupDocs.Search](/search/net/) abilita operazioni avanzate di ricerca del contenuto nei documenti XLSX, consentendo risultati di ricerca affinati nelle applicazioni .NET.
      
      1. Imposta la cartella per memorizzare l'indice di ricerca.
      2. Scegli la cartella contenente i file XLSX.
      3. Configura opzioni di ricerca aggiuntive.
      4. Esegui la ricerca e rivedi i risultati.
   
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
        // Definisci il percorso per l'indice di ricerca
        Index index = new Index("c:/MyIndex");

        // Seleziona la cartella contenente i documenti da cercare
        index.Add("c:/MyDocuments");

        // Abilita la ricerca per omofoni per trovare parole che suonano simili
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Esegui una query di ricerca complessa
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Funzionalità avanzate di ricerca e indicizzazione"
  description: "GroupDocs.Search for .NET migliora la ricerca di testo e l'indicizzazione su oltre 70 formati di file, fornendo strumenti efficienti per localizzare e gestire le informazioni."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale potente"
      content: "Cerca testo in più tipi di documenti, inclusi PDF, documenti Word, presentazioni PowerPoint e fogli di calcolo. Utilizza funzionalità come corrispondenze esatte, ricerca fuzzy e jolly per affinare i risultati."

    # feature loop
    - title: "Indicizzazione rapida per grandi volumi di dati"
      content: "Crea e gestisci indici di ricerca per un recupero veloce delle informazioni. L'indicizzazione ottimizza le ricerche su ampie collezioni di documenti."

    # feature loop
    - title: "Supporto multilingue"
      content: "Esegui ricerche in oltre 80 lingue, con supporto per diverse disposizioni di tastiera e varianti di parole per migliorare l'accuratezza."

    # feature loop
    - title: "Impostazioni di ricerca personalizzabili"
      content: "Affina i parametri di ricerca con opzioni come sensibilità maiuscole/minuscole, filtri per intervallo di date e esclusione di parole per risultati migliori."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Esecuzione di query di ricerca avanzate"
      content: |
        Questo esempio dimostra come applicare query di ricerca per documenti XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Definisci la cartella per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Specifica il percorso ai file di documento
          index.Add("c:/MyDocuments");

          // Fornisci una password per documenti protetti
          index.Dictionaries.DocumentPasswords.Add("protected.xlsx", "123456");

          // Abilita la ricerca fuzzy per trovare parole simili
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Recupera i risultati della ricerca
          SearchResult result = index.Search("Loarem", options);
          
          // Elabora l'output della ricerca
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    title: "Esplora le funzionalità chiave"
    exclude: "document"
    description: "Sfrutta le funzionalità di ricerca avanzate e ad alte prestazioni."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca tra i documenti aziendali"
    exclude: "XLSX"
    description: "GroupDocs.Search supporta oltre 70 formati di file, inclusi documenti d'ufficio, consentendo ricerche rapide ed efficienti con capacità di indicizzazione."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Formato Documento Portabile Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---