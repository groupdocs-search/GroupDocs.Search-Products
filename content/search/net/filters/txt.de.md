
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: de
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "In TXT-Dokumenten suchen mit .NET"
head_description: "GroupDocs.Search for .NET verbessert C#-Anwendungen mit effizienter Textsuche über verschiedene Geschäftsdateiformate."

############################# Header ############################
title: "Text in Geschäftsdokumenten suchen" 
description: "GroupDocs.Search for .NET ermöglicht leistungsstarke und flexible Textsuche in Ihren Dokumenten. Integrieren Sie die Suchfunktionalität nahtlos in .NET-Anwendungen."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Was ist GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) ist eine leistungsstarke Bibliothek für effiziente Textsuche und Dokumentenindizierung. Sie unterstützt über 70 Dateiformate, einschließlich branchenüblicher Dokumente wie PDF, Word, Excel und PowerPoint. Verbessern Sie die Suchleistung mit schnellen und genauen Ergebnissen.

############################# Steps ############################
steps:
    enable: true
    title: "So suchen Sie in TXT-Daten"
    content: |
      [GroupDocs.Search](/search/net/) ermöglicht effiziente Textsuchen in TXT-Dokumenten, was es ideal für .NET-Anwendungen macht.
      
      1. Richten Sie einen Ordner zum Speichern des Suchindex ein.
      2. Wählen Sie den Ordner mit Ihren Dateien aus.
      3. Konfigurieren Sie die Sucheinstellungen, um nur TXT-Dokumente zu verarbeiten.
      4. Führen Sie die Suche aus und rufen Sie die Ergebnisse ab.
   
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
        // Pfad zum Speichern des wiederverwendbaren Suchindex
        Index index = new Index("c:/MyIndex");

        // Ordner mit Dokumenten
        index.Add("c:/MyDocuments");

        // Nur innerhalb spezifischer Dateiformate suchen
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".txt");

        // Suchergebnisse abrufen
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Suchfunktionen"
  description: "GroupDocs.Search for .NET ermöglicht aufwendige Textsuchen in mehr als 70 Dateiformaten. Die Indizierung verbessert die Sucheffizienz und hilft, Dokumenteninhalte effektiv zu verwalten."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Hauptfunktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Erweiterte Textsuche"
      content: "Extrahieren Sie relevante Texte aus beliebten Geschäftsdokumenten, einschließlich PDFs, Word-Dokumenten, Präsentationen und Tabellenkalkulationen. Unterstützt mehrere Suchtechniken wie unscharfe Suche, Homophon-Erkennung und Platzhalter."

    # feature loop
    - title: "Optimierte Indizierung für schnellere Suchen"
      content: "Erstellen und wiederverwenden Sie Suchindizes, um die Suchgeschwindigkeit zu erhöhen. Die Indizierung optimiert die Leistung bei der Suche in großen Dokumentensammlungen."

    # feature loop
    - title: "Unterstützung mehrerer Sprachen"
      content: "Führen Sie Suchen in Dokumenten in über 80 Sprachen durch. Erkennt verschiedene Tastaturlayouts und Wortvariationen zur Verbesserung der Genauigkeit."

    # feature loop
    - title: "Flexible Sucheinstellungen"
      content: "Verfeinern Sie Suchergebnisse mit anpassbaren Optionen, einschließlich Filter, reguläre Ausdrücke und Einstellungen zur Groß-/Kleinschreibung."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dokumente filtern, die verarbeitet werden sollen"
      content: |
        Erfahren Sie, wie Sie Dokumentensuchen mit Filtern eingrenzen können.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Richten Sie einen Index ein, der bestimmte Dateiformate ausschließt.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Geben Sie das Dokumentenverzeichnis an.
          index.Add("c:/MyDocuments");

          // Rufen Sie die Suchergebnisse ab.
          SearchResult result = index.Search("Lorem");
          
          // Verarbeiten und nutzen Sie die Suchergebnisse.
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
            link: "/examples/search/formats/searchfilters.txt"
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
    title: "Hauptfunktionen"
    exclude: "filters"
    description: "Führen Sie präzise und effiziente Datensuchen durch."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Daten in Ihren Geschäftsdokumenten finden"
    exclude: "TXT"
    description: "GroupDocs.Search unterstützt über 70 Dateiformate und ermöglicht eine effiziente Verarbeitung und Suche von beliebten Büro-Dokumenten."
    items: 
        # format loop 1
        - name: "Suchfilter für DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Suchfilter für PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Suchfilter für PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Suchfilter für TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Suchfilter für XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---