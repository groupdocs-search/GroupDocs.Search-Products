
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: it
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Esegui ricerche sensibili al maiuscolo in PDF con Java"
head_description: "L'API GroupDocs.Search for Java aiuta gli sviluppatori Java a eseguire ricerche sensibili al maiuscolo su più tipi di documenti."

############################# Header ############################
title: "Ricerca Documentale Sensibile al Maiuscolo" 
description: "GroupDocs.Search for Java ti consente di implementare una funzionalità di ricerca sensibile al maiuscolo nei tuoi progetti Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtienilo Gratuitamente"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Scopri di più su GroupDocs.Search"
    link: "/search/java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) è uno strumento versatile per la ricerca e indicizzazione del testo su vari documenti. Supporta oltre 70 formati come PDF, file Word, presentazioni PowerPoint, fogli Excel, immagini e ZIP, consentendoti di gestire in modo efficace ampie raccolte di dati.

############################# Steps ############################
steps:
    enable: true
    title: "Guida alla Ricerca Sensibile al Maiuscolo in File PDF"
    content: |
      Utilizzando [GroupDocs.Search](/search/java/), puoi eseguire ricerche sensibili al maiuscolo in documenti PDF, migliorando i tuoi progetti Java.
      
      1. Imposta la cartella per la memorizzazione dell'indice di ricerca.
      2. Seleziona la cartella contenente i file PDF.
      3. Esegui la ricerca sensibile al maiuscolo e raccogli i risultati.
      4. Elabora e utilizza i risultati della ricerca.
   
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
        // Definire la posizione per l'archiviazione dell'indice
        Index index = new Index("c:/MyIndex");

        // Indirizzare alla cartella contenente i documenti da cercare
        index.add("c:/MyDocuments");

        // Abilitare la modalità sensibile al maiuscolo nelle impostazioni di ricerca
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Eseguire la ricerca
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Strumenti Avanzati di Ricerca e Indicizzazione"
  description: "Con GroupDocs.Search for Java, puoi semplificare la ricerca e l'indicizzazione dei documenti per oltre 70 formati, rendendo più semplice localizzare e organizzare le informazioni."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Punti salienti di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca Testuale Flessibile"
      content: "Cerca attraverso documenti come PDF, file Word, fogli di calcolo e presentazioni con precisione. Usa strumenti come corrispondenza esatta, ricerca fuzzy e supporto per caratteri jolly per affinare i risultati."

    # feature loop
    - title: "Gestione Efficiente degli Indici"
      content: "Organizza e indicizza grandi set di dati per migliorare velocità e prestazioni della ricerca, gestendo collezioni documentali estese."

    # feature loop
    - title: "Supporto per Lingue Globali"
      content: "Esegui ricerche in oltre 80 lingue, adattandoti a diversi layout di tastiera e variazioni linguistiche per una maggiore accuratezza."

    # feature loop
    - title: "Filtri di Ricerca Personalizzabili"
      content: "Regola i criteri di ricerca con opzioni come sensibilità al maiuscolo, filtro per intervallo di date ed esclusione di parole o dati indesiderati durante l'indicizzazione."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Esempio: Query di Ricerca Sensibile al Maiuscolo"
      content: |
        Questo esempio dimostra come implementare ricerche sensibili al maiuscolo per documenti PDF.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Definire la directory per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Specificare la posizione della cartella dei documenti
          index.add("c:/MyDocuments");

          // Impostare una query di ricerca
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Attivare la sensibilità al maiuscolo nelle opzioni di ricerca
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Eseguire la ricerca nei documenti
          SearchResult result = index.search(wordQuery, options);
          
          // Elaborare i risultati ottenuti
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
            link: "/examples/search/formats/searchcase-sensitive.pdf"
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
    title: "Panoramica delle Caratteristiche Chiave"
    exclude: "case-sensitive"
    description: "Scopri le robuste ed efficaci capacità di ricerca offerte da GroupDocs.Search for Java."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formati di File Supportati per la Ricerca"
    exclude: "PDF"
    description: "GroupDocs.Search lavora con oltre 70 formati di documento popolari, offrendo impostazioni di ricerca personalizzabili e un'indicizzazione efficiente."
    items: 
        # format loop 1
        - name: "Ricerca case-sensitive in DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca case-sensitive in PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca case-sensitive in PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca case-sensitive in TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca case-sensitive in XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---