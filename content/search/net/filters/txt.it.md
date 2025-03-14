
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: it
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cerca in documenti TXT utilizzando .NET"
head_description: "GroupDocs.Search for .NET potenzia le applicazioni C# con ricerche testuali efficienti in vari formati di documenti aziendali."

############################# Header ############################
title: "Cerca testo in documenti aziendali" 
description: "GroupDocs.Search for .NET consente ricerche di testo potenti e flessibili nei tuoi documenti. Integra facilmente la funzionalità di ricerca nelle applicazioni .NET."
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
       [GroupDocs.Search for .NET](/search/net/) è una potente libreria per una ricerca testuale efficiente e l'indicizzazione dei documenti. Supporta oltre 70 formati di file, inclusi documenti standard del settore come PDF, Word, Excel e PowerPoint. Migliora le prestazioni di ricerca con risultati rapidi e accurati.

############################# Steps ############################
steps:
    enable: true
    title: "Come cercare nei dati TXT"
    content: |
      [GroupDocs.Search](/search/net/) consente ricerche testuali efficienti in documenti TXT, rendendolo ideale per applicazioni .NET.
      
      1. Imposta una cartella per memorizzare l'indice di ricerca.
      2. Seleziona la cartella contenente i tuoi file.
      3. Configura le opzioni di ricerca per elaborare solo documenti TXT.
      4. Esegui la ricerca e recupera i risultati.
   
    code:
      platform: "net"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Risultato della ricerca"
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
        // Percorso per memorizzare l'indice di ricerca riutilizzabile
        Index index = new Index("c:/MyIndex");

        // Cartella contenente documenti
        index.Add("c:/MyDocuments");

        // Cerca solo all'interno di formati di file specifici
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".txt");

        // Recupera i risultati della ricerca
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Funzionalità di ricerca avanzate"
  description: "GroupDocs.Search for .NET consente ricerche di testo sofisticate in oltre 70 formati di file. L'indicizzazione migliora l'efficienza della ricerca e aiuta a gestire efficacemente il contenuto dei documenti."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale avanzata"
      content: "Estrai testo rilevante da documenti aziendali popolari, inclusi PDF, file Word, presentazioni e fogli di calcolo. Supporta diverse tecniche di ricerca come ricerca approssimata, rilevamento di omofoni e caratteri jolly."

    # feature loop
    - title: "Indicizzazione ottimizzata per ricerche più veloci"
      content: "Crea e riutilizza indici di ricerca per migliorare la velocità di ricerca. L'indicizzazione ottimizza le prestazioni quando si cercano ampie collezioni di documenti."

    # feature loop
    - title: "Supporto per più lingue"
      content: "Esegui ricerche in documenti scritti in oltre 80 lingue. Rileva diverse disposizioni di tastiera e variazioni di parole per migliorare l'accuratezza."

    # feature loop
    - title: "Impostazioni di ricerca flessibili"
      content: "Affina i risultati di ricerca con opzioni personalizzabili, incluse filtri, espressioni regolari e impostazioni di sensibilità al maiuscolo."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtra i documenti da elaborare"
      content: |
        Scopri come restringere le ricerche di documenti usando filtri
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Configura un indice che esclude determinati formati di file
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Specifica la directory dei documenti
          index.Add("c:/MyDocuments");

          // Recupera i risultati della ricerca
          SearchResult result = index.Search("Lorem");
          
          // Elabora e utilizza l'output della ricerca
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
          - title: "Scarica risultato"
            icon: "download"
            link: "/examples/search/formats/searchfilters.txt"
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
  description: "Prova le funzionalità di GroupDocs.Search gratuitamente o richiedi una licenza"
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
    title: "Caratteristiche chiave"
    exclude: "filters"
    description: "Esegui ricerche di dati accurate ed efficienti."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Trova dati nei tuoi documenti aziendali"
    exclude: "TXT"
    description: "GroupDocs.Search supporta oltre 70 formati di file, consentendo un'elaborazione e una ricerca efficienti di documenti d'ufficio popolari."
    items: 
        # format loop 1
        - name: "Filtri di ricerca per DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Filtri di ricerca per PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Filtri di ricerca per PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Filtri di ricerca per TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Filtri di ricerca per XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---