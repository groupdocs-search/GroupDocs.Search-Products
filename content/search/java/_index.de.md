---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: de
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Dokumentensuche & Indizierungslösung für PDFs, Office-Dateien und Webinhalte"
head_description: "Leistungsstarke Textsuche und Indizierung für Java-Anwendungen. Suchen und organisieren Sie Daten in PDFs, Word, Excel, Präsentationen, E-Mails und Webformaten."

############################# Header ############################
title: "Effiziente Dokumentensuche und Indizierung mit der Java API"
description: "Befähigen Sie Java-Anwendungen mit robusten Textsuchfunktionen in allen gängigen Dokumentformaten."
words:
  for: "für"

actions:
  main: "Laden Sie Maven kostenlos herunter"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Beginnen Sie Ihre Reise noch heute!"
  description: "Entdecken Sie die Möglichkeiten von GroupDocs.Search kostenlos oder sichern Sie sich eine Lizenz, um das volle Potenzial auszuschöpfen."

release:
  title: "Version {0} veröffentlicht"
  notes: "Sehen Sie sich an, was neu ist"
  downloads: "Downloads"

code:
  title: "Text in Dateien mit Java finden"
  more: "Weitere Beispiele"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Erstellen Sie ein Index für Ihre Dokumente
    Index index = new Index("c:/MyIndex");

    // Fügen Sie Dokumente zum Index hinzu, um eine effiziente Suche zu ermöglichen
    index.add("c:/MyDocuments");
    
    // Suchen Sie nach bestimmten Wörtern oder Phrasen, wie zum Beispiel
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Übersicht"
  description: "Entdecken Sie die leistungsstarken Textsuchmöglichkeiten der Java Java-Bibliothek."
  features:
    # feature loop
    - title: "Indizierungs- und Suchoperationen in Java"
      content: "Mit GroupDocs.Search for Java können Sie Daten effizient sammeln, speichern und analysieren, um detaillierte Indizes für schnellere und genauere Suchen zu erstellen."

    # feature loop
    - title: "Optimieren Sie die Suche durch Zusammenführen von Indizes"
      content: "Kombinieren Sie mit GroupDocs.Search for Java mehrere Indizes, um Suchen zu beschleunigen. Reduzieren Sie den Einfluss kleinerer Delta-Indizes, indem Sie diese zu einem einzigen, leistungsfähigen Index zusammenführen."

    # feature loop
    - title: "Unterstützung für mehrsprachige Tastaturlayouts"
      content: "Suchen Sie über verschiedene Sprachen und Tastaturlayouts hinweg mit GroupDocs.Search for Java. Es unterstützt 88 Sprachen und 164 Tastaturkonfigurationen für unvergleichliche Vielseitigkeit."

    # feature loop
    - title: "Morphologische Suchfähigkeiten"
      content: "Finden Sie verschiedene Wortformen wie Singular/Plural Nomen oder Verbvariationen mit GroupDocs.Search for Java. Passen Sie die Suchoptionen für Englisch und andere Sprachen an."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Search for Java ist mit den größten Betriebssystemen und Paketmanagern kompatibel."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    Arbeiten Sie mit einer Vielzahl von Dateiformaten mit GroupDocs.Search for Java. [Die vollständige Liste anzeigen](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Merkmale von GroupDocs.Search for Java"
  description: "Verwalten Sie Dokumenteninhalte effektiv mit fortschrittlichen Suchfähigkeiten, die Formate wie PDF, DOCX, XLSX, PPTX und mehr unterstützen."

  items:
    # feature loop
    - icon: "document_info"
      title: "Anpassbare Suchparameter"
      content: "Verfeinern Sie Suchen mit Datumsbereichen und Groß-/Kleinschreibung."

    # feature loop
    - icon: "detect"
      title: "Erweiterte Rechtschreibprüfung"
      content: "Suchen Sie effizient mit Rechtschreibprüfung, Platzhaltern und ignorierten Sonderzeichen."

    # feature loop
    - icon: "collect"
      title: "Gefilterte Suchergebnisse"
      content: "Bewerben Sie Filter, um sich auf Suchergebnisse basierend auf spezifischen Dokumenttypen oder Kriterien zu konzentrieren."

    # feature loop
    - icon: "get"
      title: "Importieren und Exportieren von Indexdaten"
      content: "Daten zum Indizieren einfach importieren oder Ergebnisse zur weiteren Verwendung in Dateien exportieren."

    # feature loop
    - icon: "remove"
      title: "Nicht benötigte Dateien überspringen"
      content: "Optimieren Sie die Indizierung, indem Sie bestimmte Dateien oder Wörter ausschließen."

    # feature loop
    - icon: "style"
      title: "HTML- und URL-Verarbeitung"
      content: "Extrahieren Sie HTML-Inhalte in Dateien und generieren Sie URLs zur Navigation durch Suchergebnisse."

    # feature loop
    - icon: "detect"
      title: "Schnelle Suche in großen Indizes"
      content: "Beschleunigen Sie Suchoperationen, indem Sie große Indizes in handhabbare Teile teilen."

    # feature loop
    - icon: "manipulate"
      title: "Stream-basiertes Indizieren"
      content: "Indizieren Sie Daten direkt aus Streams oder Datenstrukturen."

    # feature loop
    - icon: "compare"
      title: "Umgang mit fehlerhaften Anfragen"
      content: "Erkennen Sie Rechtschreibfehler und schlagen Sie alternative Wörter für bessere Suchgenauigkeit vor."

    # feature loop
    - icon: "unreadable_characters"
      title: "Umfassende Archivunterstützung"
      content: "Indizieren Sie geschachtelte Archive und rufen Sie detaillierte Listen von Dateien innerhalb von ZIP-Dateien ab."

    # feature loop
    - icon: "hidden_print"
      title: "Platzsparende Indizierung"
      content: "Kompakte Indizes speichern Speicherplatz und verarbeiten passwortgeschützte Dateien."

    # feature loop
    - icon: "style"
      title: "Benutzerdefinierte Synonymunterstützung"
      content: "Erweitern Sie das Synonymwörterbuch, um die Suchgenauigkeit mit maßgeschneiderten Optionen zu verbessern."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Probieren Sie die Funktionen von GroupDocs.Search for Java mit diesen Codebeispielen aus."
  items:
    # code sample loop
    - title: "Auf der Suche nach genauerer Übereinstimmung mit unscharfer Suche"
      content: |
        Erforschen Sie die Flexibilität von GroupDocs.Search for Java zur Verwaltung von Inhalten mit fortschrittlichen unscharfen Suchfähigkeiten. [Erfahren Sie mehr](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Wie man das Suchergebnis verarbeitet">}}
        ```java {style=abap}
        // Erstellen Sie ein Index
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Richten Sie Suchoptionen ein
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Suchen Sie nach Dokumenten, die das Wort 'Wasser' oder die Phrase 'Lorem ipsum' enthalten
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Bearbeiten Sie das Suchergebnis
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Verfeinern Sie die Ergebnisse mit regulären Ausdrücken"
      content: |
        Verwenden Sie reguläre Ausdrücke in GroupDocs.Search for Java für präzise und detaillierte Suchergebnisse. [Entdecken Sie fortgeschrittene Techniken](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Wie man mit regulären Ausdrücken sucht">}}
        ```java {style=abap}   
        // Erstellen Sie ein Index
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Suchen Sie nach der Phrase in Textform

        // Das erste Caret-Zeichen am Anfang zeigt an, dass es sich um eine reguläre Ausdrucks-Suchanfrage handelt
        String query = "^^(.)\\1{1,}";
        // Suchen Sie nach zwei oder mehr identischen Zeichen am Anfang eines Wortes
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
