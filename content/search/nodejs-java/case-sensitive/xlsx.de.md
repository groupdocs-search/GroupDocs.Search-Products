
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: de
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Durchführen von Groß-/Kleinschreibungssuchanfragen in XLSX mit Node.js"
head_description: "Die GroupDocs.Search for Node.js via Java API ermöglicht es JavaScript Entwicklern, groß-/kleinschreibungssensitive Suchen über verschiedene Dokumenttypen hinweg auszuführen."

############################# Header ############################
title: "Groß-/Kleinschreibungssensitive Suche" 
description: "GroupDocs.Search for Node.js via Java ermöglicht es Ihnen, fortschrittliche Funktionen für groß-/kleinschreibungssensitive Suchen in Ihren Node.js-Anwendungen zu implementieren."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos Herunterladen"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) ist eine leistungsstarke Bibliothek zum Suchen und Indizieren von Text in Dokumenten. Sie unterstützt über 70 Formate, einschließlich PDFs, Word, Excel, PowerPoint, Bilder und ZIP-Dateien, was eine effiziente Handhabung großer Datenmengen ermöglicht.

############################# Steps ############################
steps:
    enable: true
    title: "Schritte zur Durchführung groß-/kleinschreibungssensitiver Suchen in XLSX-Dateien"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) erleichtert das Durchführen von groß-/kleinschreibungssensitiven Suchen in XLSX-Dateien und verbessert Ihre Node.js via Java-Workflows.
      
      1. Richten Sie einen Ordner ein, um den Suchindex zu speichern.
      2. Wählen Sie den Ordner mit den XLSX-Dateien aus.
      3. Führen Sie die Suche aus und erhalten Sie die Ergebnisse.
      4. Verarbeiten und verwenden Sie die Ergebnisse.
   
    code:
      platform: "nodejs-java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Suchergebnis"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "Klicken, um zu kopieren"
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

        // Geben Sie den Pfad für den Indexordner an
        const index = new searchLib.Index("c:/MyIndex");

        // Setzen Sie den Ordner, der die zu durchsuchenden Dokumente enthält
        index.add("c:/MyDocuments");

        // Aktivieren Sie die groß-/kleinschreibungssensitive Suche in den Einstellungen
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Führen Sie die Suche aus
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Schlüsselfunktionen für Dokumentensuche und -indizierung"
  description: "Mit GroupDocs.Search for Node.js via Java können Sie Text in über 70 Dateiformaten durchsuchen und indizieren. Greifen Sie mühelos auf Informationen zu und organisieren Sie diese mit fortgeschrittenen Suchwerkzeugen."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Kernfunktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Umfassende Textsuche"
      content: "Finden Sie Text in verschiedenen Dokumenttypen wie PDFs, Word-Dokumenten, Tabellenkalkulationen und Präsentationen. Nutzen Sie Optionen wie exakte Übereinstimmungen, unscharfe Suchen und Platzhalter für präzise Ergebnisse."

    # feature loop
    - title: "Effiziente Datenindizierung"
      content: "Erstellen und verwalten Sie Indizes, um Suchvorgänge zu beschleunigen. Die Indizierung hilft Ihnen, Daten in großen Dokumentensammlungen zu organisieren und schnell zu finden."

    # feature loop
    - title: "Unterstützt mehrere Sprachen"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen mit Unterstützung für verschiedene Tastaturlayouts und Wortvariationen, um genaue Suchergebnisse zu gewährleisten."

    # feature loop
    - title: "Anpassbare Suchoptionen"
      content: "Passen Sie die Sucheinstellungen an, einschließlich Groß-/Kleinschreibung, Datumsfilter und den Ausschluss spezifischer Begriffe oder Daten während der Indizierung."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Beispiel: Implementierung der groß-/kleinschreibungssensitiven Suche"
      content: |
        Dieses Beispiel zeigt, wie man groß-/kleinschreibungssensitive Suchen für XLSX-Dokumente durchführt.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definieren Sie den Ordner für den Suchindex
          const index = new searchLib.Index("c:/MyIndex");
              
          // Geben Sie den Pfad zum Dokumentenordner an
          index.add("c:/MyDocuments");

          // Richten Sie eine Suchanfrage ein
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Aktivieren Sie die Einstellungen für die groß-/kleinschreibungssensitive Suche
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Suchen Sie nach dem Text in Dokumenten
          const result = index.search(wordQuery, options);
          
          // Verarbeiten und bearbeiten Sie die Ergebnisse
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Kopieren"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "Klicken, um zu kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
  title: "Bereit, loszulegen?"
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
    title: "Wichtige Funktionen"
    exclude: "case-sensitive"
    description: "Entdecken Sie fortschrittliche Funktionen für schnelles und präzises Durchsuchen von Dokumenten."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Kompatible Dokumentformate"
    exclude: "XLSX"
    description: "GroupDocs.Search unterstützt über 70 Dokumentformate. Passen Sie Ihre Suchoptionen an und sparen Sie Zeit mit der Indizierung."
    items: 
        # format loop 1
        - name: "Groß- und kleinschreibungssensitive Suche in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Groß- und kleinschreibungssensitive Suche in PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Groß- und kleinschreibungssensitive Suche in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Groß- und kleinschreibungssensitive Suche in TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Groß- und kleinschreibungssensitive Suche in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---