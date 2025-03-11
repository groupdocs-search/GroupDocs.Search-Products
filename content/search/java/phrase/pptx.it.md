
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: it
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cerca frasi in PPTX utilizzando Java"
head_description: "GroupDocs.Search for Java potenzia le applicazioni Java con avanzate capacità di ricerca di frasi nei contenuti dei documenti."

############################# Header ############################
title: "Trova frasi nei documenti" 
description: "Individua rapidamente frasi specifiche con GroupDocs.Search for Java. Aggiungi funzionalità di ricerca potenti alle tue applicazioni Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Caratteristiche di GroupDocs.Search"
    link: "/search/java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) è una libreria robusta per indicizzare e cercare testo all'interno dei documenti. Supporta oltre 70 formati di file, tra cui PDF, documenti Word, fogli di calcolo Excel, immagini e file ZIP, garantendo risultati di ricerca rapidi e precisi.

############################# Steps ############################
steps:
    enable: true
    title: "Come trovare frasi in documenti PPTX"
    content: |
      [GroupDocs.Search](/search/java/) semplifica la ricerca di frasi in documenti PPTX. Utilizza varie opzioni per affinare i risultati di ricerca nelle applicazioni Java.
      
      1. Crea una directory per l'indice di ricerca.
      2. Specifica la cartella con i file PPTX.
      3. Regola i parametri di ricerca.
      4. Recupera e analizza i risultati della ricerca.
   
    code:
      platform: "java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        // Definisci il percorso dell'indice di ricerca
        Index index = new Index("c:/MyIndex");

        // Specifica la cartella contenente i documenti
        index.add("c:/MyDocuments");

        // Imposta le preferenze di ricerca
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Esegui la query di ricerca
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Esplora il motore di ricerca documentale Java"
  description: "GroupDocs.Search for Java consente ricerche di frasi in oltre 70 formati di file. Trova e organizza facilmente i dati utilizzando funzionalità di ricerca avanzate."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Capacità principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca per frase"
      content: "Individua frasi esatte in documenti aziendali, come PDF, file Word, presentazioni e fogli di calcolo. Utilizza caratteri jolly e altre opzioni quando la frase esatta non è nota."

    # feature loop
    - title: "Indicizzazione dei dati ottimizzata"
      content: "Accelera le ricerche nei documenti creando e riutilizzando indici di ricerca. L'indicizzazione organizza i dati in modo efficiente per ricerche più veloci e accurate."

    # feature loop
    - title: "Compatibilità multi-lingua"
      content: "Cerca documenti in oltre 80 lingue. Supporta diverse impostazioni di tastiera e analisi morfologica per migliorare la precisione della ricerca."

    # feature loop
    - title: "Opzioni di ricerca avanzate"
      content: "Personalizza le ricerche con sensibilità al maiuscolo, ricerca fuzzy, corrispondenza di omofoni, filtraggio dei documenti e altre funzionalità potenti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzo di metodi di ricerca avanzati"
      content: |
        Scopri come costruire query per cercare in PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Definisci la directory per l'indice di ricerca
          Index index = new Index("c:/MyIndex");
              
          // Imposta il percorso per i documenti target
          index.add("c:/MyDocuments");

          // Crea una query di ricerca per una frase specifica
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Recupera i risultati della ricerca
          SearchResult result = index.search(query);
          
          // Elabora e utilizza i risultati recuperati
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pptx"
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
  description: "Prova le funzionalità di GroupDocs.Search gratuitamente oppure richiedi una licenza"
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
    title: "Capacità di ricerca avanzate"
    exclude: "phrase"
    description: "Utilizza funzionalità di ricerca all'avanguardia per migliorare la precisione e le prestazioni."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca frasi in documenti aziendali"
    exclude: "PPTX"
    description: "GroupDocs.Search abilita ricerche di frasi in oltre 70 formati di documenti. Sfrutta opzioni avanzate e indicizzazione per ricerche efficienti."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Formato Documento Portabile Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---