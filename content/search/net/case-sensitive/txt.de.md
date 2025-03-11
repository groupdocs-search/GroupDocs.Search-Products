
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: de
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Groß- und Kleinschreibungssensible Suche in TXT mit .NET"
head_description: "Die GroupDocs.Search for .NET API ermöglicht es C# Entwicklern, groß- und kleinschreibungssensible Suchen in verschiedenen Dokumenten durchzuführen."

############################# Header ############################
title: "Groß- und Kleinschreibungssensible Suche" 
description: "GroupDocs.Search for .NET ermöglicht die Erstellung von fortgeschrittenen, groß- und kleinschreibungssensiblen Suchanfragen innerhalb Ihrer .NET Anwendungen."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos Herunterladen"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Erfahren Sie mehr"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) ist eine leistungsstarke Bibliothek für die Textsuche und -indizierung in Dokumenten. Sie unterstützt über 70 Dateiformate, einschließlich PDF, Word, PowerPoint, Excel, Bilder und ZIP-Dateien, und gewährleistet eine effiziente Handhabung großer Datenmengen.

############################# Steps ############################
steps:
    enable: true
    title: "So führen Sie eine groß- und kleinschreibungssensible Suche in TXT Dokumenten durch"
    content: |
      [GroupDocs.Search](/search/net/) vereinfacht die groß- und kleinschreibungssensible Suche in TXT Dokumenten. Nutzen Sie es, um die Ergebnisse in .NET Anwendungen zu verfeinern.
      
      1. Definieren Sie den Ordner zur Speicherung des Suchindexes.
      2. Wählen Sie den Ordner mit TXT Dateien aus.
      3. Führen Sie die Suche aus und erhalten Sie die Ergebnisse.
      4. Verarbeiten Sie die Ergebnisse.
   
    code:
      platform: "net"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "Klicken zum Kopieren"
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
        // Legt den Pfad zum Indexordner fest
        Index index = new Index("c:/MyIndex");

        // Geben Sie den Ordner an, der die zu durchsuchenden Dokumente enthält
        index.Add("c:/MyDocuments");

        // Aktivieren Sie die groß- und kleinschreibungssensitive Suche in den Optionen
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Führen Sie die Suche aus
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fortgeschrittene Funktionen für die Dokumentensuche und -indizierung"
  description: "Die GroupDocs.Search for .NET Bibliothek vereinfacht die Textsuche und Indizierung über 70+ Dateiformate. Finden und verwalten Sie Informationen mit leistungsstarken Suchwerkzeugen."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Hauptfunktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Erweiterte Textsuche"
      content: "Durchsuchen Sie Text in verschiedenen Dateiformaten, darunter PDFs, Word-Dokumente, Tabellenkalkulationen und Präsentationen. Nutzen Sie Optionen wie exakte Übereinstimmungen, unscharfe Suche und Platzhalter für präzise Ergebnisse."

    # feature loop
    - title: "Indizierung großer Datensätze"
      content: "Erstellen und pflegen Sie Indizes für schnellere Suchen. Organisierte Indizierung vereinfacht das Durchsuchen umfangreicher Dokumentensammlungen."

    # feature loop
    - title: "Mehrsprachige Unterstützung"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen, mit Unterstützung für verschiedene Tastaturlayouts und Wortformen für genauere Ergebnisse."

    # feature loop
    - title: "Anpassbare Suchoptionen"
      content: "Passen Sie die Suchparameter mit Groß-/Kleinschreibungssensitivität, Datumsbereichsfiltern und der Möglichkeit, spezifische Wörter oder Daten während der Indizierung auszuschließen, an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verwendung groß- und kleinschreibungssensibler Suchanfragen"
      content: |
        Dieses Beispiel zeigt, wie man groß- und kleinschreibungssensible Suchanfragen zur Suche in TXT Dokumenten verwendet.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Legen Sie den Ordner für den Suchindex fest
          Index index = new Index("c:/MyIndex");
              
          // Geben Sie den Pfad zu den zu durchsuchenden Dokumenten an
          index.Add("c:/MyDocuments");

          // Erstellen Sie eine Suchanfrage
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Aktivieren Sie die Optionen für die groß- und kleinschreibungssensible Suche
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Suchen Sie nach Text in den Dokumenten
          SearchResult result = index.Search(wordQuery, options);
          
          // Verarbeiten Sie die Suchergebnisse
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Kopieren"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
  title: "Bereit zum Starten?"
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
    title: "Entdecken Sie die Hauptfunktionen"
    exclude: "case-sensitive"
    description: "Erforschen Sie fortschrittliche und effiziente Suchfunktionen."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Beliebte Dokumentenformate durchsuchen"
    exclude: "TXT"
    description: "GroupDocs.Search unterstützt über 70 Dateiformate. Passen Sie die Suchregeln an und nutzen Sie die Indizierung, um Zeit und Aufwand zu sparen."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Microsoft Word Open XML Dokument"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "PowerPoint Open XML Präsentation"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML Tabelle"
  

---