---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/java/filters/zip/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "ZIP Dokumentfilterung in Suchergebnis über Java-API integrieren?"
head_description: "GroupDocs.Search Java API hilft Softwareentwicklern, ZIP Suchfunktionen für Dokumente hinzuzufügen und Dokumentfilter anzuwenden, um Suchergebnisse über Java API anzupassen."

############################# Header ############################
title: "So integrieren Sie die Dokumentenfilterung, um Suchergebnisse in Java-Apps anzupassen"
description: "GroupDocs.Search Java API ermöglicht Programmierern die Integration erweiterter ZIP Dokumentsuchfunktionen sowie die Anpassung von Suchergebnissen, indem sie die Dokumentfilterung in ihren Java-Apps festlegen."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "So integrieren Sie die Dokumentenfilterung, um Suchergebnisse in Java-Apps anzupassen"
    content: |
       Das Filtern von Dokumenten ist eine sehr nützliche Aktivität, die es Softwareanwendungen ermöglicht, Dokumente nach der relevanten Wortfolge zu suchen und abzurufen, die von einem Benutzer in den Text von indizierten Dokumenten eingegeben wurde. Ein Filter enthält eine Reihe von Regeln, die Kriterien definieren, die zum Auswählen von Datensätzen verwendet werden. Die Dokumentfilterung ermöglicht es Benutzern, ihre Suche auf einen bestimmten Abschnitt oder einen bestimmten Dokumenttyp einzuschränken sowie durch die Ergebnisse zu navigieren und zu finden, wonach sie suchen. GroupDocs.Search für Java ist eine funktionsreiche, hochleistungsfähige Dokumentenindizierungs- und Such-API, die es Softwareentwicklern ermöglicht, Anwendungen zu erstellen, die eine Textindizierung und Suche nach einigen der beliebtesten Dokumentdateiformate erreichen können. Es unterstützt vollständig verschiedene Dokumenttypen wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblätter, PowerPoint-Präsentationen, Outlook MSG, PST und so weiter. Es stehen verschiedene Arten von Filern zur Verfügung, mit denen Benutzer die Suchergebnisse anpassen können, z. B. Dateipfadfilter, Dateierweiterungsfilter, Attributfilter und viele mehr. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Dokumentfilter beim Durchsuchen von ZIP-Dokumenten über Java anwenden"
      content_left: |
       Die Java-API von GroupDocs.Search hilft Softwareentwicklern, leistungsstarke Anwendungen mit Suchfunktionen unter Verwendung der Java-API zu erstellen. Das folgende Java-Codebeispiel zeigt, wie Sie mit nur wenigen Codezeilen einen Dokumentfilter zum Durchsuchen verschiedener Arten von Dokumenten anwenden.

      title_right: "Dokumentfiltereinstellung beim Durchsuchen von ZIP Dokumenten"
      content_right: |
       * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
       * Erstellen eines Indexes im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)).
       * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)).
       * Erstellen eines Suchoptionsobjekts durch Aufrufen der Klasse [earchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions).
       * Legen Sie den Dokumentfilter fest, indem Sie die Methode [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) aufrufen
       * Starten Sie die Suche und zeigen Sie Textdokumente an, wenn Sie welche finden
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "Kombinieren Sie Suchdokumentfilter, um einen zusammengesetzten Filter über Java zu erstellen"
      content_left: |
        GroupDocs.Search for Java ermöglicht Softwareprogrammierern, erweiterte Suchfunktionen hinzuzufügen und benutzerdefinierte Filter für die Dokumentensuche in ihrer Java-Anwendung anzuwenden. Benutzer können zusammengesetzte Filter erstellen, indem sie verschiedene Arten von Suchfiltern kombinieren. Der folgende Java-Code zeigt, wie Suchdokumentfilter kombiniert werden, um zusammengesetzte Filter mit booleschen Operatoren UND, ODER, NICHT usw. mit nur wenigen Codezeilen zu erstellen.

      title_right: "Erstellen Sie einen zusammengesetzten Filter, um ZIP-Dateien zu durchsuchen"
      content_right: |
       * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
       * Erstellen eines UND-Verbundfilters, der alle FB2- und EPUB-Dokumente zurückgibt, die das Wort „Einstein“ in ihren vollständigen Pfaden enthalten
       * Filter1 erstellen durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Erstellen Sie filter2 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Kombinieren Sie Filter, indem Sie die Methode [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...)) aufrufen
       * Erstellen Sie einen zusammengesetzten OR-Filter, der alle DOC-, DOCX-, PDF- und alle Dokumente zurückgibt, die das Wort Einstein in ihren vollständigen Pfaden enthalten
       * Erstellen Sie filter3 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Erstellen Sie filter4 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Kombinieren Sie Filter, indem Sie die Methode [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...)) aufrufen
       * Erstellen eines Filters, der alle gefundenen Dokumente mit Ausnahme von TXT-Dokumenten zurückgibt
       * Erstellen Sie filter4 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Appy Not-Filter durch Aufrufen der Methode [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter)).

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
    - title_left: "System Anforderungen"
      content_left: |
       GroupDocs.Search für Java wird auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Um den vollständigen Leitfaden zu den Systemanforderungen zu erhalten, besuchen Sie bitte [Systemanforderungen](https://docs.groupdocs.com/search/java/system-requirements/), bevor Sie den folgenden Code ausführen. Stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem installiert sind System:
         * Betriebssysteme: Microsoft Windows, Linux, MacOS
         * Unterstützung für Java-Versionen: J2SE 7.0 (1.7), J2SE 8.0 (1.8) oder höher
         * Holen Sie sich die neueste Version von GroupDocs.Search für Java-APIs von GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "Warum GroupDocs.Search verwenden?"
      content_right: |
        * Suchindexerstellung sowohl im Speicher als auch auf der Festplatte.
        * Möglichkeit der Indizierung aus einer Datei, einem Stream oder einer Struktur.
        * Unterstützung für die Indexierung passwortgeschützter Dokumente.
        * Unterstützung für das Zusammenführen mehrerer Indizes.
        * Dokument während der Suchindizierung filtern.
        * Unterstützung der Rechtschreibprüfung während der Suche.
        * Mischzeichen werden vollständig unterstützt
        * Kombinieren verschiedener Suchtypen in einer Suchanfrage.
        * Einfache Suche nach Wörtern und regulären Ausdrücken wird unterstützt
        * Vollständige Unterstützung von Alias-Ersetzungen in Suchanfragen.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---