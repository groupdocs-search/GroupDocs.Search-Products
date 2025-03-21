
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: it
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Ricerca booleana XLSX tramite Node.js"
head_description: "Utilizza l'API GroupDocs.Search for Node.js via Java per eseguire ricerche avanzate nel contenuto dei documenti con operatori booleani come AND, OR e NOT, progettata per sviluppatori JavaScript."

############################# Header ############################
title: "Esegui ricerche logiche booleane" 
description: "Con GroupDocs.Search for Node.js via Java, puoi creare query di ricerca avanzate utilizzando operatori booleani (AND, OR, NOT) senza soluzione di continuità all'interno del tuo ambiente Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Scarica ora"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Che cos'è GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Scopri di più"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) è uno strumento robusto per cercare e indicizzare testi all'interno di documenti. Supporta oltre 70 formati come PDF, Word, Excel, PowerPoint, immagini e file ZIP, facilitando il trattamento di grandi quantità di informazioni in modo efficiente.

############################# Steps ############################
steps:
    enable: true
    title: "Come cercare in documenti XLSX usando operatori booleani"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) consente di cercare contenuti in file XLSX in modo efficace. Con la logica booleana, puoi affinare le tue query di ricerca nelle applicazioni Node.js via Java per una maggiore precisione.
      
      1. Configura la cartella per memorizzare l'indice di ricerca.
      2. Seleziona la cartella contenente i file XLSX per la ricerca.
      3. Esegui la query di ricerca e recupera i risultati.
      4. Elabora e analizza i risultati della ricerca.
   
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

        // Imposta la posizione della cartella dell'indice
        const index = new searchLib.Index("c:/MyIndex");

        // Specifica la cartella contenente i documenti da cercare
        index.add("c:/MyDocuments");

        // Esegui una query di ricerca con logica avanzata
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Strumenti potenti per la ricerca e l'indicizzazione dei documenti"
  description: "GroupDocs.Search for Node.js via Java semplifica la ricerca di testo e l'indicizzazione per oltre 70 tipi di file, aiutandoti a trovare e gestire le informazioni più rapidamente e con precisione."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Caratteristiche principali di GroupDocs.Search"
  features:
    # feature loop
    - title: "Ricerca testuale avanzata"
      content: "Trova rapidamente il testo all'interno di vari formati come PDF, documenti Word, presentazioni e fogli di calcolo. Usa funzionalità come corrispondenze esatte, ricerche wildcard e ricerca fuzzy per risultati precisi."

    # feature loop
    - title: "Indicizzazione dei dati efficiente"
      content: "Crea e gestisci indici per accelerare le ricerche in grandi raccolte di documenti. L'indicizzazione garantisce un accesso rapido e strutturato ai tuoi dati."

    # feature loop
    - title: "Supporto multilingue"
      content: "Cerca in documenti scritti in oltre 80 lingue. Il supporto morfologico e la compatibilità con i layout di tastiera migliorano i risultati delle ricerche in diverse lingue."

    # feature loop
    - title: "Impostazioni di ricerca flessibili"
      content: "Personalizza la tua ricerca abilitando la sensibilità alle maiuscole, applicando filtri temporali o escludendo parole e dati specifici durante l'indicizzazione."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Esempio di ricerca booleana avanzata"
      content: |
        Questo esempio dimostra come creare query basate su Boolean per cercare contenuti in documenti XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definisci la cartella per l'indice di ricerca
          const index = new searchLib.Index("c:/MyIndex");
              
          // Fornisci la posizione dei documenti da cercare
          index.add("c:/MyDocuments");

          // Costruisci una query utilizzando operatori booleani
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Recupera i risultati della ricerca
          const result = index.search(booleanQuery);
          
          // Elabora e utilizza i risultati della ricerca
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
            link: "/examples/search/formats/searchboolean.xlsx"
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
    title: "Capacità chiave di GroupDocs.Search"
    exclude: "boolean"
    description: "Sblocca funzionalità di ricerca avanzate, efficienti e personalizzabili."
    items: 
          
        # operation loop 1
        - name: "Ricerca per condizione"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Trova informazioni nei documenti utilizzando condizioni booleane"

        # operation loop 2
        - name: "Ricerca case-sensitive"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Migliora l'accuratezza della ricerca considerando la sensibilità al maiuscolo"

        # operation loop 3
        - name: "Indicizzazione documentale"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Indicizza i documenti una volta e riutilizza l'indice per più ricerche"

        # operation loop 4
        - name: "Filtri di ricerca"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Utilizza i filtri per restringere i dati trattati"

        # operation loop 5
        - name: "Frase esatta"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Cerca una specifica frase o espressione"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cerca formati di documenti popolari"
    exclude: "XLSX"
    description: "GroupDocs.Search supporta oltre 70 formati di file, fornendo regole di ricerca flessibili e indicizzazione efficiente per risparmiare tempo e sforzo."
    items: 
        # format loop 1
        - name: "Ricerca booleana in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Ricerca booleana in PDF"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Formato di Documento Portatile Adobe"
          
        # format loop 3
        - name: "Ricerca booleana in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Presentazione PowerPoint Open XML"

        # format loop 4
        - name: "Ricerca booleana in TXT"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Documento di Testo"
          
        # format loop 5
        - name: "Ricerca booleana in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Foglio di calcolo Microsoft Excel Open XML"
  

---