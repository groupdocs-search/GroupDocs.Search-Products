---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java-Textsuche & Indizierung API für Dokumente, PDF, Office und Web"
head_description: "Erweiterte Textsuch-API für Java-Anwendungen zum Suchen, Indexieren und Abrufen von Daten aus Dokumenten: PDF, Word, Excel, Präsentationen, E-Mail und Web-Dateiformate."

############################# Header ############################
title: "Suchen und Indexieren von Dokumenten über die Java-API"
description: "Erstellen Sie Java-Anwendungen, um die Textsuche in allen gängigen Dokumentformaten durchzuführen.."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "/border/groupdocs-search-java.svg"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Überblick"

            # button loop
            - link: "#features"
              text: "Merkmale"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/search"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Überblick ############################
overview:
    enable: true
    content: |
      Mit GroupDocs.Search für Java können Sie Geschäftsanwendungen erstellen, mit denen Ihre Endbenutzer Suchvorgänge wie nie zuvor durchführen können. Unsere Java-API ermöglicht es Benutzern, einfache bis fortgeschrittene Textsuchfunktionen zu betreiben. Erstellen und führen Sie mehrere Indizes zusammen. Verwenden Sie einfache, boolesche, reguläre Ausdrücke (Regex), Fuzzy und andere Arten von Abfragen, um Indizes schnell und intelligent zu durchsuchen. Sie können Ihre benötigten Informationen aus Dateien, Dokumenten, E-Mails und Archiven abrufen, da GroupDocs.Search für Java alle gängigen Dateiformate unterstützt.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Nachfolgend finden Sie eine Übersicht über GroupDocs.Search für Java:

        left:
          enable: true
          icon: "fas fa-search"
          title: "Indizierung"
          content: |
            * Erstellen & verwalten
            * Mehrere Indizes zusammenführen
            * Multi-Threading Async Indizierung
            * Compact Indizierung
            * Archived Files Indizierung
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "Erweiterte Suche & Suchanfragen"
          content: |
            * Ungenaue Suche
            * Synonymsuche
            * E-Mail-Suche
            * Umgang mit homophonen Begriffen
            * Suche nach geschützten Dateien
            * Einfach
            * Wildcard
            * Regulärer Ausdruck (Regex)
            * Facettiert & Boolesch
            * Groß-/Kleinschreibung beachten
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Search für Java unterstützt alle gängigen [Dokumentdateiformate](https://docs.groupdocs.com/search/java/supported-document-formats/) einschließlich: Microsoft Office, Bilder, Diagramme und viele andere.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office-Formate"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Project**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Andere Formate"
              content: |
                * **Portable Document Format**: PDF
                * **OpenDocument**: ODT, OTT, ODS, OTS, ODP
                * **E-Mail**: PST, OST, MSG, EML, EMLX
                * **Webdateiformate**: XML, HTM, HTML, XHTML, MHT, MHTML
                * **Audio**: MP3, WAV
                * **Video**: AVI, MOV, QT, FLV, ASF
                * **Text**: TXT
                * **Rich-Text-Format**: RTF
                * **Markdown-Dokumentationsdatei**: MD
                * **Bilder**: BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **Andere**: TORRENT, ZIP, DCM, DJVU, EPUB, FB2

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Search for Java unterstützt das Folgen Betriebssysteme, Frameworks & Paketmanager:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * Java 7 (1.7) und höher

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Entwicklungsumgebungen"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build-Automatisierungstool"
              content: |
                * Maven

############################# Merkmale ############################
features:
    enable: true
    title: "GroupDocs.Search for Java Merkmale"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Erstellen Sie einen Index auf der Festplatte oder im Arbeitsspeicher mit asynchronem Multithreading"

      # feature loop
      - icon: "fas fa-eye"
        content: "Zeigen Sie den Fortschritt der Indexerstellung und -aktualisierung an"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Überspringen Sie selektiv die Indizierung für bestimmte Dateien und überspringen Sie bestimmte Wörter, um schneller zu indizieren"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Führen Sie den Import durch oder verwenden Sie die Liste, um Zeichen während der Indizierung zu ändern und in eine Datei zu exportieren"

      # feature loop
      - icon: "fas fa-code"
        content: "Index bei Fehlerindizierung neu laden & Benutzer bei widersprüchlichen Einstellungen warnen"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Indexstatusbenachrichtigung bezüglich der zuletzt verarbeiteten Dateien"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Indizieren Sie gezippte Archive in anderen ZIP-Archiven und erhalten Sie eine Liste der indizierten Dateien in einem Archiv"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Sparen Sie Platz durch kompakte Indizierung & passwortgeschützte Indizierung von Dokumenten"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Dokumenttextextraktion aus Index oder Quelldatei"

      # feature loop
      - icon: "fas fa-border-all"
        content: "HTML-formatierte Textextraktion in eine Datei und URL erzeugen, um durch Suchergebnisse in HTML zu navigieren"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Fügen Sie bei der Indizierung jedem Dokument beliebige Zusatzfelder hinzu"

      # feature loop
      - icon: "fas fa-columns"
        content: "Konfigurieren Sie den Ähnlichkeitsgrad für Ungenaue Suche und zeigen Sie die besten Ergebnisse"

      # feature loop
      - icon: "fas fa-print"
        content: "Konfigurieren und führen Sie eine Synonymsuche durch und gehen Sie intelligent mit homophonen Begriffen um"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Verwenden Sie Datumsbereich und Groß-/Kleinschreibung als Suchparameter"

      # feature loop
      - icon: "fas fa-lock"
        content: "Erstellen Sie einen Index zum Suchen und Durchsuchen von E-Mail-Nachrichten über die Aspose.Email-API"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Verwenden Sie Suchphrasen mit Rechtschreibprüfung und Platzhaltern und überspringen Sie Sonderzeichen in Abfragen"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Erstellen Sie einen einzelnen Objektbaum, indem Sie mehrere Abfragen kombinieren"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Unterteilen Sie die Suche in kleinere Blöcke, um schnell riesige Indizes zu durchsuchen"

      # feature loop
      - icon: "fas fa-heading"
        content: "Indizieren Sie Dokumente aus Streams und Datenstrukturen"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Richten Sie die Dokumentenfilterung in den Suchergebnissen ein"

      # feature loop
      - icon: "fas fa-cube"
        content: "Englische Synonyme zum Standard-Synonym-Wörterbuch hinzufügen"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Aktivieren Sie die genaue Anzahl der Vorkommen für jedes gefundene Wort, um bei Rechtschreibfehlern alternative Wortvorschläge anzubieten"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Hinzufügen von Textattributen zu indizierten Dokumenten ohne Neuindizierung"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Perform Indizierung and Searching Operations Based on Characters"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Index-Metadaten von nicht-textuellen Dokumentformaten"

    more_feature:
      # more_feature_loop
      - title: "Indizierung and Search Operation"
        content: |
          Indizierung wird von GroupDocs.Search für Java verwendet, um Daten zu sammeln, zu speichern und für genaue und effiziente Suchvorgänge zu parsen. GroupDocs.Search für Java verwendet solche Indizes häufig zur Durchführung von Suchen.

          * **Index erstellen**: Indexordner erstellen und Dokumente zu diesem Ordner hinzufügen/indizieren.
          * **Index laden**: Laden Sie einen bestehenden Index.
          * **Dokumente zum Index hinzufügen**: Dokumente asynchron zum bestehenden Index hinzufügen.
          * **Index aktualisieren**: Aktualisieren Sie den bestehenden Index, wenn ein Dokument geändert, hinzugefügt oder gelöscht wird. Dadurch bleiben die Suchergebnisse aktuell.
          
          ```java
          // Index erstellen
          Index index = new Index("c:\\MyIndex");
          // Hinzufügen von Dokumenten zum Index
          index.addToIndex("c:\\MyDocuments");
          // Suche nach Wörtern 'affect' or 'effect' in einem Dokument mit 'principal', 'principle', 'principles', or 'principally'
          SearchResults results = index.search("?ffect & princip?(2~4)");
          ```
      # more_feature_loop
      - title: "Führen Sie mehrere Indizes zusammen, um die Sucheffizienz zu verbessern"
        content: "GroupDocs.Search for Java API bietet die Funktion, mehrere Indizes zu einem gemeinsamen Index zusammenzuführen. Für einen Index, der häufig geändert wird, werden mehrere Delta-Indizes erstellt. Dieser Ansatz verlangsamt jedoch die Suchleistung. GroupDocs.Search für Java überwindet diesen Engpass, indem es durch Zusammenführen verschiedener Delta-Indizes einen gemeinsamen Index erstellt. Dieser gemeinsame zusammengeführte Index enthält alle Informationen der zusammengeführten Delta-Indizes. Dieser Ansatz hält die Delta-Indizes unverändert, während die Sucheffizienz bemerkenswert verbessert wird. Sie können verschiedene Funktionen konfigurieren, um diesen Prozess weiter zu optimieren."

      # more_feature_loop
      - title: "Erkennen Sie Suchanfragen mit unterschiedlichem Tastaturlayout"
        content: "GroupDocs.Search für Java erkennt Suchanfragen, die nicht zu Ihrem Tastaturlayout passen. Derzeit können 88 Sprachen und 164 verschiedene Tastaturlayouts erfolgreich von GroupDocs.Search for Java erkannt werden."

      # more_feature_loop
      - title: "Suche mit morphologischer Wortform"
        content: "Mit GroupDocs.Search für Java haben Sie die Freiheit, nach verschiedenen Wortformen zu suchen. Sie können nach Singular- und Pluralform eines bestimmten Substantivs suchen. Oder Sie können alle Formen eines Verbs durchsuchen. Wurzel, Singular der dritten Person und Präteritum sowie verschiedene andere Formen können ebenfalls durchsucht werden. Für nicht englische Sprachen können Sie benutzerdefinierte Wortformen konfigurieren."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search bietet APIs zum Anzeigen von Dokumenten für andere beliebte Entwicklungsumgebungen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for .NET"
          image: "/border/groupdocs-search-net.svg"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

        # solution loop
        - img_alt: "GroupDocs.Search for Node.js"
          image: "/border/groupdocs-search-nodejs-java.svg"
          product: "GroupDocs.Search"
          platform: "Node.js via Java"
          link: "/search/nodejs-java/"

############################# Back to top ###############################
back_to_top:
  enable: true
---