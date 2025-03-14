
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: it
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Cerca frasi in DOCX usando Node.js"
head_description: "GroupDocs.Search for Node.js via Java aggiunge potenti funzionalità di ricerca per frasi a applicazioni JavaScript per una ricerca documentale efficace."

############################# Header ############################
title: "Trova frasi nei documenti" 
description: "Trova rapidamente frasi specifiche con GroupDocs.Search for Node.js via Java. Integra capacità di ricerca veloci e accurate nelle tue applicazioni Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Caratteristiche di GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) è una libreria ad alte prestazioni per indicizzare e cercare testo nei documenti. Supporta oltre 70 formati di file, inclusi PDF, documenti Word, fogli di calcolo Excel, immagini e archivi ZIP, garantendo risultati di ricerca accurati e rapidi.

############################# Steps ############################
steps:
    enable: true
    title: "Come trovare frasi nei documenti DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) rende la ricerca di frasi nei documenti DOCX semplice. Applica diverse opzioni di ricerca per perfezionare i risultati nelle applicazioni Node.js via Java.
      
      1. Imposta una cartella per l'indice di ricerca.
      2. Definisci la cartella contenente i file DOCX.
      3. Configura i parametri di ricerca.
      4. Recupera e elabora i risultati della ricerca.
   
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

        // Specifica il percorso per memorizzare l'indice di ricerca
        const index = new searchLib.Index("c:/MyIndex");

        // Imposta la cartella contenente i documenti
        index.add("c:/MyDocuments");

        // Configura le impostazioni di ricerca
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Esegui la query di ricerca
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Scopri il motore di ricerca documentale Node.js"
  description: "GroupDocs.Search for Node.js via Java abilita ricerche per frasi in oltre 70 formati di file, semplificando la ricerca e l'organizzazione dei dati con funzionalità di ricerca avanzate."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Capacità chiave di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca per frasi"
      content: "Trova frasi esatte in documenti aziendali come PDF, file Word, presentazioni e fogli di calcolo. Usa caratteri jolly e opzioni di ricerca flessibili quando la frase completa è sconosciuta."

    # feature loop
    - title: "Indicizzazione dei dati ottimizzata"
      content: "Migliora le prestazioni di ricerca creando indici riutilizzabili. L'indicizzazione strutturata accelera le ricerche nei documenti e migliora l'accuratezza."

    # feature loop
    - title: "Compatibilità multilingue"
      content: "Cerca documenti in oltre 80 lingue, con supporto per layout da tastiera diversi e variazioni morfologiche delle parole, garantendo risultati precisi."

    # feature loop
    - title: "Opzioni di ricerca avanzate"
      content: "Personalizza le ricerche con sensibilità al maiuscolo, corrispondenza fuzzy, rilevamento di omofoni, filtraggio dei documenti e altre funzionalità potenti."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzare tecniche di ricerca avanzate"
      content: |
        Scopri come costruire query per la ricerca in DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definisci la directory dell'indice di ricerca
          const index = new searchLib.Index("c:/MyIndex");
              
          // Imposta il percorso per i documenti di destinazione
          index.add("c:/MyDocuments");

          // Crea una query per la frase desiderata
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Recupera i risultati della ricerca
          const result = index.search(query);
          
          // Elabora e utilizza i risultati
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
            link: "/examples/search/formats/searchphrase.docx"
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
    title: "Capacità di ricerca avanzate"
    exclude: "phrase"
    description: "Sfrutta potenti funzionalità di ricerca per risultati più rapidi e accurati."
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
    title: "Cerca frasi in documenti aziendali"
    exclude: "DOCX"
    description: "GroupDocs.Search supporta la ricerca per frasi in oltre 70 formati di documenti. Usa opzioni avanzate e indicizzazione per semplificare il processo di ricerca."
    items: 
        # format loop 1
        - name: "Ricerca frase in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca frase in PDF"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca frase in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca frase in TXT"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca frase in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---