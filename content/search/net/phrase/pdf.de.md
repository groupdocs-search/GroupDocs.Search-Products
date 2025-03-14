
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: de
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Suchphrasen in PDF mit .NET"
head_description: "GroupDocs.Search for .NET verbessert C#-Anwendungen mit leistungsstarken Suchfunktionen für Dokumenteninhalt."

############################# Header ############################
title: "Nach Phrasen in Dokumenten suchen" 
description: "Finden Sie spezifische Phrasen schnell mit GroupDocs.Search for .NET. Integrieren Sie eine effiziente Suchfunktionalität in Ihre .NET-Anwendungen."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Herunterladen"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search-Funktionen"
    link: "/search/net/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) ist eine leistungsstarke Bibliothek zum Indizieren und Durchsuchen von Text in Dokumenten. Sie unterstützt über 70 Dateiformate, darunter PDFs, Word-Dokumente, Excel-Tabellen, Bilder und ZIP-Dateien, und ermöglicht schnelle und präzise Suchergebnisse.

############################# Steps ############################
steps:
    enable: true
    title: "So suchen Sie nach Phrasen in PDF-Dokumenten"
    content: |
      [GroupDocs.Search](/search/net/) vereinfacht die Suche in PDF-Dokumenten. Verwenden Sie verschiedene Optionen, um Suchergebnisse in .NET-Anwendungen zu verfeinern.
      
      1. Richten Sie den Ordner für den Suchindex ein.
      2. Geben Sie den Ordner an, der PDF-Dateien enthält.
      3. Konfigurieren Sie die Sucheinstellungen.
      4. Holen Sie die Suchergebnisse ab und verarbeiten Sie diese.
   
    code:
      platform: "net"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Suchergebnis"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "Klicken, um zu kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Pfad zum Speichern des Suchindex
        Index index = new Index("c:/MyIndex");

        // Ordner mit Dokumenten
        index.Add("c:/MyDocuments");

        // Suchoptionen konfigurieren
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Die Suche ausführen
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Entdecken Sie die Dokumentensuchmaschine von .NET"
  description: "GroupDocs.Search for .NET ermöglicht die Phrasensuche in über 70 Dateiformaten. Lokalisieren und verwalten Sie Daten mit fortschrittlichen Suchfunktionen."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Search"
  features:
    # feature loop
    - title: "Phrasensuche"
      content: "Suchen Sie nach genauen Phrasen in Geschäftsdokumenten, einschließlich PDFs, Word-Dateien, Präsentationen und Tabellenkalkulationen. Verwenden Sie Platzhalter und andere Optionen, wenn die genaue Phrase unbekannt ist."

    # feature loop
    - title: "Effizientes Datenindizieren"
      content: "Erstellen und verwenden Sie Suchindizes, um Dokumentensuchen zu beschleunigen. Indizierung strukturiert Daten effizient, sodass Phrasensuchen schneller erfolgen."

    # feature loop
    - title: "Mehrsprachige Unterstützung"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen. Unterstützt verschiedene Tastaturlayouts und morphologische Wortformen für eine genauere Suche."

    # feature loop
    - title: "Flexible Suchoptionen"
      content: "Passen Sie Suchanfragen mit Funktionen wie Groß-/Kleinschreibung, unscharfer Suche und Homophon-Suche sowie Dokumentfilterung an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verwendung fortgeschrittener Suchtechniken"
      content: |
        Erfahren Sie, wie Sie Abfragen für die Suche in PDF erstellen.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Geben Sie den Ordner für den Suchindex an
          Index index = new Index("c:/MyIndex");
              
          // Legen Sie den Pfad zu den Dokumenten für die Suche fest
          index.Add("c:/MyDocuments");

          // Erstellen Sie eine Abfrage für eine spezifische Phrase
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Holen Sie die Suchergebnisse ab
          SearchResult result = index.Search(query);
          
          // Verarbeiten und nutzen Sie die Ergebnisse
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Kopieren"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "Klicken, um zu kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pdf"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Bereit, loszulegen?"
  description: "Testen Sie die Funktionen von GroupDocs.Search kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Nuget Download"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Erweiterte Funktionen"
    exclude: "phrase"
    description: "Nutzen Sie leistungsstarke und effiziente Suchfunktionen."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Phrasensuche in Geschäftsdokumenten"
    exclude: "PDF"
    description: "GroupDocs.Search unterstützt Suchen in über 70 Dokumentformaten. Nutzen Sie erweiterte Optionen und Indizierung, um Ihren Suchprozess zu optimieren."
    items: 
        # format loop 1
        - name: "Phrase Suche in DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Phrase Suche in PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Phrase Suche in PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Phrase Suche in TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Phrase Suche in XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---