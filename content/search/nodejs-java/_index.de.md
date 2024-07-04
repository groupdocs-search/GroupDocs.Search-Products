---
############################# Static ############################
layout: "landing"
date: 2024-07-04T14:43:38
draft: false

lang: de
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Textsuch- und Indexierungsbibliothek für Dokumente, PDF, Office und Web"
head_description: "Erweiterte Textsuchlösung für Node.js-Anwendungen zum Suchen, Indizieren und Sammeln von Daten aus Dokumenten: PDF, Word, Excel, Präsentationen, E-Mail- und Webdateiformate."

############################# Header ############################
title: "Suchen und indizieren Sie Dokumente mithilfe der Node.js-API"
description: "Verbessern Sie Node.js-Anwendungen durch die Implementierung der Textsuche in allen gängigen Dokumentformaten."
words:
  for: "für"

actions:
  main: "Kostenloser NPM-Download"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Bereit anzufangen?"
  description: "Testen Sie die Funktionen von GroupDocs.Search kostenlos oder fordern Sie eine Lizenz an"

release:
  title: "Version {0} veröffentlicht"
  notes: "Schau was neu ist"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Suche im Ordner mit JavaScript"
  more: "Mehr Beispiele"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // Index erstellen
    const index = new Index('c:/MyIndex');

    // Dokumente zum Index hinzufügen
    index.add('c:/MyDocuments');
    
    // Suche nach verschiedenen Wörtern wie
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search auf einen Blick"
  description: "Node.js JavaScript-Bibliothek für die Textsuche"
  features:
    # feature loop
    - title: "Node.js Indexierung und Suchvorgänge"
      content: "Durch die Indexierung in GroupDocs.Search for Node.js via Java werden Daten für präzise und effiziente Suchvorgänge gesammelt, gespeichert und analysiert. Diese Indizes werden häufig zur Durchführung von Suchen verwendet."

    # feature loop
    - title: "Führen Sie mehrere Indizes zusammen, um die Sucheffizienz zu verbessern"
      content: "Die GroupDocs.Search for Node.js via Java-API ermöglicht die Zusammenführung mehrerer Indizes zu einem. Durch häufige Änderungen entstehen mehrere Delta-Indizes, die die Suchleistung verlangsamen können. Unsere Lösung führt diese Delta-Indizes in einem gemeinsamen Index zusammen, der alle Informationen aus den zusammengeführten Delta-Indizes enthält, wodurch die Sucheffizienz erheblich verbessert wird, während die Delta-Indizes unverändert bleiben. Zur Feinabstimmung dieses Prozesses können verschiedene Funktionalitäten konfiguriert werden."

    # feature loop
    - title: "Erkennen Sie Suchanfragen aus verschiedenen Tastaturlayouts"
      content: "GroupDocs.Search for Node.js via Java erkennt Suchanfragen, die nicht zum Tastaturlayout passen. Derzeit werden 88 Sprachen und 164 verschiedene Tastaturlayouts unterstützt."

    # feature loop
    - title: "Suche mit morphologischen Wortformen"
      content: "Mit GroupDocs.Search for Node.js via Java können Sie nach verschiedenen Wortformen suchen, beispielsweise nach Substantiven im Singular und Plural oder nach allen Formen eines Verbs. Englische und nicht-englische Sprachen können für bestimmte Wortformen angepasst werden."

