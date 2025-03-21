
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: de
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Text in PPTX mit GroupDocs.Search in Node.js finden"
head_description: "Verwenden Sie GroupDocs.Search for Node.js via Java mit JavaScript, um Text effizient in verschiedenen Dokumentformaten zu durchsuchen."

############################# Header ############################
title: "Intelligente Dokumentensuchlösung" 
description: "Lokalisieren Sie Text in verschiedenen Dokumentformaten mit GroupDocs.Search for Node.js via Java. Erstellen Sie erweiterte Suchabfragen innerhalb Ihrer Node.js-Anwendungen."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos ausprobieren"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Einführung in GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) ist eine Hochleistungsbibliothek für Volltextsuche und Dokumentenindizierung. Sie unterstützt über 70 Dateitypen, darunter PDF, Word, PowerPoint, Excel, Bilder und ZIP-Archive, und garantiert schnelle und präzise Ergebnisse.

############################# Steps ############################
steps:
    enable: true
    title: "Durchsuchen von PPTX-Dateien"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ermöglicht es Ihnen, Suchen in PPTX-Dateien durchzuführen und die Ergebnisse in Node.js via Java-Anwendungen zu verfeinern.
      
      1. Definieren Sie einen Speicherordner für den Suchindex.
      2. Wählen Sie einen Ordner mit PPTX-Dateien aus.
      3. Legen Sie zusätzliche Suchparameter fest.
      4. Führen Sie die Suche aus und analysieren Sie die Ergebnisse.
   
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

        // Bestimmen Sie das Verzeichnis für die Speicherung des Suchindexes
        const index = new searchLib.Index("c:/MyIndex");

        // Wählen Sie den Ordner mit den zu durchsuchenden Dokumenten aus
        index.add("c:/MyDocuments");

        // Aktivieren Sie die Homophonesuche für ähnlich klingende Wörter
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Führen Sie eine komplexe Suchanfrage aus
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Such- und Indizierungsfunktionen"
  description: "GroupDocs.Search for Node.js via Java bietet leistungsstarke Textsuche- und Indizierungswerkzeuge mit Unterstützung für über 70 Dokumentformate, um das Finden und Organisieren von Informationen zu erleichtern."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Wesentliche Vorteile von GroupDocs.Search"
  features:
    # feature loop
    - title: "Umfassende Textsuche"
      content: "Text in verschiedenen Dokumenttypen finden, einschließlich PDFs, Word-Dokumenten, PowerPoint-Präsentationen und Tabellenkalkulationen. Verwenden Sie exakte Übereinstimmungen, unscharfe Suche und Platzhalter für verfeinerte Ergebnisse."

    # feature loop
    - title: "Effiziente Indizierung für große Datenmengen"
      content: "Beschleunigen Sie Suchen durch die Erstellung strukturierter Indizes, die das Abrufen von Informationen aus großen Dokumentensammlungen erleichtern."

    # feature loop
    - title: "Unterstützt über 80 Sprachen"
      content: "Durchsuchen Sie Dokumente in verschiedenen Sprachen mit automatischer Erkennung verschiedener Wortformen und Tastaturlayouts."

    # feature loop
    - title: "Anpassbare Sucheinstellungen"
      content: "Passen Sie Suchoptionen wie Groß-/Kleinschreibung, Datumsfilter und Wortausschlüsse an, um präzise Ergebnisse zu erzielen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Suchanfrage für PPTX-Dokumente"
      content: |
        Dieses Beispiel zeigt, wie Suchabfragen innerhalb von PPTX-Dokumenten verwendet werden.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Verzeichnis für die Suchindizierung festlegen
          const index = new searchLib.Index("c:/MyIndex");
              
          // Dateipfad für die Dokumentenspeicherung angeben
          index.add("c:/MyDocuments");

          // Passwort für geschützte Dateien eingeben
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", '123456');

          // Unscharfe Suche für ähnliche Worterkennung aktivieren
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Suchergebnisse extrahieren
          const result = index.search("Loarem", options);
          
          // Ergebnisse verarbeiten und überprüfen
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
            link: "/examples/search/formats/searchdocument.pptx"
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
    title: "Entdecken Sie die wichtigsten Funktionen"
    exclude: "document"
    description: "Entdecken Sie hochgeschwindigkeits Suchfunktionen, die für Effizienz und Genauigkeit ausgelegt sind."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Suchen in verschiedenen Dokumenten"
    exclude: "PPTX"
    description: "GroupDocs.Search arbeitet mit über 70 Dateiformaten, einschließlich Büro-dokumenten, und sorgt für schnelle und präzise Suchen mit Indizierungsunterstützung."
    items: 
        # format loop 1
        - name: "Suche im DOCX-Dokument"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Suche im PDF-Dokument"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Suche im PPTX-Dokument"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Suche im TXT-Dokument"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Suche im XLSX-Dokument"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---