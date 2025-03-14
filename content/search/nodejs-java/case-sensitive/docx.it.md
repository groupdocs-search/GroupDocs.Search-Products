
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: it
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Esegui ricerche sensibili al maiuscolo in DOCX con Node.js"
head_description: "L'API GroupDocs.Search for Node.js via Java consente agli sviluppatori JavaScript di eseguire ricerche sensibili al maiuscolo su diversi tipi di documento."

############################# Header ############################
title: "Ricerca Sensibile al Maiuscolo" 
description: "GroupDocs.Search for Node.js via Java ti permette di implementare funzionalità avanzate di ricerca sensibile al maiuscolo nelle tue applicazioni Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica Gratuitamente"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) è una potente libreria per cercare e indicizzare testo in documenti. Supporta oltre 70 formati, tra cui PDF, Word, Excel, PowerPoint, immagini e file ZIP, consentendo una gestione efficiente di grandi volumi di dati.

############################# Steps ############################
steps:
    enable: true
    title: "Passaggi per Eseguire Ricerche Sensibili al Maiuscolo nei File DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) rende semplice eseguire ricerche sensibili al maiuscolo nei file DOCX, migliorando i tuoi flussi di lavoro Node.js via Java.
      
      1. Configura una cartella per memorizzare l'indice di ricerca.
      2. Seleziona la cartella contenente i file DOCX.
      3. Esegui la ricerca e ottieni i risultati.
      4. Elabora e utilizza i risultati.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Risultato della ricerca"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "clicca per copiare"
        copy_done: "copiato"
      links:
        #  loop
        - title: "Altri esempi"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Documentazione"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Specifica il percorso per la cartella dell'indice
        const index = new searchLib.Index("c:/MyIndex");

        // Imposta la cartella contenente i documenti da cercare
        index.add("c:/MyDocuments");

        // Abilita la ricerca sensibile al maiuscolo nelle impostazioni
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Esegui la ricerca
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Caratteristiche Principali per la Ricerca e Indicizzazione dei Documenti"
  description: "Con GroupDocs.Search for Node.js via Java, puoi ricercare e indicizzare testo in oltre 70 formati di file. Accedi e organizza le informazioni con facilità utilizzando strumenti di ricerca avanzati."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Caratteristiche Principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca Testuale Completa"
      content: "Trova testo in vari tipi di documento come PDF, file Word, fogli di calcolo e presentazioni. Utilizza opzioni come corrispondenze esatte, ricerche fuzzy e caratteri jolly per risultati accurati."

    # feature loop
    - title: "Indicizzazione Dati Efficiente"
      content: "Crea e gestisci indici per velocizzare le ricerche. L'indicizzazione aiuta a organizzare e localizzare rapidamente i dati in ampie raccolte di documenti."

    # feature loop
    - title: "Supporta Più Lingue"
      content: "Cerca documenti in oltre 80 lingue con supporto per layout di tastiera diversi e variazioni di parole, garantendo risultati di ricerca accurati."

    # feature loop
    - title: "Impostazioni di Ricerca Personalizzabili"
      content: "Regola le impostazioni di ricerca, inclusa la sensibilità al caso, i filtri di data e l'esclusione di termini o dati specifici durante l'indicizzazione."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Esempio: Implementazione della Ricerca Sensibile al Maiuscolo"
      content: |
        Questo esempio dimostra come eseguire ricerche sensibili al maiuscolo per documenti DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definisci la cartella per l'indice di ricerca
          const index = new searchLib.Index("c:/MyIndex");
              
          // Fornisci il percorso della cartella dei documenti
          index.add("c:/MyDocuments");

          // Configura una query di ricerca
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Attiva le impostazioni di ricerca sensibili al maiuscolo
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Cerca il testo nei documenti
          const result = index.search(wordQuery, options);
          
          // Elabora e gestisci i risultati
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Copia"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "clicca per copiare"
          copy_done: "copiato"
        top_links:
          #  loop
          - title: "Scarica risultato"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.docx"
        links:
          #  loop
          - title: "Altri esempi"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Documentazione"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto per iniziare?"
  description: "Prova le funzionalità di GroupDocs.Search gratuitamente o richiedi una licenza"
  items:
    #  loop
    - title: "Download di NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenze"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Funzionalità Chiave"
    exclude: "case-sensitive"
    description: "Esplora caratteristiche avanzate per ricerche documentali veloci e precise."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formati di Documento Compatibili"
    exclude: "DOCX"
    description: "GroupDocs.Search supporta oltre 70 formati di documento. Personalizza le tue opzioni di ricerca e risparmia tempo con l'indicizzazione."
    items: 
        # format loop 1
        - name: "Ricerca case-sensitive in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca case-sensitive in PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca case-sensitive in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca case-sensitive in TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca case-sensitive in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---