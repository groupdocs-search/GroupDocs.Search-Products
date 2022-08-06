---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/java/case-sensitive/csv/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Java-API zur Durchführung einer Textsuche mit Berücksichtigung der Groß-/Kleinschreibung in CSV-Dokumenten"
head_description: "GDie Java-API roupDocs.Search ermöglicht Programmierern, eine Textsuche mit Berücksichtigung der Groß- und Kleinschreibung durchzuführen und die genaue Struktur von Wörtern in CSV-Dokumenten über Java zu ermitteln."

############################# Header ############################
title: "Führen Sie eine Suche mit Berücksichtigung der Groß-/Kleinschreibung in CSV-Dokumenten in Java-Apps durch"
description: "Die Java-API GroupDocs.Search ermöglicht Softwareentwicklern die Textsuche mit Berücksichtigung der Groß- und Kleinschreibung in verschiedenen Dokumenttypen wie PDF, HTML, DOCX, PPTX, XLSX und mehr in Java-Apps."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Wie führe ich eine Suche mit Berücksichtigung der Groß- und Kleinschreibung in Java-Apps durch?"
    content: |
      Groß-/Kleinschreibung ist eine sehr nützliche Suchtechnik, die die Fähigkeit eines Programms beschreibt, zwischen Großbuchstaben (Großbuchstaben) und Kleinbuchstaben (Kleinbuchstaben) bei Web-, Datenbank- oder Dokumentensuchen zu unterscheiden. Es ist sehr wichtig, sich daran zu erinnern, dass die Suchmaschine standardmäßig die Groß-/Kleinschreibung nicht beachtet, was bedeutet, dass die Suche nach dem Wort Computer beide Fragmente mit einem Schlüsselnamen oder Text mit den Wörtern Computer und computer ergibt. Nehmen wir an, wir müssen die Suchergebnisse auf diejenigen mit dem Großbuchstaben „Computer“ eingrenzen, was bedeutet, dass wir eine Suche mit Berücksichtigung der Groß- und Kleinschreibung benötigen. GroupDocs.Search für Java ist eine effektive API zum Suchen und Indexieren von Dokumenten, mit der Softwareentwickler Anwendungen entwickeln können, die eine Textsuche und Indexierung für einige der beliebtesten Dokumenttypen wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblätter, PowerPoint-Präsentationen, Outlook MSG, PST und viele mehr. Darüber hinaus kann es Suchanfragen identifizieren, die in einer Sprache geschrieben sind, die nicht mit Ihrem Tastaturlayout übereinstimmt.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Suche mit Berücksichtigung der Groß- und Kleinschreibung in CSV-Dokumenten über Java"
      content_left: |
       Die Java-API von GroupDocs.Search hat vollständige Unterstützung für grundlegende sowie erweiterte Suchfunktionen integriert, die es Softwareentwicklern ermöglichen, mit nur wenigen Codezeilen in ihren Java-Anwendungen zwischen Groß- und Kleinschreibung zu suchen.
       
       Das folgende Java-Codebeispiel zeigt, wie Sie mit nur wenigen Codezeilen eine Suche mit Berücksichtigung der Groß-/Kleinschreibung mit einer Abfrage im Text in CSV-Dateien erreichen.

      title_right: "Führen Sie eine Suche mit Berücksichtigung der Groß-/Kleinschreibung in CSV-Dateien durch"
      content_right: |
         * Identifizieren Sie den Pfad zum Indexordner sowie zum Dokumentenordner.
         * Erstellen eines Indexes im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)).
         * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Instanz der Klasse [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1).
         * Initiieren Sie eine neue Instanz der Klasse [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
         * Aktivieren der Suchoption mit Berücksichtigung der Groß-/Kleinschreibung durch Aufrufen der Methode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch).
         * Suchabfrage definieren und Suche starten
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Führen Sie eine Suche mit Berücksichtigung der Groß-/Kleinschreibung in Objektform über Java durch"
      content_left: |
        GroupDocs.Search Java gibt Softwareentwicklern die Möglichkeit, Suchfunktionen für verschiedene Dokumentformate in ihre eigenen Anwendungen aufzunehmen. Das folgende Java-Codebeispiel zeigt, wie Sie mit einer Abfrage in Objektform über CSV-Dokumente zwischen Groß- und Kleinschreibung suchen.

      title_right: "Wenden Sie die Suche mit Berücksichtigung der Groß-/Kleinschreibung in CSV Dokumenten an"
      content_right: |
       * Identifizieren Sie den Pfad zum Indexordner sowie zum Dokumentenordner.
       * Erstellen eines Indexes im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)).
       * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Instanz der Klasse [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1).
       * Initiieren Sie eine neue Instanz der Klasse [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
       * Aktivieren der Suchoption mit Berücksichtigung der Groß-/Kleinschreibung durch Aufrufen der Methode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch).
       * Erstellen einer Suchabfrage im Objekt durch Aufrufen der Methode [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)).
       * Suchabfrage definieren und Suche starten
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

    - title_left: "System Requirements"
      content_left: |
        GroupDocs.Search for Java is supported on all major platforms and operating systems. For complete system requirements guide, please visit [system requirements](https://docs.groupdocs.com/search/java/system-requirements/) before executing the code below, please make sure that you have the following prerequisites installed on your system:
         * Operating Systems: Microsoft Windows, Linux, MacOS
         * Java Versions Support: J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above
         * Get the latest version of GroupDocs.Search for Java APIs from GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "Why Use GroupDocs.Search"
      content_right: |
        * Search Index creation in memory as well as on disk.
        * Ability of indexing from a file, stream or structure.
        * Password protected documents indexing support.
        * Support for merging of several indexes.
        * Filter Document during search indexing.
        * Spell check support during the search.
        * Blended characters are fully supported
        * Combining different types of search into one search query.
        * Simple word  and regular expression searches support
        * Fully support alias replacement in search queries.

demos:
    enable: true
        

about_formats:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---