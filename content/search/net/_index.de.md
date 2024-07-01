---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET Textsuche & Indizierung API for Word Excel PDF Email HTML"
head_description: "C# .NET-Textsuch-API zum intelligenten Indizieren und Abrufen von Daten aus PDF-, Microsoft Office Word-, Excel-, Präsentations-, OneNote-, E-Mail-, ZIP-, EPUB- und Webdateien."

############################# Header ############################
title: ".NET-API zum Suchen und Indizieren von Dokumenten"
description: "API zum Indizieren von Daten und Durchführen einer Textsuche in allen gängigen Dokumentformaten mit .NET-Anwendungen."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "/border/groupdocs-search-net.svg"
        product: "GroupDocs.Search"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "Preisgestaltung"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Überblick ############################
overview:
    enable: true
    content: |
      GroupDocs.Search für .NET ist eine Dokument- und Textsuch-API für Geschäftsanwendungen, die in C#, ASP.NET und anderen .NET-Technologien entwickelt wurden. Diese .NET-API unterstützt grundlegende bis erweiterte Suchfunktionen, z. B. das Erstellen und Zusammenführen mehrerer Indizes, das Durchsuchen von Indizes mit Einfach, Boolesch, Fuzzy, regulären Ausdrücken (Regex) und anderen Abfragetypen, um Ihre erforderlichen Daten aus Dateien, Dokumenten usw. abzurufen E-Mails, durch intelligente Suche. Wenn Sie eine schnelle, zuverlässige, intelligente und funktionsreiche Suchanwendung für Ihre Endbenutzer erstellen möchten, die alle gängigen Dateiformate unterstützt, ist GroupDocs.Search für .NET alles, was Sie brauchen.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Nachfolgend finden Sie eine Übersicht über GroupDocs.Search für .NET:
      
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
          GroupDocs.Search für .NET unterstützt die folgenden [Dokumentdateiformate](https://docs.groupdocs.com/search/net/supported-document-formats/):

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
          GroupDocs.Search for .NET unterstützt das Folgen Betriebssysteme, Frameworks & Paket-Managers:
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Betriebssysteme"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Unterstützte Frameworks"
              content: |
                * .NET Framework 2.0 oder höher
                * Mono Framework 1.2 oder höher
                * .NET-Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Paket-Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Entwicklungsumgebungen"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Merkmale ############################
features:
    enable: true
    title: "GroupDocs.Search for .NET Merkmale"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Index im Arbeitsspeicher oder auf Festplatte erstellen & Multithreaded Indizierung & Merging durchführen"

      # feature loop
      - icon: "fas fa-eye"
        content: "Indizierung für bereits indizierte Dateien oder mit einer bestimmten Zeichenfolge im Namen verhindern"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Zeigen Sie den Fortschrittsprozentsatz der Indexerstellung und -aktualisierung an und erhalten Sie einen Suchbericht"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Schnellere Indizierung durch Ausschluss bestimmter Wörter & Indexstatus-Benachrichtigung für kürzlich verarbeitete Dateien"

      # feature loop
      - icon: "fas fa-code"
        content: "Indizieren Sie ZIP-Archive innerhalb von ZIP-Archiven und erhalten Sie eine Liste der indizierten Dateien, die in einem Archiv enthalten sind"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Verwenden Sie Auflisten oder Importieren, um Zeichen während der Indizierung zu ersetzen und in eine Datei zu exportieren"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Passwortgeschützte Dateien indexieren & suchen & kompakte Indizierung, um Speicherplatz zu sparen"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Extrahieren Sie Text aus dem Index oder der Quelldatei und speichern Sie die Codierung der Textdatei automatisch im Index"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Fügen Sie bei der Indizierung jedem Dokument beliebige Zusatzfelder hinzu"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Richten Sie die Dokumentenfilterung in den Suchergebnissen ein"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Behandeln Sie Tippfehler durch Ungenaue Suche, legen Sie den Ähnlichkeitsgrad in Ungenaue Suche fest und zeigen Sie nur die besten Ergebnisse an"

      # feature loop
      - icon: "fas fa-columns"
        content: "Indizieren Sie Dokumente aus Streams und Datenstrukturen"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Suchen Sie nach vollständigen Sätzen mit Stoppwörtern und kombinieren Sie die facettierte Suche mit der booleschen Suche"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Suche basierend auf homophonen Begriffen, Synonymen, Datumsbereich, Platzhaltern und Groß-/Kleinschreibung"

      # feature loop
      - icon: "fas fa-print"
        content: "Indizieren und suchen Sie E-Mails aus Outlook und durchsuchen Sie sie mit der Aspose.Email-API"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Unterstützt Rechtschreibprüfung und Platzhalter in Suchanfragen und Überspringen von Sonderzeichen in Suchphrasen"

      # feature loop
      - icon: "fas fa-lock"
        content: "Begrenzen Sie die Ergebnisse für jeden Begriff in der Suchanfrage sowie für alle Ergebnisse"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Extrahieren Sie HTML-Text in eine Datei und generieren Sie eine URL, um durch HTML-formatierte Suchergebnisse zu navigieren"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Kombinieren Sie mehrere Abfragen in einem einzigen Objektbaum"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Benachrichtigen Sie den Benutzer über nicht unterstützende Einstellungen und automatisches Neuladen des Index im Falle eines Indizierungsfehlers"

      # feature loop
      - icon: "fas fa-heading"
        content: "Aktivieren Sie die genaue Anzahl der Vorkommen für jedes gefundene Wort, um bei Rechtschreibfehlern alternative Wortvorschläge anzubieten"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Hinzufügen von Textattributen zu indizierten Dokumenten ohne Neuindizierung"

      # feature loop
      - icon: "fas fa-cube"
        content: "Führen Sie Indizierung und Suchoperationen basierend auf Zeichen durch"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Index-Metadaten von nicht-textuellen Dokumentformaten"

    more_feature:
      # more_feature_loop
      - title: "Indizierung & Search"
        content: |
          GroupDocs.Search für die .NET-API verwendet häufig den Index, um eine Suche durchzuführen. Indizes werden verwendet, um Daten für eine schnelle und genaue Suche zu sammeln, zu analysieren oder zu speichern.

          * **Index erstellen**: Indexordner erstellen und Dokumente zu diesem Ordner hinzufügen/indizieren.
          * **Index laden**: Laden Sie einen bestehenden Index.
          * **Dokumente zum Index hinzufügen**: Dokumente asynchron zum bestehenden Index hinzufügen.
          * **Index aktualisieren**: Aktualisieren Sie den bestehenden Index, wenn ein Dokument geändert, hinzugefügt oder gelöscht wird. Dadurch bleiben die Suchergebnisse aktuell.

          ```cs
          Index  index = new Index(@"c:\MyIndex");
          index.AddToIndex(@"c:\MyDocuments");
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      # more_feature_loop
      - title: "Führen Sie mehrere Indizes zusammen, um die Sucheffizienz zu verbessern"
        content: "GroupDocs.Search für .NET kann mehrere Indizes zu einem einzigen Index zusammenführen. Wenn ein Index häufig aktualisiert wird, hat er mehrere Delta-Indizes, aber dieser Ansatz verringert die Suchleistung. GroupDocs.Search for .NET API führt alle Delta-Indizes zu einem konsolidierten Index zusammen. Der primäre zusammengeführte Index enthält alle Informationen aus den zusammengeführten Delta-Indizes; die Delta-Indizes bleiben jedoch unverändert. Dieser von unserer API verwendete Ansatz verbessert die Sucheffizienz erheblich. Die Funktion zum Zusammenführen von Indizes bietet zahlreiche Funktionalitäten zum Optimieren, um diesen Prozess weiter zu optimieren."

      # more_feature_loop
      - title: "Speichern Sie Text im Index, um HTML-Markup zu generieren"
        content: "GroupDocs.Search für .NET kann Text indizierter Dokumente in einem Index zwischenspeichern. Dieser zwischengespeicherte Text wird dann verwendet, um schnell HTML-Markup zu generieren, indem Suchergebnisse hervorgehoben werden. Dieser Ansatz ist viel schneller als das direkte Extrahieren von Text aus Dateien. Das Abrufen von Text aus dem Cache ist auch dann verfügbar, wenn die Quelldateien nicht mehr verfügbar sind. Der zwischengespeicherte Text kann gespeichert werden, indem verschiedene Komprimierungsstufen angewendet werden, um weniger Speicherplatz zu belegen und die Indizierungszeit zu verkürzen."

      # more_feature_loop
      - title: "Erhalten Sie verwandte Dokumente durch Fuzzy- und Regex-Suche"
        content: "Wenn Sie eine Fuzzy- oder Regex-Suche durchführen, können Sie die Liste der Dokumente abrufen, die genau mit Ihrer Eingabe übereinstimmen. Sie erhalten jedoch auch eine Liste von Dokumenten, die Wörter oder Begriffe enthalten, die Ihrer Eingabe ähnlich sind. Wenn Sie beispielsweise GroupDocs.Search für .NET verwenden und eine Fuzzy-Suche nach der Abfrage „Kosten“ durchführen, erhalten Sie Dokumente, die das Wort „Kosten“ enthalten, und Dokumente, die ähnliche Wörter wie „Mantel“ enthalten. Die Ergebnisse hängen davon ab, welchen Grad an Unschärfe Sie mit dieser API konfiguriert haben."

      # more_feature_loop
      - title: "Erkennen Sie Suchanfragen mit unterschiedlichem Tastaturlayout"
        content: "GroupDocs.Search für .Net kann Suchanfragen erkennen, die in einer Sprache geschrieben sind, die nicht mit Ihrem Tastaturlayout übereinstimmt. Derzeit kann diese .NET-API erfolgreich 88 Sprachen und 164 verschiedene Tastaturlayouts erkennen."

      # more_feature_loop
      - title: "Suche mit morphologischer Wortform"
        content: "GroupDocs.Search for .NET API ermöglicht Ihnen die Suche nach verschiedenen Wortformen. Beispielsweise können Sie für ein Substantiv nach seiner Singular- und Pluralform suchen. Bei einem Verb können Sie nach allen Formen dieses Verbs suchen. Sie können auch nach Wurzel, Singular in der dritten Person, Präteritum und verschiedenen anderen Formen suchen. Für andere Sprachen als Englisch können Sie benutzerdefinierte Wortformen implementieren."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search bietet APIs zum Anzeigen von Dokumenten für andere beliebte Entwicklungsumgebungen"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for Java"
          image: "/border/groupdocs-search-java.svg"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

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
