
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: de
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Suche in TXT-Dokumenten mit Node.js"
head_description: "GroupDocs.Search for Node.js via Java fügt JavaScript-Anwendungen schnelle und präzise Textsuchfunktionen hinzu und unterstützt mehrere Dokumentformate."

############################# Header ############################
title: "Text in Geschäftsdokumenten finden" 
description: "GroupDocs.Search for Node.js via Java bietet leistungsstarke und flexible Suchfunktionen für Dokumente. Integrieren Sie die Textsuche in Node.js-Anwendungen."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) ist eine robuste Such- und Indexierungsbibliothek, die ein schnelles Abrufen von Text in Dokumenten ermöglicht. Sie unterstützt über 70 Dateiformate, darunter PDFs, Word, Excel und PowerPoint, um präzise und effiziente Suchen zu gewährleisten.

############################# Steps ############################
steps:
    enable: true
    title: "Wie man in TXT-Dokumenten eine Suche durchführt"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) macht das Suchen von Text in TXT-Dokumenten einfach und effizient für Node.js via Java-Anwendungen.
      
      1. Erstellen Sie ein Verzeichnis zum Speichern des Suchindex.
      2. Wählen Sie den Ordner aus, der die Dokumente enthält.
      3. Stellen Sie die Suchoptionen so ein, dass nur TXT-Dateien einbezogen werden.
      4. Starten Sie die Suche und rufen Sie die Ergebnisse ab.
   
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

        // Definieren Sie ein Verzeichnis zum Speichern des Suchindex
        const index = new searchLib.Index("c:/MyIndex");

        // Geben Sie den Ordner mit durchsuchbaren Dokumenten an
        index.add("c:/MyDocuments");

        // Suchen Sie nur in bestimmten Dateiformaten
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // Rufen Sie die Suchergebnisse ab und verarbeiten Sie sie
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Suchfunktionen"
  description: "GroupDocs.Search for Node.js via Java verbessert die Effizienz der Dokumentensuche durch die Indizierung von über 70 Dateiformaten. Optimieren Sie das Abrufen von Inhalten mit fortschrittlichen Suchtechniken."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Search"
  features:
    # feature loop
    - title: "Umfassende Textsuche"
      content: "Extrahieren und lokalisieren Sie Text in gängigen Dokumentformaten, wie PDFs, Word-Dokumenten, Tabellenkalkulationen und Präsentationen. Unterstützt unscharfe Suchen, Homophone und Wildcard-Abfragen."

    # feature loop
    - title: "Optimierte Indizierung für Leistung"
      content: "Beschleunigen Sie Suchen durch Erstellung wiederverwendbarer Indizes. Erhöht Geschwindigkeit und Effizienz beim Arbeiten mit großen Dokumentensammlungen."

    # feature loop
    - title: "Mehrsprachige Unterstützung"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen. Erkennt Tastaturlayouts und Wortvariationen für bessere Genauigkeit."

    # feature loop
    - title: "Anpassbare Suchoptionen"
      content: "Feinabstimmung der Suchergebnisse mit Filtern, regulären Ausdrücken, Groß-/Kleinschreibung und anderen flexiblen Einstellungen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Durchsuchbare Dokumente filtern"
      content: |
        Erfahren Sie, wie Sie Dokumentensuchen mit Filtern verfeinern.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Konfigurieren Sie einen Index, um unerwünschte Dateiformate auszuschließen
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Geben Sie das Verzeichnis mit Dokumenten an
          index.add("c:/MyDocuments");

          // Verarbeiten Sie die Suchausgaben für eine weitere Verwendung
          const result = index.Search("Lorem", options);
          
          // Verarbeiten Sie die Suchausgaben für eine weitere Verwendung
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Hauptfunktionen"
    exclude: "filters"
    description: "Führen Sie schnelle und präzise Textsuchen in Dokumenten durch."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Suche in verschiedenen Dokumentformaten"
    exclude: "TXT"
    description: "GroupDocs.Search unterstützt über 70 Dateitypen, die eine effiziente Textsuche in verschiedenen Office- und Geschäftsdokumenten ermöglichen."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Microsoft Word Open XML Dokument"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "PowerPoint Open XML Präsentation"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Microsoft Excel Open XML Tabelle"
  

---