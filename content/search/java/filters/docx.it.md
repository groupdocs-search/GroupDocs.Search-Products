
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: it
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cerca in documenti DOCX utilizzando Java"
head_description: "GroupDocs.Search for Java aggiunge potenti capacità di ricerca testuale alle applicazioni Java, supportando vari formati di documenti aziendali."

############################# Header ############################
title: "Trova testo in documenti aziendali" 
description: "GroupDocs.Search for Java consente di cercare testo in documenti utilizzando query flessibili e precise. Integra facilmente la funzionalità di ricerca nelle applicazioni Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica gratuitamente"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) è una libreria robusta per una ricerca testuale rapida e l'indicizzazione dei documenti. Supporta oltre 70 formati di file, inclusi standard del settore come PDF, Word, Excel e PowerPoint. Migliora le tue applicazioni con capacità di ricerca ad alta velocità e precisione.

############################# Steps ############################
steps:
    enable: true
    title: "Come cercare in documenti DOCX"
    content: |
      [GroupDocs.Search](/search/java/) consente ricerche testuali rapide ed efficienti in documenti DOCX, perfette per applicazioni Java.
      
      1. Specifica una cartella per memorizzare l'indice di ricerca.
      2. Seleziona la cartella contenente i tuoi documenti.
      3. Configura le opzioni di ricerca per limitare i risultati ai documenti DOCX.
      4. Esegui la ricerca e ottieni i risultati.
   
    code:
      platform: "java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Risultato della ricerca"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Directory per memorizzare l'indice di ricerca riutilizzabile
        Index index = new Index("c:/MyIndex");

        // Cartella contenente i documenti
        index.add("c:/MyDocuments");

        // Filtra le ricerche per formato di documento
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".docx");

        // Recupera i risultati della ricerca
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacità di ricerca avanzate"
  description: "GroupDocs.Search for Java offre una ricerca testuale avanzata su più di 70 formati di file. L'indicizzazione accelera le ricerche e migliora l'efficienza nella gestione dei documenti."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale potente"
      content: "Trova testo in formati di documenti popolari come PDF, file Word, presentazioni e fogli di calcolo. Supporta diversi metodi di ricerca, inclusi ricerca fuzzy, omofoni e caratteri jolly."

    # feature loop
    - title: "Indicizzazione ottimizzata per prestazioni migliori"
      content: "Crea e riutilizza indici di ricerca per migliorare la velocità e l'efficienza delle ricerche, specialmente in grandi collezioni di documenti."

    # feature loop
    - title: "Supporto per ricerca multilingue"
      content: "Cerca all'interno di documenti scritti in oltre 80 lingue. Rileva diverse impostazioni della tastiera e variazioni di parole per una maggiore precisione."

    # feature loop
    - title: "Opzioni di ricerca personalizzabili"
      content: "Affina i risultati di ricerca con filtri, espressioni regolari e altre impostazioni di ricerca avanzate."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtra i documenti prima della ricerca"
      content: |
        Scopri come affinare le ricerche utilizzando filtri.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Imposta un indice che esclude determinati formati di file.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Specifica il percorso di archiviazione dei documenti.
          index.add("c:/MyDocuments");

          // Recupera i risultati della ricerca.
          SearchResult result = index.search("Lorem", options);
          
          // Elabora e utilizza i risultati della ricerca.
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Copia"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica risultato"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzionalità di GroupDocs.Search gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Download di Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Caratteristiche chiave"
    exclude: "filters"
    description: "Esegui ricerche testuali precise ed efficienti."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca in documenti aziendali"
    exclude: "DOCX"
    description: "GroupDocs.Search supporta oltre 70 formati di file, rendendo semplice la ricerca in documenti d’ufficio ampiamente utilizzati."
    items: 
        # format loop 1
        - name: "Filtri di ricerca per DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Filtri di ricerca per PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Filtri di ricerca per PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Filtri di ricerca per TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Filtri di ricerca per XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---