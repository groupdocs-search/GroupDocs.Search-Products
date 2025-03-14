
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: de
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Text in PDF-Dokumenten mit GroupDocs.Search für Java finden"
head_description: "GroupDocs.Search for Java unterstützt Java-Entwickler dabei, Texte schnell in verschiedenen Dokumentformaten zu durchsuchen."

############################# Header ############################
title: "Intelligente Textsuche in Dokumenten" 
description: "Mit GroupDocs.Search for Java können Sie nahtlos Texte aus verschiedenen Dokumenttypen in Ihren Java-Anwendungen durchsuchen und extrahieren."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Kostenlose Testversion erhalten"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Was macht GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Mehr Erfahren"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) ist eine leistungsstarke Bibliothek zur Dokumentensuche und -indizierung, die über 70 Dateiformate unterstützt, darunter PDF, Word, PowerPoint, Excel, Bilder und ZIP-Archive. Sie ermöglicht schnelle, präzise und skalierbare Suchfunktionen für große Dokumentensammlungen.

############################# Steps ############################
steps:
    enable: true
    title: "Durchsuchung von Texten in PDF-Dateien durchführen"
    content: |
      [GroupDocs.Search](/search/java/) ermöglicht es, PDF-Dateien mithilfe komplexer Logik und Indizierung zu durchsuchen, was die Suchgenauigkeit in Java-Anwendungen verbessert.
      
      1. Richten Sie ein Verzeichnis zur Speicherung des Suchindexes ein.
      2. Wählen Sie einen Ordner mit PDF-Dateien aus.
      3. Definieren Sie zusätzliche Suchoptionen.
      4. Führen Sie die Suche aus und analysieren Sie die Ergebnisse.
   
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
        // Verzeichnis für die Speicherung des Suchindex festlegen
        Index index = new Index("c:/MyIndex");

        // Ordner angeben, der durchsuchbare Dokumente enthält
        index.add("c:/MyDocuments");

        // Homophon-Suche aktivieren, um Wörter mit ähnlicher Aussprache zu erfassen
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Führen Sie eine erweiterte Suchanfrage aus
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Erweiterte Such- und Indizierungsfunktionen"
  description: "GroupDocs.Search for Java vereinfacht die Textsuche und Indizierung in über 70 Dokumentformaten und bietet effiziente Werkzeuge, um Informationen schnell zu verwalten und abzurufen."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Kernfunktionen von GroupDocs.Search"
  features:
    # feature loop
    - title: "Umfassende Textsuche"
      content: "Finden Sie Texte in mehreren Dokumentformaten wie PDFs, Word-Dokumenten, PowerPoint-Präsentationen und Tabellen. Nutzen Sie exakte Übereinstimmungen, unscharfe Suche und Wildcard-Operatoren für verfeinerte Suchergebnisse."

    # feature loop
    - title: "Optimierte Indizierung für große Datenmengen"
      content: "Erstellen Sie strukturierte Indizes, um Suchvorgänge zu beschleunigen und effizient durch umfangreiche Dokumentenbestände zu navigieren."

    # feature loop
    - title: "Unterstützt mehrere Sprachen"
      content: "Führen Sie Suchen in über 80 Sprachen durch, mit integrierter Unterstützung für unterschiedliche Tastaturlayouts und Wortmorphologievariationen, um die Genauigkeit zu erhöhen."

    # feature loop
    - title: "Flexible Suchoptionen"
      content: "Passen Sie Suchen mit Optionen wie Groß- und Kleinschreibung, datumsbasiertem Filtern und der Möglichkeit, spezifische Wörter auszuschließen, für präzise Ergebnisse an."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementierung fortgeschrittener Suchabfragen"
      content: |
        Dieses Beispiel zeigt, wie man Suchabfragen verwendet, um effizient in PDF-Daten zu suchen.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Verzeichnis für die Suchindizierung festlegen
          Index index = new Index("c:/MyIndex");
              
          // Dateipfad für die Dokumente angeben
          index.add("c:/MyDocuments");

          // Passwort für verschlüsselte Dokumente eingeben
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", "123456");

          // Unscharfe Suche aktivieren, um ähnliche Wörter zu erkennen
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Suchergebnisse abrufen
          SearchResult result = index.Search("Loarem", options);
          
          // Suchergebnisse verarbeiten und analysieren
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    exclude: "document"
    description: "Entdecken Sie leistungsstarke Textsuchfunktionen, die für Effizienz und Präzision entwickelt wurden."
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
    title: "Informationen in PDF-Dokumenten mit GroupDocs.Search finden"
    exclude: "PDF"
    description: "GroupDocs.Search unterstützt über 70 Formate, einschließlich Office-Dateien, und ermöglicht schnelle Suchen mit fortschrittlichen Indizierungsfunktionen."
    items: 
        # format loop 1
        - name: "Suche im DOCX-Dokument"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Microsoft Word Open XML-Dokument"
          
        # format loop 2
        - name: "Suche im PDF-Dokument"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Suche im PPTX-Dokument"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "PowerPoint Open XML-Präsentation"

        # format loop 4
        - name: "Suche im TXT-Dokument"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Textdokument"
          
        # format loop 5
        - name: "Suche im XLSX-Dokument"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Microsoft Excel Open XML-Spreadsheet"
  

---