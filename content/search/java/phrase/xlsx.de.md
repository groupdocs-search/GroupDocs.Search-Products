
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: de
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Suchphrasen in XLSX mit Java finden"
head_description: "GroupDocs.Search for Java erweitert Java Anwendungen um fortschrittliche Suchfunktionen für Dokumenteninhalte."

############################# Header ############################
title: "Phrasen in Dokumenten finden" 
description: "Lokalisieren Sie schnell spezifische Phrasen mit GroupDocs.Search for Java. Fügen Sie leistungsstarke Suchfunktionen zu Ihren Java Anwendungen hinzu."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Herunterladen"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search Funktionen"
    link: "/search/java/"
    link_title: "Erfahren Sie mehr"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) ist eine robuste Bibliothek zum Indizieren und Suchen von Text innerhalb von Dokumenten. Sie unterstützt über 70 Dateiformate, darunter PDFs, Word-Dokumente, Excel-Tabellen, Bilder und ZIP-Dateien, um schnelle und präzise Suchergebnisse zu gewährleisten.

############################# Steps ############################
steps:
    enable: true
    title: "So finden Sie Phrasen in XLSX Dokumenten"
    content: |
      [GroupDocs.Search](/search/java/) vereinfacht die Phrasensuche in XLSX Dokumenten. Verwenden Sie verschiedene Optionen, um die Suchergebnisse in Java Anwendungen zu verfeinern.
      
      1. Erstellen Sie ein Verzeichnis für den Suchindex.
      2. Geben Sie den Ordner mit XLSX Dateien an.
      3. Passen Sie die Suchparameter an.
      4. Rufen Sie die Suchergebnisse ab und analysieren Sie diese.
   
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
        // Definieren Sie den Pfad des Suchindex
        Index index = new Index("c:/MyIndex");

        // Geben Sie den Ordner mit den Dokumenten an
        index.add("c:/MyDocuments");

        // Stellen Sie die Suchpräferenzen ein
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Führen Sie die Suchanfrage aus
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erforschen Sie die Dokumentensuchmaschine von Java"
  description: "GroupDocs.Search for Java ermöglicht die Phrasensuche in über 70 Dateiformaten. Finden und organisieren Sie Daten mithilfe fortschrittlicher Suchfunktionen."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Wesentliche Funktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Phrasensuche"
      content: "Lokalisieren Sie exakte Phrasen in Geschäftsdokumenten, wie PDFs, Word-Dateien, Präsentationen und Tabellen. Verwenden Sie Platzhalter und andere Optionen, wenn die genaue Phrase unbekannt ist."

    # feature loop
    - title: "Optimierte Datenindizierung"
      content: "Beschleunigen Sie die Dokumentensuche, indem Sie Suchindizes erstellen und wiederverwenden. Die Indizierung organisiert Daten effizient für schnellere und genauere Suchen."

    # feature loop
    - title: "Mehrsprachige Kompatibilität"
      content: "Durchsuchen Sie Dokumente in über 80 Sprachen. Unterstützt verschiedene Tastaturlayouts und morphologische Analysen zur Verbesserung der Suchgenauigkeit."

    # feature loop
    - title: "Erweiterte Suchoptionen"
      content: "Passen Sie Suchen mit Groß-/Kleinschreibung, unscharfen Suchen, homophonen Anpassungen, Dokumentfilterung und anderen leistungsstarken Funktionen an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Nutzung fortschrittlicher Suchmethoden"
      content: |
        Erfahren Sie, wie Sie Abfragen für die Suche in XLSX erstellen.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Definieren Sie das Verzeichnis für den Suchindex
          Index index = new Index("c:/MyIndex");
              
          // Setzen Sie den Pfad zu den Ziel-Dokumenten
          index.add("c:/MyDocuments");

          // Erstellen Sie eine Suchanfrage für eine spezifische Phrase
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Rufen Sie die Suchergebnisse ab
          SearchResult result = index.search(query);
          
          // Verarbeiten und nutzen Sie die abgerufenen Ergebnisse
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Erweiterte Suchfunktionen"
    exclude: "phrase"
    description: "Nutzen Sie modernste Suchfunktionen für verbesserte Genauigkeit und Leistung."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Suchphrasen in Geschäftsdokumenten"
    exclude: "XLSX"
    description: "GroupDocs.Search ermöglicht die Phrasensuche in über 70 Dokumentenformaten. Nutzen Sie fortschrittliche Optionen und Indizierung für effiziente Suchen."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Microsoft Word Open XML Dokument"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "PowerPoint Open XML Präsentation"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Microsoft Excel Open XML Tabelle"
  

---