
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: it
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Trova testo nei documenti XLSX con GroupDocs.Search per Java"
head_description: "GroupDocs.Search for Java aiuta gli sviluppatori Java a cercare rapidamente testo all'interno di vari formati di documento."

############################# Header ############################
title: "Ricerca intelligente del testo nei documenti" 
description: "Con GroupDocs.Search for Java, puoi cercare e estrarre senza soluzione di continuità testo da più tipi di documenti nelle tue applicazioni Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Richiedi Prova Gratuita"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Cosa fa GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) è una robusta libreria per la ricerca e l'indicizzazione dei documenti che supporta oltre 70 formati di file, inclusi PDF, Word, PowerPoint, Excel, immagini e archivi ZIP. Consente di effettuare ricerche rapide, precise e scalabili su ampie collezioni di documenti.

############################# Steps ############################
steps:
    enable: true
    title: "Esegui ricerche testuali nei file XLSX"
    content: |
      [GroupDocs.Search](/search/java/) facilita la ricerca nei file XLSX utilizzando logiche sofisticate e indicizzazione, migliorando la precisione della ricerca nelle applicazioni Java.
      
      1. Configura una directory per memorizzare l'indice di ricerca.
      2. Scegli una cartella contenente file XLSX.
      3. Definisci opzioni di ricerca aggiuntive.
      4. Esegui la ricerca e analizza i risultati.
   
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
        // Imposta la directory per memorizzare l'indice di ricerca
        Index index = new Index("c:/MyIndex");

        // Specificare la cartella contenente documenti ricercabili
        index.add("c:/MyDocuments");

        // Abilita la ricerca di omofoni per abbinare parole con pronunce simili
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Esegui una query di ricerca avanzata
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacità di ricerca e indicizzazione avanzate"
  description: "GroupDocs.Search for Java semplifica la ricerca e l'indicizzazione di oltre 70 formati di documento, fornendo strumenti efficienti per gestire e recuperare rapidamente informazioni."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Funzionalità principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale completa"
      content: "Trova testo in vari formati di documento come PDF, documenti Word, presentazioni PowerPoint e fogli di calcolo. Utilizza corrispondenze esatte, ricerca fuzzy e operatori jolly per risultati di ricerca affinati."

    # feature loop
    - title: "Indicizzazione ottimizzata per grandi dati"
      content: "Crea indici strutturati per accelerare le ricerche, facilitando la navigazione in repository di documenti estesi in modo efficiente."

    # feature loop
    - title: "Supporto per più lingue"
      content: "Esegui ricerche in oltre 80 lingue con supporto integrato per diversi layout di tastiera e variazioni morfologiche delle parole, migliorando la precisione."

    # feature loop
    - title: "Impostazioni di ricerca flessibili"
      content: "Personalizza le ricerche con opzioni come la sensibilità al maiuscolo e minuscolo, filtraggio basato su date e la possibilità di escludere parole specifiche per risultati precisi."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementazione di query di ricerca avanzate"
      content: |
        Questo esempio illustra come utilizzare query di ricerca per cercare in modo efficiente all'interno dei documenti XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Definisci la directory per l'indicizzazione della ricerca
          Index index = new Index("c:/MyIndex");
              
          // Fornisci il percorso del file per i documenti
          index.add("c:/MyDocuments");

          // Inserisci la password per i documenti crittografati
          index.getDictionaries().getDocumentPasswords().add("protected.xlsx", "123456");

          // Attiva la ricerca fuzzy per rilevare parole simili
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Recupera i risultati della ricerca
          SearchResult result = index.Search("Loarem", options);
          
          // Elabora e analizza i risultati della ricerca
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    title: "Panoramica delle funzionalità chiave"
    exclude: "document"
    description: "Scopri le funzionalità di ricerca testuale ad alte prestazioni progettate per efficienza e precisione."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Trova informazioni nei documenti XLSX con GroupDocs.Search"
    exclude: "XLSX"
    description: "GroupDocs.Search supporta oltre 70 formati, inclusi file di office, consentendo ricerche rapide con funzionalità avanzate di indicizzazione."
    items: 
        # format loop 1
        - name: "Ricerca nel documento DOCX"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca nel documento PDF"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca nel documento PPTX"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca nel documento TXT"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca nel documento XLSX"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---