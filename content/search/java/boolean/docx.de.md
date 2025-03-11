
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: de
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Boolesche Suche in DOCX mit Java"
head_description: "Mit GroupDocs.Search for Java können Entwickler Dokumentensuchen mithilfe von Booleschen Operatoren wie AND, OR und NOT durchführen."

############################# Header ############################
title: "Boolesche Textsuche" 
description: "Nutzen Sie GroupDocs.Search for Java, um in Ihren Java-Projekten komplexe boolesche (AND, OR, NOT) Suchanfragen zu erstellen."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos herunterladen"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Über GroupDocs.Search"
    link: "/search/java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) ist eine vielseitige Bibliothek, die für die Textsuche und Datenindizierung in Dokumenten entwickelt wurde. Sie unterstützt über 70 Dateitypen, darunter PDF, Word, Excel, PowerPoint-Bilder und ZIP-Archive, und ermöglicht effiziente Suchen in großen Datenmengen.

############################# Steps ############################
steps:
    enable: true
    title: "So führen Sie Boolesche Suchen in DOCX-Dokumenten durch"
    content: |
      [GroupDocs.Search](/search/java/) ermöglicht zielgerichtete Textsuchen in DOCX-Dokumenten. Mit Unterstützung für boolesche Bedingungen können Sie die Suchgenauigkeit in Java-Anwendungen erhöhen.
      
      1. Geben Sie den Ordner an, in dem der Suchindex gespeichert werden soll.
      2. Wählen Sie den Ordner mit den DOCX-Dokumenten aus.
      3. Führen Sie die Suchanfrage aus und rufen Sie die Ergebnisse ab.
      4. Verarbeiten Sie die erhaltenen Ergebnisse.
   
    code:
      platform: "java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "Klicken zum Kopieren"
        copy_done: "kopiert"
      links:
        #  loop
        - title: "Weitere Beispiele"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Dokumentation"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Legen Sie den Pfad für den Indexordner fest
        Index index = new Index("c:/MyIndex");

        // Geben Sie den Ordnerpfad mit den Dokumenten für die Suche an
        index.add("c:/MyDocuments");

        // Führen Sie eine Suche mit einer komplexen Abfrage aus
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Leistungsstarke Werkzeuge für Dokumentensuche und Indizierung"
  description: "GroupDocs.Search for Java vereinfacht die Textsuche und Datenindizierung für über 70 Formate. Ihre fortschrittlichen Werkzeuge ermöglichen es Ihnen, Inhalte mühelos zu finden und zu verwalten."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Wichtige Funktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Umfassende Textsuche"
      content: "Suchen Sie über mehrere Formate wie PDFs, Word-Dokumente, Präsentationen, Tabellenkalkulationen und mehr. Nutzen Sie Optionen wie exakte Übereinstimmungen, unscharfe Suche und Platzhalterabfragen zur Verfeinerung der Ergebnisse."

    # feature loop
    - title: "Effiziente Datenindizierung"
      content: "Erstellen und pflegen Sie Indizes für schnellere Dokumentensuchen. Diese Funktion organisiert Daten effizient, was die Handhabung großer Dokumentensammlungen erleichtert."

    # feature loop
    - title: "Mehrsprachige Unterstützung"
      content: "Suchen Sie in Dokumenten, die in über 80 Sprachen verfasst sind. Steigern Sie die Genauigkeit durch morphologische Wortformen und verschiedene Tastaturlayouts."

    # feature loop
    - title: "Flexible Suchanpassung"
      content: "Passen Sie die Sucheinstellungen mit Funktionen wie Groß-/Kleinschreibung, Datumsbereichsfiltern und Ausschlüssen zur Verfeinerung Ihrer Ergebnisse an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Verwendung komplexer Boolescher Suchabfragen"
      content: |
        Dieses Beispiel demonstriert, wie Boolesche Suchen in DOCX-Dateien durchgeführt werden.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Legen Sie den Ordner für den Suchindex fest
          Index index = new Index("c:/MyIndex");
              
          // Geben Sie den Pfad zu den zu durchsuchenden Dokumenten an
          index.add("c:/MyDocuments");

          // Bauen Sie die Abfrage mithilfe Boolescher Logik auf
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Rufen Sie die Suchergebnisse ab
          SearchResult result = index.search(booleanQuery);
          
          // Verarbeiten Sie die abgerufenen Ergebnisse
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Kopieren"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "Klicken zum Kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
        links:
          #  loop
          - title: "Weitere Beispiele"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Dokumentation"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Bereit zum Starten?"
  description: "Testen Sie die Funktionen von GroupDocs.Search kostenlos oder fordern Sie eine Lizenz an"
  items:
    #  loop
    - title: "Maven Download"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Lizenzierung"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Wichtige Funktionen auf einen Blick"
    exclude: "boolean"
    description: "Entfesseln Sie leistungsstarke und effiziente Suchfähigkeiten"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Beliebte Dokumentformate durchsuchen"
    exclude: "DOCX"
    description: "GroupDocs.Search unterstützt über 70 Dateiformate, sodass Sie Suchregeln anpassen und die Indizierung nutzen können, um die Leistung zu optimieren."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word Open XML Dokument"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPoint Open XML Präsentation"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft Excel Open XML Tabelle"
  

---