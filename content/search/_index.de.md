---
############################# Static ############################
layout: "family"
date:  2025-01-09T15:38:59
draft: false

product: "Search"
product_tag: "search"

lang: de

############################# Head ############################
head_title: "Dokumententextsuche und Indizierung | APIs & Kostenlose Webanwendung"
head_description: "Führen Sie effiziente Textsuche und Datenindizierung in PDF, MS Office, OpenDocument und anderen gängigen Dateiformaten mit unseren APIs oder der kostenlosen Online-Dokumentensuchanwendung durch."

############################# Header ############################
title: "Umfassende Dokumentensuch- und Indizierungslösung"
description:  |
  Führen Sie die Textsuche und Indizierung in PDF, Microsoft Office, OpenOffice und vielen anderen Dokumentdateiformaten durch.

  Finden Sie schnell Informationen in großen Dokumentensammlungen mit fortschrittlichen Volltextsuchfunktionen.

  Passen Sie Suchfunktionen wie Synonyme, unscharfe Suche und Stemming an, um die Genauigkeit und Ergebnisse zu verbessern.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Wählen Sie Ihre Plattform"
  title: "Plattformunabhängigkeit"
  description: "GroupDocs.Search ist mit den folgenden Betriebssystemen und Frameworks kompatibel:"
  details_link_title: "Erfahren Sie mehr"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Jeder andere Texteditor
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Hauptmerkmale von GroupDocs.Search"
  description: "GroupDocs.Search bietet leistungsstarke Werkzeuge zur Indizierung und Suche von Text in gängigen Dokumentformaten. Vereinfachen und verbessern Sie das Dokumentenmanagement mit erweiterten Suchfunktionen."

  items:
    # items loop
    - icon: "view"
      title: "Erweiterte Textsuche"
      content: "Führen Sie schnelle und präzise Textsuchen in indizierten Dokumenten durch."

    # items loop
    - icon: "manipulate"
      title: "Anpassbare Suchoptionen"
      content: "Nutzen Sie Funktionen wie unscharfe Suche, Synonyme und Stemming für genauere Ergebnisse."

    # items loop
    - icon: "merge"
      title: "Unterstützung für mehrere Formate"
      content: "Indizieren und suchen Sie Inhalte in Microsoft Office, PDF, OpenOffice und anderen gängigen Formaten."

    # items loop
    - icon: "additional"
      title: "Effiziente Indizierung"
      content: "Erstellen und pflegen Sie schnell Indizes für große Dokumentensammlungen."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Textsuche in gängigen Dokumentformaten"
  description: "GroupDocs.Search Codebeispiele"
  items:
    # code sample loop
    - title: "Textsuche"
      content: |
       GroupDocs.Search ist ein leistungsstarkes Werkzeug zur Auffindung von Text in Dokumenten. Sie können durch mehrere Dokumente in verschiedenen Formaten suchen, die in einem bestimmten Ordner gespeichert sind. Die Suchergebnisse werden in einem separaten Ordner gespeichert, sodass Sie darauf zugreifen und sie ohne erneute Suche wiederverwenden können.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Erstellen Sie eine Instanz der Index-Klasse und geben Sie den Speicherort für die Indizes an.
            Index index = new Index("\\Index Folder");

            //Geben Sie den Pfad zu den Dokumenten an, in denen die Suche durchgeführt wird.
            index.Add("\\Documents Folder");

            //Erstellen Sie eine Instanz des SearchOptions-Objekts.
            SearchOptions options = new SearchOptions();

            //Führen Sie die Suche nach dem gewünschten Text durch.
            SearchResult result = index.Search("ipsum dolor", options);

            //Verarbeiten Sie die Suchergebnisse.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Erstellen Sie eine Instanz der Index-Klasse und geben Sie den Speicherort für die Indizes an.
            Index index = new Index("\\Index Folder");

            //Geben Sie den Pfad zu den Dokumenten an, in denen die Suche durchgeführt wird.
            index.add("\\Documents Folder");

            //Erstellen Sie eine Instanz des SearchOptions-Objekts.
            SearchOptions options = new SearchOptions();

            //Führen Sie die Suche nach dem gewünschten Text durch.
            SearchResult result = index.search("ipsum dolor", options);

            //Verarbeiten Sie die Suchergebnisse.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Erstellen Sie eine Instanz der Index-Klasse und geben Sie den Speicherort für die Indizes an.
            const index = new searchLib.Index('\\Index Folder');

            //Geben Sie den Pfad zu den Dokumenten an, in denen die Suche durchgeführt wird.
            index.add('\\Documents Folder');

            //Erstellen Sie eine Instanz des SearchOptions-Objekts.
            const options = new searchLib.SearchOptions();

            //Führen Sie die Suche nach dem gewünschten Text durch.
            const result = index.search('ipsum dolor', options);

            //Verarbeiten Sie die Suchergebnisse.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Unterstützt über 70 Dateiformate"
  description: "GroupDocs.Search unterstützt fast alle gängigen Dateiformate."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Unsere Produktstatistiken"
  description: "Entdecken Sie wichtige Kennzahlen, die unsere Leistung, Reichweite und Wachstum zeigen."

  items:
    # items loop
    - number: "70+"
      title: "Unterstützte Formate"
      content: "Wir bieten Kompatibilität mit über 70 gängigen Dokumentformaten."

    # items loop
    - number: "500k"
      title: "NuGet-Downloads"
      content: "GroupDocs.Search für .NET wurde über 500.000 Mal auf NuGet heruntergeladen."

    # items loop
    - number: "12k"
      title: "Maven-Downloads"
      content: "Java-Entwickler haben GroupDocs.Search über 12.000 Mal von Maven heruntergeladen."

    # items loop
    - number: "150+"
      title: "Zufriedene Kunden"
      content: "Entwickler und führende Unternehmen weltweit vertrauen auf unsere Produkte für innovative Lösungen."


