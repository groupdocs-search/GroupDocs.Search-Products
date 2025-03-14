
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: it
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Cerca in documenti TXT usando Node.js"
head_description: "GroupDocs.Search for Node.js via Java offre funzionalità di ricerca testuale veloce e precisa per applicazioni in JavaScript, supportando più formati di documento."

############################# Header ############################
title: "Trova testi in documenti aziendali" 
description: "GroupDocs.Search for Node.js via Java fornisce una funzionalità di ricerca potente e flessibile per i documenti. Integra in modo fluido la ricerca testuale nelle applicazioni Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica gratuitamente"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Cos'è GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) è una libreria robusta per la ricerca e l'indicizzazione che abilita il recupero veloce di testo nei documenti. Supporta oltre 70 formati di file, compresi PDF, Word, Excel e PowerPoint, garantendo ricerche precise ed efficienti.

############################# Steps ############################
steps:
    enable: true
    title: "Come eseguire una ricerca in documenti TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) semplifica e rende efficiente la ricerca di testo in documenti TXT per applicazioni Node.js via Java.
      
      1. Crea una directory per memorizzare l'indice di ricerca.
      2. Scegli la cartella che contiene i documenti.
      3. Imposta le opzioni di ricerca per includere solo file TXT.
      4. Esegui la ricerca e recupera i risultati.
   
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

        // Definire una directory per memorizzare l'indice di ricerca
        const index = new searchLib.Index("c:/MyIndex");

        // Specificare la cartella contenente i documenti ricercabili
        index.add("c:/MyDocuments");

        // Limitare la ricerca a formati di file specifici
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // Recuperare e processare i risultati della ricerca
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacità di ricerca avanzate"
  description: "GroupDocs.Search for Node.js via Java migliora l'efficienza della ricerca documentale indicizzando oltre 70 formati di file. Ottimizza il recupero dei contenuti con tecniche di ricerca avanzata."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale completa"
      content: "Estrai e localizza testo in formati documentali popolari, come PDF, file Word, fogli di calcolo e presentazioni. Supporta ricerca fuzzy, omofoni e query wildcard."

    # feature loop
    - title: "Indicizzazione ottimizzata per le prestazioni"
      content: "Accelera le ricerche creando indici riutilizzabili. Migliora la velocità e l'efficienza lavorando con grandi collezioni di documenti."

    # feature loop
    - title: "Supporto multi-lingua"
      content: "Cerca attraverso documenti in oltre 80 lingue. Riconosce layout di tastiera e variazioni di parole per una maggiore precisione."

    # feature loop
    - title: "Opzioni di ricerca personalizzabili"
      content: "Affina i risultati di ricerca con filtri, espressioni regolari, sensibilità al maiuscolo e altre impostazioni flessibili."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtra documenti ricercabili"
      content: |
        Scopri come affinare le ricerche di documenti utilizzando i filtri.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Configura un indice per escludere formati di file indesiderati
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Specifica la directory contenente i documenti
          index.add("c:/MyDocuments");

          // Elabora l'output della ricerca per ulteriori utilizzi
          const result = index.Search("Lorem", options);
          
          // Elabora l'output della ricerca per ulteriori utilizzi
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Funzionalità chiave"
    exclude: "filters"
    description: "Esegui ricerche testuali rapide e precise tra i documenti."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca in vari formati di documento"
    exclude: "TXT"
    description: "GroupDocs.Search supporta oltre 70 tipi di file, consentendo ricerche testuali efficienti in diversi documenti aziendali e d'ufficio."
    items: 
        # format loop 1
        - name: "Filtri di ricerca per DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Filtri di ricerca per PDF"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Filtri di ricerca per PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Filtri di ricerca per TXT"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Filtri di ricerca per XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---