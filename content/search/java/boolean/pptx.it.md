
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: it
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Ricerca booleana in PPTX con Java"
head_description: "Con GroupDocs.Search for Java, gli sviluppatori possono eseguire ricerche nei documenti utilizzando operatori booleani come AND, OR e NOT."

############################# Header ############################
title: "Ricerca di testo booleano" 
description: "Utilizza GroupDocs.Search for Java per creare query di ricerca avanzate booleane (AND, OR, NOT) nei tuoi progetti Java."
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
    title: "Informazioni su GroupDocs.Search"
    link: "/search/java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) è una libreria versatile progettata per la ricerca testuale e l'indicizzazione dei dati nei documenti. Supporta oltre 70 tipi di file, inclusi PDF, Word, Excel, PowerPoint, immagini e archivi ZIP, consentendo ricerche efficienti attraverso grandi collezioni di dati.

############################# Steps ############################
steps:
    enable: true
    title: "Come eseguire ricerche booleano in documenti PPTX"
    content: |
      [GroupDocs.Search](/search/java/) consente ricerche testuali all'interno di documenti PPTX. Con il supporto per condizioni boolean, puoi migliorare l'accuratezza delle ricerche nelle applicazioni Java.
      
      1. Specificare la cartella per memorizzare l'indice di ricerca.
      2. Seleziona la cartella contenente documenti PPTX.
      3. Esegui la query di ricerca e ottieni i risultati.
      4. Elabora i risultati ottenuti.
   
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
        // Imposta il percorso per la cartella dell'indice
        Index index = new Index("c:/MyIndex");

        // Fornisci il percorso della cartella contenente i documenti per la ricerca
        index.add("c:/MyDocuments");

        // Esegui una ricerca con una query complessa
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Strumenti potenti per la ricerca e l'indicizzazione dei documenti"
  description: "GroupDocs.Search for Java semplifica le ricerche testuali e l'indicizzazione dei dati per oltre 70 formati. I suoi strumenti avanzati ti permettono di trovare e gestire contenuti con efficienza."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale completa"
      content: "Cerca attraverso più formati come PDF, documenti Word, presentazioni, fogli di calcolo e altro. Usa opzioni come corrispondenza esatta, ricerca fuzzy e query con caratteri jolly per affinare i risultati."

    # feature loop
    - title: "Indicizzazione dei dati efficiente"
      content: "Crea e mantieni indici per ricerche documentali più rapide. Questa funzione organizza i dati in modo efficiente, facilitando la gestione di grandi collezioni di documenti."

    # feature loop
    - title: "Supporto multilingue"
      content: "Cerca in documenti scritti in oltre 80 lingue. Migliora l'accuratezza sfruttando le forme morfologiche delle parole e le diverse disposizioni della tastiera."

    # feature loop
    - title: "Personalizzazione flessibile delle ricerche"
      content: "Regola le impostazioni di ricerca con funzionalità come distinzione tra maiuscole e minuscole, filtri per intervallo di date e esclusioni per affinare i tuoi risultati."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzo di query di ricerca booleane complesse"
      content: |
        Questo esempio dimostra come eseguire ricerche boolean in file PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Imposta la cartella per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Fornisci il percorso ai documenti da cercare
          index.add("c:/MyDocuments");

          // Costruisci la query utilizzando logica booleana
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Recupera i risultati della ricerca
          SearchResult result = index.search(booleanQuery);
          
          // Elabora i risultati recuperati
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
            link: "/examples/search/formats/searchboolean.pptx"
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
    title: "Caratteristiche chiave a colpo d'occhio"
    exclude: "boolean"
    description: "Sblocca potenti e efficienti capacità di ricerca"
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca formati di documenti popolari"
    exclude: "PPTX"
    description: "GroupDocs.Search supporta oltre 70 formati di file, consentendoti di personalizzare le regole di ricerca e di utilizzare l'indicizzazione per ottimizzare le prestazioni."
    items: 
        # format loop 1
        - name: "Ricerca booleana in DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca booleana in PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca booleana in PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca booleana in TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca booleana in XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---