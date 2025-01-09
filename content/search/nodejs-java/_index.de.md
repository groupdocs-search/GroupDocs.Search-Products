---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
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
head_title: "Node.js Textsuche & Indizierungsbibliothek für Dokumente, PDF, Office & Web"
head_description: "Fortgeschrittene Textsuchlösung für Node.js-Anwendungen, um Daten aus Dokumenten zu suchen, zu indizieren & zu sammeln: PDF, Word, Excel, Präsentationen, E-Mail & Web-Dateiformate."

############################# Header ############################
title: "Dokumente mit der Node.js API durchsuchen & indizieren"
description: "Verbessern Sie Node.js-Anwendungen, indem Sie Textsuche in allen gängigen Dokumentformaten implementieren."
words:
  for: "für"

actions:
  main: "Kostenloser NPM Download"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Lizenzierung"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Beginnen Sie Ihre Reise noch heute!"
  description: "Entdecken Sie die Möglichkeiten von GroupDocs.Search kostenlos oder sichern Sie sich eine Lizenz, um das volle Potenzial auszuschöpfen."

release:
  title: "Version {0} veröffentlicht"
  notes: "Sehen Sie sich an, was neu ist"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Führen Sie eine Textsuche in einem Ordner mit JavaScript durch"
  more: "Weitere Beispiele"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Erstellen Sie ein Index für Ihre Dokumente
    const index = new searchLib.Index('c:/MyIndex');

    // Fügen Sie Dokumente zum Index hinzu, um eine effiziente Suche zu ermöglichen
    index.add('c:/MyDocuments');
    
    // Suchen Sie nach bestimmten Wörtern oder Phrasen, wie zum Beispiel
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Übersicht"
  description: "Node.js JavaScript-Bibliothek für die Textsuche"
  features:
    # feature loop
    - title: "Node.js Indizierungs- und Suchoperationen"
      content: "Die Indizierung in GroupDocs.Search for Node.js via Java sammelt, speichert und analysiert Daten für präzise und effiziente Suchoperationen. Diese Indizes werden häufig zur Durchführung von Suchen verwendet."

    # feature loop
    - title: "Mehrere Indizes zusammenführen, um die Sucheffizienz zu verbessern"
      content: "GroupDocs.Search for Node.js via Java API ermöglicht das Zusammenführen mehrerer Indizes zu einem. Häufige Änderungen erstellen mehrere Delta-Indizes, die die Suchleistung verlangsamen können. Unsere Lösung führt diese Delta-Indizes in einen gemeinsamen Index zusammen, der alle Informationen aus den zusammengeführten Delta-Indizes enthält, und verbessert dadurch erheblich die Sucheffizienz, während die Delta-Indizes unverändert bleiben. Verschiedene Funktionen können konfiguriert werden, um diesen Prozess zu optimieren."

    # feature loop
    - title: "Erkennen von Suchanfragen aus verschiedenen Tastaturlayouts"
      content: "GroupDocs.Search for Node.js via Java erkennt Suchanfragen, die nicht mit dem Tastaturlayout übereinstimmen. Derzeit werden 88 Sprachen und 164 verschiedene Tastaturlayouts unterstützt."

    # feature loop
    - title: "Suchen mit morphologischen Wortformen"
      content: "Mit GroupDocs.Search for Node.js via Java können Sie nach verschiedenen Wortformen suchen, wie Singular und Plural Nomen oder alle Formen eines Verbs. Englisch und nicht-englische Sprachen können an spezifische Wortformen angepasst werden."

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
    GroupDocs.Search for Node.js via Java ermöglicht die Verarbeitung einer Vielzahl von Dateiformaten. [Erforschen Sie die vollständige Liste](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
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
  title: "GroupDocs.Search for Node.js via Java Merkmale"
  description: "Steuern Sie die Inhalte von Geschäftsdokumenten mit unserer fortschrittlichen Suchmaschine, die beliebte Dateiformate wie PDF, DOCX, XLSX, PPTX und mehr unterstützt."

  items:
    # feature loop
    - icon: "document_info"
      title: "Flexible Parameter"
      content: "Datumsspanne und Groß-/Kleinschreibung als Suchparameter verwenden"

    # feature loop
    - icon: "detect"
      title: "Rechtschreibprüfung der Suche"
      content: "Verwenden Sie Suchphrasen mit Rechtschreibprüfung und Platzhaltern und überspringen Sie spezielle Zeichen in Abfragen."

    # feature loop
    - icon: "collect"
      title: "Ergebnisse filtern"
      content: "Richten Sie Dokumentfilterung in den Suchergebnissen ein"

    # feature loop
    - icon: "get"
      title: "Importieren & Exportieren"
      content: "Importieren oder verwenden Sie eine Liste, um während der Indizierung Zeichen zu ändern, und exportieren Sie in eine Datei."

    # feature loop
    - icon: "remove"
      title: "Unnötige Daten überspringen"
      content: "Wählen Sie selektiv das Indizieren bestimmter Dateien und überspringen Sie bestimmte Wörter, um schneller zu indizieren."

    # feature loop
    - icon: "style"
      title: "URL-Verarbeitung"
      content: "Extrahieren Sie HTML-formatierten Text in eine Datei und generieren Sie eine URL, um Suchergebnisse in HTML zu navigieren."

    # feature loop
    - icon: "detect"
      title: "Schnelle Suche"
      content: "Teilen Sie Suchen in kleinere Teile auf, um große Indizes schnell zu durchsuchen."

    # feature loop
    - icon: "manipulate"
      title: "Stream-Verarbeitung"
      content: "Indizieren Sie Dokumente aus Streams und Datenstrukturen."

    # feature loop
    - icon: "compare"
      title: "Umgang mit Schreibfehlern"
      content: "Ermöglichen Sie die genaue Anzahl der Vorkommen jedes gefundenen Wortes, um alternative Wortvorschläge im Falle von Schreibfehlern zu bieten."

    # feature loop
    - icon: "unreadable_characters"
      title: "Archivunterstützung"
      content: "Indizieren Sie gezippte Archive innerhalb anderer ZIP-Archive und rufen Sie eine Liste der indizierten Dateien in einem Archiv ab."

    # feature loop
    - icon: "hidden_print"
      title: "Platzersparnis"
      content: "Speichern Sie Platz mit kompaktem Indizieren und indizieren Sie passwortgeschützte Dokumente."

    # feature loop
    - icon: "style"
      title: "Benutzerdefinierte Synonyme"
      content: "Fügen Sie englische Synonyme zum Standard-Synonymwörterbuch hinzu."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Codebeispiele"
  description: "Erforschen Sie die Funktionen von GroupDocs.Search for Node.js via Java mit Beispielen."
  items:
    # code sample loop
    - title: "Verwenden Sie die 'unscharfe' Suche zur Steigerung der Produktivität"
      content: |
        Genießen Sie die flexible Funktionalität von GroupDocs.Search for Node.js via Java, um die Kontrolle des Inhalts durch ausgeklügelte Suchalgorithmen zu verbessern. [Erfahren Sie mehr](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Wie man das Suchergebnis verarbeitet">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Erstellen Sie ein Index
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Richten Sie Suchoptionen ein
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Suchen Sie nach Dokumenten, die das Wort 'Wasser' oder die Phrase 'Lorem ipsum' enthalten
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Bearbeiten Sie das Suchergebnis
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Reguläre Ausdrücke sind für erweiterte Suchszenarien verfügbar"
      content: |
        GroupDocs.Search for Node.js via Java ermöglicht es uns, reguläre Ausdrücke zu verwenden, um das Suchergebnis zu verfeinern. [Tauchen Sie ein in fortgeschrittene Suchtechniken](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Wie man mit regulären Ausdrücken sucht">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Erstellen Sie ein Index
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Suchen Sie nach der Phrase in Textform

        // Das erste Caret-Zeichen am Anfang zeigt an, dass es sich um eine reguläre Ausdrucks-Suchanfrage handelt
        const query = '^^(.)\\1{1,}';
        // Suchen Sie nach zwei oder mehr identischen Zeichen am Anfang eines Wortes
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
