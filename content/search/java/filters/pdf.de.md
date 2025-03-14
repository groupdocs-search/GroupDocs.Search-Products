
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: de
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "In PDF-Dokumenten mit Java suchen"
head_description: "GroupDocs.Search for Java fügt leistungsstarke Textsuche zu Java-Anwendungen hinzu und unterstützt verschiedene Geschäftsdateiformate."

############################# Header ############################
title: "Text in Geschäftsdokumenten finden" 
description: "GroupDocs.Search for Java ermöglicht die Textsuche in Dokumenten durch flexible und präzise Abfragen. Integrieren Sie die Suchfunktionalität nahtlos in Java-Anwendungen."
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
    title: "Was ist GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) ist eine robuste Bibliothek für schnelle Textsuche und Dokumentindizierung. Sie unterstützt über 70 Dateiformate, einschließlich weit verbreiteter Standards wie PDF, Word, Excel und PowerPoint. Verbessern Sie Ihre Anwendungen mit schnellen und präzisen Suchfunktionen.

############################# Steps ############################
steps:
    enable: true
    title: "So suchen Sie in PDF-Dokumenten"
    content: |
      [GroupDocs.Search](/search/java/) ermöglicht schnelle und effektive Textsuchen in PDF-Dokumenten, ideal für Java-Anwendungen.
      
      1. Geben Sie einen Ordner an, um den Suchindex zu speichern.
      2. Wählen Sie den Ordner mit Ihren Dokumenten aus.
      3. Konfigurieren Sie die Suchoptionen, um die Ergebnisse auf PDF-Dokumente zu beschränken.
      4. Führen Sie die Suche aus und erhalten Sie Ergebnisse.
   
    code:
      platform: "java"
      copy_title: "Kopieren"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Suchergebnis"
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
        copy_tip: "Klicken, um zu kopieren"
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
        // Verzeichnis zum Speichern des wiederverwendbaren Suchindex
        Index index = new Index("c:/MyIndex");

        // Ordner mit den Dokumenten
        index.add("c:/MyDocuments");

        // Suchergebnisse nach Dokumentformat filtern
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // Suchergebnisse abrufen
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Suchfunktionen"
  description: "GroupDocs.Search for Java bietet eine fortschrittliche Textsuche über mehr als 70 Dateiformate hinweg. Die Indizierung beschleunigt Suchen und verbessert die Effizienz des Dokumentenmanagements."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Hauptmerkmale von GroupDocs.Search"
  features:
    # feature loop
    - title: "Leistungsstarke Textsuche"
      content: "Finden Sie Text in gängigen Dokumentenformaten wie PDFs, Word-Dokumenten, Präsentationen und Tabellenkalkulationen. Unterstützt verschiedene Suchmethoden, einschließlich unscharfer Suche, Homophone und Platzhalter."

    # feature loop
    - title: "Optimierte Indizierung für bessere Leistung"
      content: "Erstellen und verwenden Sie Suchindizes erneut, um Geschwindigkeit und Effizienz der Suche, insbesondere in großen Dokumentensammlungen, zu verbessern."

    # feature loop
    - title: "Mehrsprachige Unterstützung für die Suche"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen. Erkennt verschiedene Tastaturlayouts und Wortvariationen für eine verbesserte Genauigkeit."

    # feature loop
    - title: "Anpassbare Suchoptionen"
      content: "Eingrenzen von Suchergebnissen mit Filtern, regulären Ausdrücken und anderen erweiterten Suchoptionen."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Dokumente vor der Suche filtern"
      content: |
        Erfahren Sie, wie Sie Suchanfragen mit Filtern verfeinern können.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Erstellen Sie einen Index, der bestimmte Dateiformate ausschließt.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Geben Sie den Speicherpfad für Dokumente an.
          index.add("c:/MyDocuments");

          // Suchergebnisse abrufen.
          SearchResult result = index.search("Lorem", options);
          
          // Verarbeiten und verwenden Sie die Suchergebnisse.
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
          copy_tip: "Klicken, um zu kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pdf"
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
  title: "Bereit, loszulegen?"
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
    title: "Hauptmerkmale"
    exclude: "filters"
    description: "Führen Sie präzise und effektive Textsuchen durch."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "In Geschäftsdokumenten suchen"
    exclude: "PDF"
    description: "GroupDocs.Search unterstützt über 70 Dateiformate, wodurch die Suche in gängigen Office-Dokumenten vereinfacht wird."
    items: 
        # format loop 1
        - name: "Suchfilter für DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Suchfilter für PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Suchfilter für PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Suchfilter für TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Suchfilter für XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---