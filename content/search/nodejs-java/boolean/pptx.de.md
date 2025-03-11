
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: de
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Boolesche PPTX-Suche über Node.js"
head_description: "Nutzen Sie die GroupDocs.Search for Node.js via Java-API, um erweiterte Suchen im Dokumenteninhalt mit booleschen Operatoren wie AND, OR und NOT durchzuführen, maßgeschneidert für JavaScript-Entwickler."

############################# Header ############################
title: "Durchführen von booleschen Logiksuchen" 
description: "Mit GroupDocs.Search for Node.js via Java können Sie erweiterte Suchanfragen unter Verwendung von booleschen Operatoren (AND, OR, NOT) nahtlos in Ihrer Node.js-Umgebung erstellen."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Jetzt herunterladen"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) ist ein leistungsstarkes Tool zum Suchen und Indizieren von Texten in Dokumenten. Es unterstützt über 70 Formate wie PDF, Word, Excel, PowerPoint, Bilder und ZIP-Dateien, was die Verarbeitung großer Informationsmengen effizient gestaltet.

############################# Steps ############################
steps:
    enable: true
    title: "So suchen Sie in PPTX-Dokumenten mit booleschen Operatoren"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ermöglicht Ihnen eine effektive Suche nach Inhalten in PPTX-Dateien. Mit boolescher Logik können Sie Ihre Suchanfragen in Node.js via Java-Anwendungen verfeinern, um die Genauigkeit zu verbessern.
      
      1. Richten Sie den Ordner ein, um den Suchindex zu speichern.
      2. Wählen Sie den Ordner mit PPTX-Dateien für die Suche aus.
      3. Führen Sie die Suchanfrage aus und rufen Sie die Ergebnisse ab.
      4. Verarbeiten und analysieren Sie die Suchergebnisse.
   
    code:
      platform: "nodejs-java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "Klicken zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Legen Sie den Speicherort für den Indexordner fest
        const index = new searchLib.Index("c:/MyIndex");

        // Geben Sie den Ordner mit den zu durchsuchenden Dokumenten an
        index.add("c:/MyDocuments");

        // Führen Sie eine Suchanfrage mit erweiterter Logik aus
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Leistungsstarke Werkzeuge für die Dokumentensuche und -indizierung"
  description: "GroupDocs.Search for Node.js via Java optimiert die Textsuche und Indizierung für über 70 Dateitypen, sodass Sie Informationen schneller und präziser finden und verwalten können."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Hauptfunktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Erweiterte Textsuche"
      content: "Schnelles Finden von Texten in verschiedenen Formaten wie PDFs, Word-Dokumenten, Präsentationen und Tabellenkalkulationen. Nutzen Sie Funktionen wie genaue Übereinstimmungen, Platzhalter-Suchen und unscharfe Suche für präzise Ergebnisse."

    # feature loop
    - title: "Effiziente Datenindizierung"
      content: "Erstellen und verwalten Sie Indizes, um die Suche in großen Dokumentensammlungen zu beschleunigen. Die Indizierung gewährleistet schnellen und strukturierten Zugriff auf Ihre Daten."

    # feature loop
    - title: "Mehrsprachige Unterstützung"
      content: "Suchen Sie in Dokumenten, die in über 80 Sprachen verfasst sind. Morphologische Unterstützung und Kompatibilität mit verschiedenen Tastaturlayouts verbessern die Suchergebnisse in unterschiedlichen Sprachen."

    # feature loop
    - title: "Flexible Sucheinstellungen"
      content: "Passen Sie Ihre Suche an, indem Sie Groß- und Kleinschreibung aktivieren, Datumsfilter anwenden oder bestimmte Wörter und Daten bei der Indizierung überspringen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Beispiel für eine erweiterte boolesche Suche"
      content: |
        Dieses Beispiel zeigt, wie man auf Booleschen basierenden Abfragen zur Suche nach Inhalten in PPTX-Dokumenten erstellt.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definieren Sie den Ordner für den Suchindex
          const index = new searchLib.Index("c:/MyIndex");
              
          // Geben Sie den Speicherort der zu durchsuchenden Dokumente an
          index.add("c:/MyDocuments");

          // Erstellen Sie eine Abfrage mit booleschen Operatoren
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Rufen Sie die Suchergebnisse ab
          const result = index.search(booleanQuery);
          
          // Verarbeiten und verwenden Sie die Suchergebnisse
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Kopieren"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pptx"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit zum Starten?"
  description: "Testen Sie die Funktionen von GroupDocs.Search kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "NPM Download"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Wichtige Funktionen von GroupDocs.Search"
    exclude: "boolean"
    description: "Entfesseln Sie erweiterte, effiziente und anpassbare Suchfunktionen."
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
    title: "Suche in gängigen Dokumentenformaten"
    exclude: "PPTX"
    description: "GroupDocs.Search unterstützt über 70 Dateiformate und bietet flexible Suchregeln sowie eine effiziente Indizierung, um Zeit und Aufwand zu sparen."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Microsoft Word Open XML Dokument"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "PowerPoint Open XML Präsentation"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Microsoft Excel Open XML Tabelle"
  

---