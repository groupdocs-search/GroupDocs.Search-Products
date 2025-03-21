
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: de
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Suchanfragen in TXT mit Node.js"
head_description: "GroupDocs.Search for Node.js via Java fügt leistungsstarke Suchfunktionalitäten für Phrasen zu JavaScript-Anwendungen hinzu, um die Dokumentensuche effizienter zu gestalten."

############################# Header ############################
title: "Phrasen in Dokumenten finden" 
description: "Mit GroupDocs.Search for Node.js via Java gezielt spezifische Phrasen schnell lokalisieren. Integrieren Sie schnelle und präzise Suchfunktionen in Ihre Node.js-Anwendungen."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Herunterladen"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search-Funktionen"
    link: "/search/nodejs-java/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) ist eine leistungsstarke Bibliothek für das Indizieren und Durchsuchen von Texten in Dokumenten. Sie unterstützt über 70 Dateiformate, einschließlich PDF, Word-Dokumente, Excel-Tabellen, Bilder und ZIP-Archive, um genaue und schnelle Suchergebnisse zu gewährleisten.

############################# Steps ############################
steps:
    enable: true
    title: "So finden Sie Phrasen in TXT-Dokumenten"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) erleichtert die Phrasensuche in TXT-Dokumenten. Wenden Sie verschiedene Suchoptionen an, um die Ergebnisse in Node.js via Java-Anwendungen zu verfeinern.
      
      1. Richten Sie einen Ordner für den Suchindex ein.
      2. Definieren Sie den Ordner, der TXT-Dateien enthält.
      3. Konfigurieren Sie die Suchparameter.
      4. Holen Sie sich die Suchergebnisse und verarbeiten Sie diese.
   
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

        // Geben Sie den Speicherort für den Suchindex an
        const index = new searchLib.Index("c:/MyIndex");

        // Legen Sie den Ordner mit den Dokumenten fest
        index.add("c:/MyDocuments");

        // Konfigurieren Sie die Suchparameter
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Führen Sie die Suchabfrage aus
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Entdecken Sie die Dokumentensuchmaschine von Node.js"
  description: "GroupDocs.Search for Node.js via Java ermöglicht Phrasensuchen über mehr als 70 Dateiformate, wodurch das Finden und Organisieren von Daten mit fortschrittlichen Suchfunktionen vereinfacht wird."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Wesentliche Funktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Phrasensuche"
      content: "Finden Sie exakte Phrasen in Geschäftsdokumenten wie PDFs, Word-Dateien, Präsentationen und Tabellen. Nutzen Sie Platzhalter und flexible Suchoptionen, wenn die vollständige Phrase unbekannt ist."

    # feature loop
    - title: "Optimierte Datenindizierung"
      content: "Steigern Sie die Suchleistung durch die Erstellung wiederverwendbarer Indizes. Strukturierte Indizierung beschleunigt die Dokumentensuche und verbessert die Genauigkeit."

    # feature loop
    - title: "Mehrsprachige Kompatibilität"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen mit Unterstützung für verschiedene Tastaturlayouts und morphologische Wortvariationen, um präzise Ergebnisse zu erzielen."

    # feature loop
    - title: "Erweiterte Suchoptionen"
      content: "Passen Sie Suchvorgänge mit Groß-/Kleinschreibung, unscharfer Übereinstimmung, Homophon-Erkennung, Dokumentenfilterung und anderen leistungsstarken Funktionen an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verwendung fortgeschrittener Suchtechniken"
      content: |
        Erfahren Sie, wie Sie Abfragen zum Suchen in TXT erstellen.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definieren Sie das Verzeichnis des Suchindexes
          const index = new searchLib.Index("c:/MyIndex");
              
          // Legen Sie den Pfad zu den Ziel-Dokumenten fest
          index.add("c:/MyDocuments");

          // Erstellen Sie eine Abfrage für die gewünschte Phrase
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Holen Sie sich die Suchergebnisse
          const result = index.search(query);
          
          // Verarbeiten und nutzen Sie die Ergebnisse
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
            link: "/examples/search/formats/searchphrase.txt"
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
    title: "Erweiterte Suchfunktionen"
    exclude: "phrase"
    description: "Nutzen Sie leistungsstarke Suchfunktionen für schnellere und genauere Ergebnisse."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Phrasen in Geschäftsdokumenten suchen"
    exclude: "TXT"
    description: "GroupDocs.Search unterstützt die Phrasensuche in über 70 Dokumentformaten. Nutzen Sie erweiterte Optionen und Indizierung, um den Suchprozess zu optimieren."
    items: 
        # format loop 1
        - name: "Phrase Suche in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Phrase Suche in PDF"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Phrase Suche in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Phrase Suche in TXT"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Phrase Suche in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---