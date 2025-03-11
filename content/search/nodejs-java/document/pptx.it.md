
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: it
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Trova testo in PPTX con GroupDocs.Search in Node.js"
head_description: "Utilizza GroupDocs.Search for Node.js via Java con JavaScript per cercare testo in modo efficiente in vari formati di documento."

############################# Header ############################
title: "Soluzione intelligente per la ricerca di documenti" 
description: "Localizza testo in diversi formati di documento con GroupDocs.Search for Node.js via Java. Crea query di ricerca avanzate all'interno delle tue applicazioni Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prova Gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introduzione a GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) è una libreria ad alte prestazioni per la ricerca di testo completo e l'indicizzazione dei documenti. Supporta oltre 70 tipi di file, inclusi PDF, Word, PowerPoint, Excel, immagini e archivi ZIP, garantendo risultati rapidi e accurati.

############################# Steps ############################
steps:
    enable: true
    title: "Esegui ricerca in file PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ti consente di eseguire ricerche in file PPTX, affinando i risultati nelle applicazioni Node.js via Java.
      
      1. Definisci una cartella di archiviazione per l'indice di ricerca.
      2. Seleziona una cartella con file PPTX.
      3. Imposta parametri di ricerca aggiuntivi.
      4. Esegui la ricerca e analizza i risultati.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copia"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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

        // Specifica la directory per il salvataggio dell'indice di ricerca
        const index = new searchLib.Index("c:/MyIndex");

        // Scegli la cartella contenente i documenti da cercare
        index.add("c:/MyDocuments");

        // Abilita la ricerca per omofoni per parole che suonano simili
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Esegui una query di ricerca complessa
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacità avanzate di ricerca e indicizzazione"
  description: "GroupDocs.Search for Node.js via Java offre potenti strumenti di ricerca e indicizzazione del testo in oltre 70 formati di documento, facilitando la ricerca e l'organizzazione delle informazioni."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Vantaggi chiave di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca del testo completa"
      content: "Trova testo in più tipi di documento, inclusi PDF, documenti Word, presentazioni PowerPoint e fogli di calcolo. Usa corrispondenze esatte, ricerca fuzzy e caratteri jolly per risultati più raffinati."

    # feature loop
    - title: "Indicizzazione efficiente per grandi quantità di dati"
      content: "Accelera le ricerche creando indici strutturati, facilitando il recupero di informazioni da grandi collezioni di documenti."

    # feature loop
    - title: "Supporta oltre 80 lingue"
      content: "Cerca all'interno di documenti in diverse lingue, con riconoscimento automatico di vari formati di parole e layout di tastiera."

    # feature loop
    - title: "Impostazioni di ricerca personalizzate"
      content: "Regola le opzioni di ricerca come la distinzione tra maiuscole e minuscole, filtri di data e esclusioni di parole per ottenere risultati precisi."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizzo della ricerca per documenti PPTX"
      content: |
        Questo esempio mostra come utilizzare query di ricerca all'interno di documenti PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Imposta la directory per l'indicizzazione della ricerca
          const index = new searchLib.Index("c:/MyIndex");
              
          // Fornisci il percorso del file per il salvataggio del documento
          index.add("c:/MyDocuments");

          // Inserisci la password per i file protetti
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", '123456');

          // Abilita la ricerca fuzzy per il rilevamento di parole simili
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Estrai i risultati della ricerca
          const result = index.search("Loarem", options);
          
          // Elabora e verifica i risultati
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pptx"
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
  description: "Prova le funzionalità di GroupDocs.Search gratuitamente oppure richiedi una licenza"
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
    title: "Esplora le caratteristiche chiave"
    exclude: "document"
    description: "Scopri le funzionalità di ricerca ad alta velocità progettate per migliorare l'efficienza e l'accuratezza."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca in una varietà di documenti"
    exclude: "PPTX"
    description: "GroupDocs.Search funziona con oltre 70 formati di file, inclusi documenti d'ufficio, garantendo ricerche rapide e accurate con supporto per l'indicizzazione."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Formato Documento Portabile Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---