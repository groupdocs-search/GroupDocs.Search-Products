
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: de
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Fall-Insensitive Suchen in TXT mit Java"
head_description: "Die GroupDocs.Search for Java API unterstützt Java Entwickler bei der Durchführung von groß-/kleinschreibungssensitiven Suchen über mehrere Dokumenttypen."

############################# Header ############################
title: "Groß-/Kleinschreibungssensitive Dokumentensuche" 
description: "GroupDocs.Search for Java ermöglicht Ihnen die Implementierung präziser, groß-/kleinschreibungssensitiver Suchfunktionen in Ihren Java Projekten."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlos Erhalten"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Erfahren Sie mehr über GroupDocs.Search"
    link: "/search/java/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) ist ein vielseitiges Tool für die Textsuche und Indizierung über verschiedene Dokumente hinweg. Es unterstützt über 70 Formate wie PDFs, Word-Dateien, PowerPoint-Präsentationen, Excel-Tabellen, Bilder und ZIPs, sodass Sie umfangreiche Datensätze effizient verwalten können.

############################# Steps ############################
steps:
    enable: true
    title: "Leitfaden zur groß-/kleinschreibungssensitiven Suche in TXT Dateien"
    content: |
      Mit [GroupDocs.Search](/search/java/) können Sie groß-/kleinschreibungssensitive Suchen in TXT Dokumenten durchführen und Ihre Java Projekte erweitern.
      
      1. Legen Sie den Ordner für die Speicherung des Suchindex fest.
      2. Wählen Sie den Ordner mit TXT Dateien aus.
      3. Führen Sie die groß-/kleinschreibungssensitive Suche aus und sammeln Sie die Ergebnisse.
      4. Verarbeiten und nutzen Sie die Suchergebnisse.
   
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
        // Legen Sie den Speicherort für den Index fest
        Index index = new Index("c:/MyIndex");

        // Weisen Sie auf den Ordner hin, der die zu durchsuchenden Dokumente enthält
        index.add("c:/MyDocuments");

        // Aktivieren Sie den groß-/kleinschreibungssensitiven Modus in den Sucheinstellungen
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Führen Sie die Suche aus
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Such- und Indizierungswerkzeuge"
  description: "Mit GroupDocs.Search for Java können Sie die Dokumentensuche und Indizierung für mehr als 70 Formate optimieren, was das Auffinden und Organisieren von Informationen erleichtert."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Highlights von GroupDocs.Search"
  features:
    # feature loop
    - title: "Flexibele Textsuche"
      content: "Durchsuchen Sie Dokumente wie PDFs, Word-Dateien, Tabellenkalkulationen und Präsentationen. Nutzen Sie Funktionen wie exakte Übereinstimmungen, unscharfe Suche und Platzhalterunterstützung zur Verfeinerung Ihrer Ergebnisse."

    # feature loop
    - title: "Effizientes Indexmanagement"
      content: "Organisieren und indizieren Sie große Datensätze, um die Suchgeschwindigkeit und -leistung beim Bearbeiten großer Dokumentensammlungen zu verbessern."

    # feature loop
    - title: "Unterstützung verschiedener Sprachen"
      content: "Führen Sie Suchen in über 80 Sprachen durch und berücksichtigen Sie verschiedene Tastaturlayouts und sprachliche Variationen für bessere Genauigkeit."

    # feature loop
    - title: "Anpassbare Suchfilter"
      content: "Passen Sie die Suchkriterien mit Optionen wie Groß-/Kleinschreibungssensitivität, Datumsbereichsfilterung und dem Ausschluss unerwünschter Wörter oder Daten während der Indizierung an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Beispiel: Groß-/Kleinschreibungssensitive Suchabfragen"
      content: |
        Dieses Beispiel zeigt, wie Sie groß-/kleinschreibungssensitive Suchen für TXT Dokumente implementieren können.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Definieren Sie das Verzeichnis für den Suchindex
          Index index = new Index("c:/MyIndex");
              
          // Geben Sie den Speicherort des Dokumentenordners an
          index.add("c:/MyDocuments");

          // Richten Sie eine Suchanfrage ein
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Aktivieren Sie die Groß-/Kleinschreibungssensitivität in den Suchoptionen
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Führen Sie die Dokumentensuche durch
          SearchResult result = index.search(wordQuery, options);
          
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
          copy_tip: "Klicken, um zu kopieren"
          copy_done: "kopiert"
        top_links:
          #  loop
          - title: "Ergebnis herunterladen"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
    title: "Überblick über die Hauptfunktionen"
    exclude: "case-sensitive"
    description: "Entdecken Sie die robusten und effektiven Suchmöglichkeiten, die GroupDocs.Search for Java bietet."
    items: 
          
        # operation loop 1
        - name: "Suche nach Bedingungen"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "Informationen in Dokumenten anhand boolescher Bedingungen finden"

        # operation loop 2
        - name: "Groß- und kleinschreibungssensitive Suche"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "Verbessern Sie die Suchgenauigkeit, indem Sie die Groß- und Kleinschreibung berücksichtigen"

        # operation loop 3
        - name: "Dokumentenindizierung"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "Indizieren Sie Dokumente einmal und verwenden Sie den Index für mehrere Suchen"

        # operation loop 4
        - name: "Suchfilter"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "Verwenden Sie Filter, um die verarbeiteten Daten einzugrenzen"

        # operation loop 5
        - name: "Exakte Phrase"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "Nach einem bestimmten Satz oder einer bestimmten Phrase suchen"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Unterstützte Dateiformate für Suchen"
    exclude: "TXT"
    description: "GroupDocs.Search arbeitet mit über 70 gängigen Dokumentformaten, bietet anpassbare Suchoptionen und effiziente Indizierung."
    items: 
        # format loop 1
        - name: "Groß- und kleinschreibungssensitive Suche in DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Groß- und kleinschreibungssensitive Suche in PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Groß- und kleinschreibungssensitive Suche in PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Groß- und kleinschreibungssensitive Suche in TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Groß- und kleinschreibungssensitive Suche in XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---