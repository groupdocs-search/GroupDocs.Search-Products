---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: de
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET Dokumentensuch- und Indizierungsbibliothek für PDFs, Office-Dateien und mehr"
head_description: "Leistungsfähige .NET-Lösung für Textsuche und Indizierung in Dokumenten wie PDFs, Word, Excel, Präsentationen, E-Mails und Webformaten."

############################# Header ############################
title: "Fortgeschrittene Dokumentensuche und Indizierung mit der .NET API"
description: "Steigern Sie .NET-Anwendungen mit modernsten Textsuchfähigkeiten über gängige Dokumentformate hinweg."
words:
  for: "für"

actions:
  main: "Laden Sie Nuget kostenlos herunter"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Beginnen Sie Ihre Reise noch heute!"
  description: "Entdecken Sie die Möglichkeiten von GroupDocs.Search kostenlos oder sichern Sie sich eine Lizenz, um das volle Potenzial auszuschöpfen."

release:
  title: "Version {0} veröffentlicht"
  notes: "Sehen Sie sich an, was neu ist"
  downloads: "Downloads"

code:
  title: "Text in Verzeichnissdateien suchen"
  more: "Weitere Beispiele"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Erstellen Sie ein Index für Ihre Dokumente
    Index index = new Index("c:/MyIndex");

    // Fügen Sie Dokumente zum Index hinzu, um eine effiziente Suche zu ermöglichen
    index.Add("c:/MyDocuments");
    
    // Suchen Sie nach bestimmten Wörtern oder Phrasen, wie zum Beispiel
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Übersicht"
  description: "Entdecken Sie die .NET C#-Bibliothek für robuste Textsuche und Indizierung."
  features:
    # feature loop
    - title: ".NET Indizierungs- und Suchfunktionen"
      content: "Indizieren, speichern und verarbeiten Sie Dokumentdaten effizient mit GroupDocs.Search for .NET für hochpräzise und schnelle Suchoperationen."

    # feature loop
    - title: "Indizes kombinieren für bessere Suchgeschwindigkeit"
      content: "GroupDocs.Search for .NET ermöglicht Ihnen, mehrere Indizes zu einem zu kombinieren, um die Leistung zu optimieren. Reduzieren Sie den Einfluss von Delta-Indizes, indem Sie sie in einen umfassenden Index zusammenfassen, um reibungslosere Suchen durchzuführen."

    # feature loop
    - title: "Suchen über verschiedene Tastaturlayouts"
      content: "Verarbeiten Sie Suchanfragen in 88 Sprachen und 164 Tastaturlayouts mühelos mit GroupDocs.Search for .NET's intelligenter Erkennung."

    # feature loop
    - title: "Morphologische Wortsuche"
      content: "GroupDocs.Search for .NET unterstützt Suchanfragen nach Wortvarianten wie Singular/Plural Nomen und verschiedene Verbformen, anpassbar für verschiedene Sprachen."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Search for .NET funktioniert nahtlos auf allen gängigen Betriebssystemen und Paketmanagern."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    Verarbeiten Sie eine umfangreiche Palette von Dateiformaten mit GroupDocs.Search for .NET. [Alle unterstützten Formate anzeigen](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Beliebte Büroformate
        * **Portabel:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Text:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Medienformate
        * **Beliebte Bildformate:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Mehrseitige Bilder:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Video:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Andere
        * **E-Mail:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Sonstige:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Hauptmerkmale von GroupDocs.Search for .NET"
  description: "Optimieren Sie das Dokumentenmanagement mit erweiterten Suchfunktionen in gängigen Formaten wie PDF, DOCX, XLSX, PPTX und mehr."

  items:
    # feature loop
    - icon: "document_info"
      title: "Flexible Suchparameter"
      content: "Verwenden Sie Filter wie Datumsbereiche und Groß-/Kleinschreibung zur Verfeinerung Ihrer Suche."

    # feature loop
    - icon: "detect"
      title: "Intelligente Rechtschreibprüfung"
      content: "Suchen Sie Phrasen mit Rechtschreibkorrektur, Platzhaltern und ignorierten Sonderzeichen."

    # feature loop
    - icon: "collect"
      title: "Gefilterte Suchergebnisse"
      content: "Passen Sie die Suchergebnisse nach Dokumenttyp oder Kriterien an."

    # feature loop
    - icon: "get"
      title: "Indeximport & Export"
      content: "Importieren Sie Daten, ändern Sie Indizierungseinstellungen und exportieren Sie indizierte Ergebnisse."

    # feature loop
    - icon: "remove"
      title: "Irrelevante Daten ausschließen"
      content: "Optimieren Sie die Indizierung, indem Sie bestimmte Dateien oder Wörter überspringen."

    # feature loop
    - icon: "style"
      title: "URL-Extraktion"
      content: "Konvertieren Sie HTML-formatierten Text in Dateien und erstellen Sie Links für Suchergebnisse."

    # feature loop
    - icon: "detect"
      title: "Hochgeschwindigkeits-Suche"
      content: "Teilen Sie große Indizes in kleinere Teile für schnellere Verarbeitung."

    # feature loop
    - icon: "manipulate"
      title: "Vereinfachte Datenverarbeitung"
      content: "Indizieren Sie Dokumente direkt aus Datenströmen und -strukturen."

    # feature loop
    - icon: "compare"
      title: "Erkennung von Schreibfehlern"
      content: "Schlagen Sie alternative Wörter vor und verfolgen Sie Vorkommen zur Verbesserung der Genauigkeit."

    # feature loop
    - icon: "unreadable_characters"
      title: "Archivunterstützung"
      content: "Indizieren Sie geschachtelte ZIP-Archive und rufen Sie Dateidetails innerhalb dieser ab."

    # feature loop
    - icon: "hidden_print"
      title: "Effiziente Indizierung"
      content: "Sparen Sie Speicherplatz mit kompakten Indizes und verarbeiten Sie passwortgeschützte Dokumente."

    # feature loop
    - icon: "style"
      title: "Benutzerdefinierte Synonyme"
      content: "Fügen Sie Synonyme hinzu und verwalten Sie diese für maßgeschneiderte Suchergebnisse."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Entdecken Sie die leistungsstarken Eigenschaften von GroupDocs.Search for .NET mit praktischen Beispielen."
  items:
    # code sample loop
    - title: "Produktivität mit unscharfer Suche steigern"
      content: |
        Nutzen Sie GroupDocs.Search for .NET für flexible und präzise Inhaltskontrolle mittels fortschrittlicher Suchalgorithmen. [Erfahren Sie mehr](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Wie man das Suchergebnis verarbeitet">}}
        ```csharp {style=abap}
        // Erstellen Sie ein Index
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Richten Sie Suchoptionen ein
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Suchen Sie nach Dokumenten, die das Wort 'Wasser' oder die Phrase 'Lorem ipsum' enthalten
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Bearbeiten Sie das Suchergebnis
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Erweiterte Suche mit regulären Ausdrücken"
      content: |
        GroupDocs.Search for .NET unterstützt reguläre Ausdrücke für präzise Suchen. [Erfahren Sie fortgeschrittene Techniken](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Wie man mit regulären Ausdrücken sucht">}}
        ```csharp {style=abap}   
        // Erstellen Sie ein Index
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Suchen Sie nach der Phrase in Textform

        // Das erste Caret-Zeichen am Anfang zeigt an, dass es sich um eine reguläre Ausdrucks-Suchanfrage handelt
        string query = "^^(.)\\1{1,}";
        // Suchen Sie nach zwei oder mehr identischen Zeichen am Anfang eines Wortes
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
