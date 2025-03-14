
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: de
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Durchsuchen Sie TXT-Dokumente in .NET mit GroupDocs.Search"
head_description: "Verwenden Sie GroupDocs.Search for .NET, um effiziente Textsuche in verschiedenen Dokumentformaten mit C# durchzuführen."

############################# Header ############################
title: "Erweiterte Textsuche in Dokumenten" 
description: "GroupDocs.Search for .NET erleichtert die Textsuche in gängigen Dokumentformaten und ermöglicht Ihnen, leistungsstarke Suchabfragen in Ihren .NET-Anwendungen zu erstellen."
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
       [GroupDocs.Search for .NET](/search/net/) ist eine leistungsstarke Bibliothek, die für die Volltextsuche und Indizierung in Dokumenten entwickelt wurde. Sie unterstützt über 70 Dateiformate, einschließlich PDF, Word, PowerPoint, Excel, Bilder und ZIP-Dateien, und gewährleistet schnelle und präzise Suchergebnisse.

############################# Steps ############################
steps:
    enable: true
    title: "So führen Sie eine Textsuche in TXT-Dokumenten durch"
    content: |
      [GroupDocs.Search](/search/net/) ermöglicht erweiterte Suchoperationen in TXT-Dokumenten und liefert verfeinerte Suchergebnisse in .NET-Anwendungen.
      
      1. Richten Sie den Ordner ein, um den Suchindex zu speichern.
      2. Wählen Sie den Ordner mit den TXT-Dateien.
      3. Konfigurieren Sie zusätzliche Suchoptionen.
      4. Führen Sie die Suche aus und überprüfen Sie die Ergebnisse.
   
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
        // Definieren Sie den Pfad für den Suchindex
        Index index = new Index("c:/MyIndex");

        // Wählen Sie den Ordner mit den zu durchsuchenden Dokumenten aus
        index.Add("c:/MyDocuments");

        // Aktivieren Sie die Homophon-Suche, um ähnliche klingende Wörter zu finden
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Führen Sie eine komplexe Suchabfrage aus
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Such- und Indizierungsfunktionen"
  description: "GroupDocs.Search for .NET verbessert die Textsuche und Indizierung über mehr als 70 Dateiformate hinweg und bietet effiziente Werkzeuge zur Auffindung und Verwaltung von Informationen."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Search"
  features:
    # feature loop
    - title: "Leistungsstarke Textsuche"
      content: "Durchsuchen Sie Text über mehrere Dokumenttypen hinweg, einschließlich PDFs, Word-Dokumenten, PowerPoint-Präsentationen und Tabellenkalkulationen. Nutzen Sie Funktionen wie exakte Übereinstimmungen, unscharfe Suche und Platzhalter, um Ihre Ergebnisse zu verfeinern."

    # feature loop
    - title: "Schnelles Indizieren großer Datensätze"
      content: "Erstellen und verwalten Sie Suchindizes für eine schnelle Abrufung von Informationen. Das Indizieren optimiert die Suche über umfangreiche Dokumentensammlungen."

    # feature loop
    - title: "Mehrsprachige Unterstützung"
      content: "Führen Sie Suchen in über 80 Sprachen durch, mit Unterstützung für verschiedene Tastaturlayouts und Wortvariationen zur Verbesserung der Genauigkeit."

    # feature loop
    - title: "Anpassbare Sucheinstellungen"
      content: "Passen Sie Suchparameter mit Optionen wie Groß-/Kleinschreibung, Datumsbereichsfiltern und Wortausschlüssen für bessere Ergebnisse an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ausführen erweiterter Suchabfragen"
      content: |
        Dieses Beispiel zeigt, wie Suchabfragen für TXT-Dokumente angewendet werden.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Definieren Sie den Ordner für den Suchindex
          Index index = new Index("c:/MyIndex");
              
          // Geben Sie den Pfad zu den Dokumentdateien an
          index.Add("c:/MyDocuments");

          // Geben Sie ein Passwort für geschützte Dokumente an
          index.Dictionaries.DocumentPasswords.Add("protected.txt", "123456");

          // Aktivieren Sie die unscharfe Suche, um ähnliche Wörter zu finden
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Rufen Sie die Suchergebnisse ab
          SearchResult result = index.Search("Loarem", options);
          
          // Verarbeiten Sie die Suchausgabe
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "Schlüsselfeatures erkunden"
    exclude: "document"
    description: "Nutzen Sie die erweiterten und leistungsstarken Suchfunktionen."
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
    title: "Durchsuchen Sie Ihre Geschäftsdokumente"
    exclude: "TXT"
    description: "GroupDocs.Search unterstützt mehr als 70 Dateiformate, einschließlich Büro-Dokumenten, und ermöglicht schnelle und effiziente Suchen mit Indizierungsfunktionen."
    items: 
        # format loop 1
        - name: "Suche im DOCX-Dokument"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Suche im PDF-Dokument"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Suche im PPTX-Dokument"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Suche im TXT-Dokument"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Suche im XLSX-Dokument"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---