
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: it
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cerca frasi in PDF utilizzando .NET"
head_description: "GroupDocs.Search for .NET potenzia le applicazioni C# con potenti capacità di ricerca per frasi nel contenuto dei documenti."

############################# Header ############################
title: "Cerca frasi nei documenti" 
description: "Trova rapidamente frasi specifiche con GroupDocs.Search for .NET. Integra funzionalità di ricerca efficiente nelle tue applicazioni .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Caratteristiche di GroupDocs.Search"
    link: "/search/net/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) è una libreria potente per indicizzare e cercare testi nei documenti. Supporta oltre 70 formati di file, tra cui PDF, documenti Word, fogli Excel, immagini e file ZIP, consentendo risultati di ricerca rapidi e precisi.

############################# Steps ############################
steps:
    enable: true
    title: "Come cercare frasi in documenti PDF"
    content: |
      [GroupDocs.Search](/search/net/) semplifica la ricerca in documenti PDF. Utilizza varie opzioni per affinare i risultati di ricerca nelle applicazioni .NET.
      
      1. Imposta la cartella per l'indice di ricerca.
      2. Specifica la cartella contenente i file PDF.
      3. Configura le impostazioni di ricerca.
      4. Recupera e processa i risultati della ricerca.
   
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
        // Percorso per memorizzare l'indice di ricerca
        Index index = new Index("c:/MyIndex");

        // Cartella contenente i documenti
        index.Add("c:/MyDocuments");

        // Configura le opzioni di ricerca
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Esegui la ricerca
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Scopri il motore di ricerca documentale .NET"
  description: "GroupDocs.Search for .NET consente ricerche per frasi in oltre 70 formati di file. Localizza e gestisci i dati con capacità di ricerca avanzate."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Caratteristiche chiave di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca per frasi"
      content: "Cerca frasi esatte nei documenti aziendali, inclusi PDF, file Word, presentazioni e fogli di calcolo. Utilizza caratteri jolly e altre opzioni se la frase esatta è sconosciuta."

    # feature loop
    - title: "Indicizzazione dei dati efficiente"
      content: "Crea e riutilizza indici di ricerca per accelerare le ricerche nei documenti. L'indicizzazione struttura i dati in modo efficiente, rendendo le ricerche per frasi più veloci."

    # feature loop
    - title: "Supporto multilingue"
      content: "Cerca documenti in oltre 80 lingue. Supporta layout di tastiera diversi e forme morfologiche delle parole per una migliore precisione di ricerca."

    # feature loop
    - title: "Opzioni di ricerca flessibili"
      content: "Personalizza le ricerche con funzionalità come sensibilità alle maiuscole, ricerca fuzzy e omofona, filtraggio dei documenti e altro."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzo di tecniche di ricerca avanzate"
      content: |
        Scopri come creare query per cercare in PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Specifica la cartella per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Imposta il percorso ai documenti da cercare
          index.Add("c:/MyDocuments");

          // Crea una query per una frase specifica
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Recupera i risultati della ricerca
          SearchResult result = index.Search(query);
          
          // Processa e utilizza i risultati
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Funzionalità avanzate"
    exclude: "phrase"
    description: "Utilizza funzionalità di ricerca potenti ed efficienti."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Ricerca per frasi nei documenti aziendali"
    exclude: "PDF"
    description: "GroupDocs.Search supporta ricerche in oltre 70 formati di documento. Utilizza opzioni avanzate e indicizzazione per semplificare il tuo processo di ricerca."
    items: 
        # format loop 1
        - name: "Ricerca frase in DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca frase in PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca frase in PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca frase in TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca frase in XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---