############################# Platforms ############################
platforms:
  enable: true
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Search for Node.js via Java unterstützt alle gängigen Betriebssysteme und Paketmanager."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Unterstützte Dateiformate"
  description: |
    GroupDocs.Search for Node.js via Java ermöglicht die Verarbeitung einer Vielzahl von Dateiformaten. [Erkunden Sie die vollständige Liste](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Beliebte Office-Formate
        * **tragbar:** PDF 
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
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Netz:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Andere:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java Funktionen"
  description: "Kontrollieren Sie den Inhalt von Geschäftsdokumenten mit unserer erweiterten Suchmaschine, die gängige Dateiformate wie PDF, DOCX, XLSX, PPTX und mehr unterstützt."

  items:
    # feature loop
    - icon: "document_info"
      title: "Flexible Parameter"
      content: "Verwenden Sie Datumsbereich und Groß-/Kleinschreibung als Suchparameter"

    # feature loop
    - icon: "detect"
      title: "Rechtschreibprüfungssuche"
      content: "Verwenden Sie Suchphrasen mit Rechtschreibprüfung und Platzhaltern und überspringen Sie Sonderzeichen in Abfragen"

    # feature loop
    - icon: "collect"
      title: "Ergebnisfilterung"
      content: "Richten Sie die Dokumentfilterung in den Suchergebnissen ein"

    # feature loop
    - icon: "get"
      title: "Import Export"
      content: "Führen Sie einen Import durch oder verwenden Sie eine Liste, um Zeichen während der Indizierung und des Exports in eine Datei zu ändern"

    # feature loop
    - icon: "remove"
      title: "Überspringen Sie unnötige Daten"
      content: "Überspringen Sie selektiv die Indizierung für bestimmte Dateien und überspringen Sie bestimmte Wörter, um sie schneller zu indizieren"

    # feature loop
    - icon: "style"
      title: "URL-Verarbeitung"
      content: "Extrahieren Sie HTML-formatierten Text in eine Datei und generieren Sie eine URL, um durch Suchergebnisse in HTML zu navigieren"

    # feature loop
    - icon: "detect"
      title: "Schnelle Suche"
      content: "Teilen Sie die Suche in kleinere Abschnitte auf, um große Indizes schnell zu durchsuchen"

    # feature loop
    - icon: "manipulate"
      title: "Stream-Verarbeitung"
      content: "Indizieren Sie Dokumente aus Streams und Datenstrukturen"

    # feature loop
    - icon: "compare"
      title: "Behandeln Sie Rechtschreibfehler"
      content: "Aktivieren Sie die genaue Anzahl der Vorkommen für jedes gefundene Wort, um bei Rechtschreibfehlern alternative Wortvorschläge anzubieten"

    # feature loop
    - icon: "unreadable_characters"
      title: "Archivunterstützung"
      content: "Indizieren Sie gezippte Archive in anderen ZIP-Archiven und rufen Sie die Liste der indizierten Dateien in einem Archiv ab"

    # feature loop
    - icon: "hidden_print"
      title: "Speicherplatz sparen"
      content: "Sparen Sie Platz mit der kompakten Indizierung und Indexierung passwortgeschützter Dokumente"

    # feature loop
    - icon: "style"
      title: "Benutzerdefinierte Synonyme"
      content: "Fügen Sie englische Synonyme zum Standard-Synonymwörterbuch hinzu"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Entdecken Sie die Funktionalitäten von GroupDocs.Search for Node.js via Java anhand von Beispielen"
  items:
    # code sample loop
    - title: "Nutzen Sie die Fuzzy-Suche, um die Produktivität zu steigern"
      content: |
        Genießen Sie die flexible GroupDocs.Search for Node.js via Java-Funktionalität, um die Inhaltskontrolle von Dokumenten durch ausgefeilte Suchalgorithmen zu verbessern. [Weitere Informationen](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="So verarbeiten Sie Suchergebnisse">}}
        ```javascript {style=abap}
        // Erstellen Sie einen Index
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Suchoptionen einrichten
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Suchen Sie nach Dokumenten, die das Wort „Wasser“ oder den Ausdruck „Lorem ipsum“ enthalten.
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // Suchergebnis verarbeiten
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Für erweiterte Suchszenarien stehen reguläre Ausdrücke zur Verfügung"
      content: |
        GroupDocs.Search for Node.js via Java ermöglicht uns die Verwendung regulärer Ausdrücke, um das Suchergebnis einzugrenzen. [Tauchen Sie ein in erweiterte Suchtechniken](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="So suchen Sie mit regulären Ausdrücken">}}
        ```javascript {style=abap}   
        // Erstellen Sie einen Index
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Suchen Sie nach der Phrase in Textform

        // Das erste Caret-Zeichen am Anfang zeigt an, dass es sich um eine Suchabfrage mit regulären Ausdrücken handelt
        var query = "^^(.)\\1{1,}";
        // Suchen Sie nach zwei oder mehr identischen Zeichen am Anfang eines Worts
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