############################# Customers ###############################
customers:
  enable: true
  title: "Unsere zufriedenen Kunden"
  description: "Die GroupDocs-Bibliotheken werden von führenden Marken und Organisationen weltweit vertraut."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Beginnen Sie Ihre Reise noch heute!"
  description: "Erleben Sie GroupDocs.Search kostenlos auf Ihrer bevorzugten Plattform."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Häufig gestellte Fragen"
  description: "Finden Sie Antworten auf häufige Fragen zu GroupDocs.Search."

  items:
    # items loop
    - question: "Benötigt GroupDocs.Search externe Tools zur Durchsuchung von Dokumenten?"
      answer: "Nein, GroupDocs.Search funktioniert als eigenständige Lösung und benötigt keine zusätzlichen Tools oder Software wie Adobe Acrobat oder Microsoft Office für Suchanfragen."

    # items loop
    - question: "Kann ich GroupDocs.Search vor dem Kauf testen?"
      answer: "Ja, das können Sie! GroupDocs.Search bietet eine kostenlose Testversion. Sie können die Funktionen erkunden, obwohl die Testversion vielleicht Einschränkungen wie Wasserzeichen oder eingeschränkte Funktionalität enthält. Um alle Funktionen freizuschalten, können Sie auf der [temporären Lizenz](https://purchase.groupdocs.com/temporary-license/)-Seite eine kostenlose 30-tägige Testlizenz anfordern."

    # items loop
    - question: "Welche Lizenzierungsoptionen sind verfügbar?"
      answer: "Wir bieten mehrere Lizenzmodelle für GroupDocs.Search, die auf unterschiedliche Bedürfnisse zugeschnitten sind. Wählen Sie eine Lizenz basierend auf der Größe Ihres Teams, dem Nutzungsszenario oder ob Sie das SDK/ die API für die Verteilung an Kunden benötigen. Für flexible Nutzung sollten Sie eine verbrauchsabhängige Lizenz in Betracht ziehen, bei der Sie basierend auf der tatsächlichen Nutzung bezahlen. Erfahren Sie mehr über Ihre Optionen auf der [Preisseite](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Webanwendungen"
  description: "Entdecken Sie GroupDocs.Search mit unserer kostenlosen Webanwendung. Führen Sie Textsuchen und Indizierungen für über 70 gängigen Dateiformaten direkt in Ihrem Browser durch – völlig kostenlos."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Suchen Sie innerhalb von PDF, Excel, Word, PowerPoint und anderen Dateitypen direkt aus Ihrem Webbrowser."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Laden Sie DOCX hoch, um erweiterte Textsuchen durchzuführen, ohne Software installieren zu müssen."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Testen Sie die Indizierungs- und Abruffähigkeiten für PDFs in verschiedenen Formaten kostenlos."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---