
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: de
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Durchsuchen von PDF in .NET mit booleschen Operatoren"
head_description: "Die GroupDocs.Search for .NET API ermöglicht es C# Entwicklern, Dokumenteninhalt mithilfe von booleschen Operatoren wie AND, OR und NOT zu durchsuchen."

############################# Header ############################
title: "Textsuche mit boolescher Logik" 
description: "GroupDocs.Search for .NET erleichtert das Erstellen komplexer Suchanfragen mithilfe von booleschen Operatoren (AND, OR, NOT) innerhalb Ihrer .NET Anwendungen."
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
       [GroupDocs.Search for .NET](/search/net/) ist eine umfassende Bibliothek zum Suchen und Indizieren von Text in Dokumenten. Sie unterstützt über 70 Dateiformate, darunter PDF, Word, PowerPoint, Excel, Bilder und ZIP-Dateien, und ermöglicht die effiziente Verarbeitung großer Informationsmengen.

############################# Steps ############################
steps:
    enable: true
    title: "So durchsuchen Sie den Inhalt von PDF Dokumenten mit boolescher Logik"
    content: |
      [GroupDocs.Search](/search/net/) macht das Durchsuchen von PDF Dokumenteninhalten unkompliziert. Es bietet boolesche Suchbedingungen zur Verfeinerung der Ergebnisse in .NET Anwendungen.
      
      1. Geben Sie den Ordner an, in dem der Suchindex gespeichert werden soll.
      2. Wählen Sie den Ordner aus, der PDF Dateien enthält.
      3. Führen Sie die Suche aus und rufen Sie die Ergebnisse ab.
      4. Verarbeiten Sie die Ergebnisse.
   
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
        // Legen Sie den Pfad zum Indexordner fest
        Index index = new Index("c:/MyIndex");

        // Geben Sie den Ordner an, der die zu durchsuchenden Dokumente enthält
        index.Add("c:/MyDocuments");

        // Führen Sie eine Suche mit einer komplexen Abfrage aus
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erkunden Sie erweiterte Funktionen für die Dokumentensuche und -indizierung"
  description: "Die GroupDocs.Search for .NET Bibliothek vereinfacht die Textsuche und indizierung für mehr als 70 Dateiformate. Finden und verwalten Sie Informationen mit fortschrittlichen Suchwerkzeugen."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Search"
  features:
    # feature loop
    - title: "Leistungsstarke Textsuche"
      content: "Durchsuchen Sie Text in verschiedenen Dateitypen, einschließlich PDFs, Word-Dokumenten, PowerPoint-Präsentationen und Tabellenkalkulationen. Verwenden Sie Funktionen wie exakte Übereinstimmungen, unscharfe Suchen und Platzhalter, um die Ergebnisse zu verfeinern."

    # feature loop
    - title: "Indizieren großer Datensätze"
      content: "Erstellen und verwalten Sie Indizes für schnellere Suchen. Indizierung strukturiert und organisiert Daten, damit umfangreiche Dokumentensammlungen leichter durchsucht werden können."

    # feature loop
    - title: "Unterstützt mehrere Sprachen"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen, mit Unterstützung für verschiedene Tastaturlayouts und morphologische Wortformen, um die Suchgenauigkeit zu verbessern."

    # feature loop
    - title: "Anpassbare Suchoptionen"
      content: "Passen Sie die Such Einstellungen mit Funktionen wie Groß- und Kleinschreibung, Datumsbereichsfiltern und der Möglichkeit an, bestimmte Wörter oder Daten während der Indizierung auszuschließen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verwendung von erweiterten booleschen Suchanfragen"
      content: |
        Dieses Beispiel zeigt, wie boolesche Abfragen für die Suche in PDF Dokumenten verwendet werden.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Legen Sie den Ordner für den Suchindex fest
          Index index = new Index("c:/MyIndex");
              
          // Geben Sie den Pfad zu den zu durchsuchenden Dokumenten an
          index.Add("c:/MyDocuments");

          // Erstellen Sie eine Suchanfrage mit boolescher Logik
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Rufen Sie die Suchergebnisse ab
          SearchResult result = index.Search(booleanQuery);
          
          // Verarbeiten Sie die Suchergebnisse
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
            link: "/examples/search/formats/searchboolean.pdf"
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
    title: "Entdecken Sie die Hauptmerkmale"
    exclude: "boolean"
    description: "Erforschen Sie fortschrittliche und effiziente Suchfunktionen."
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
    title: "Durchsuchen Sie beliebte Dokumentenformate"
    exclude: "PDF"
    description: "GroupDocs.Search unterstützt über 70 Dateiformate. Passen Sie die Suchregeln an und nutzen Sie die Indizierung, um Zeit und Aufwand zu sparen."
    items: 
        # format loop 1
        - name: "Boolesche Suche in DOCX"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Boolesche Suche in PDF"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Boolesche Suche in PPTX"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Boolesche Suche in TXT"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Boolesche Suche in XLSX"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---