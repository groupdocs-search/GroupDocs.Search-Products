---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/java/boolean/rtf/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB12 

############################# Head ############################
head_title: "Java-API zum Suchen und Finden exakter Ausdrücke in RTF-Dokumenten"
head_description: "Die Java-API von GroupDocs.Search hilft Programmierern, die Wortgruppensuche einzubetten und eine bestimmte Folge von Wörtern oder eine exakte Wortgruppe im Text von RTF-Dokumenten über Java zu entdecken."

############################# Header ############################
title: "Wie kann ich über die Java-API nach genauen Sätzen oder Ausdrücken in RTF-Dokumenten suchen und diese anzeigen?"
description: "GroupDocs.Search Java API hat vollständige Unterstützung für erweiterte Suchfunktionen bereitgestellt, die es Softwareentwicklern ermöglichen, exakte Sätze oder Ausdrücke in RTF-Dokumenten über die Suche nach Ausdrücken oder exakten Sätzen zu suchen."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Was ist die Phrasensuche und wie wird sie in Java-Apps verwendet?"
    content: |
       Die Wortgruppensuche ist eine sehr effektive Methode, um in Dokumenten oder Webseiten nach einem genauen Satz oder einer Wortgruppe statt nach einem Schlüsselwort zu suchen. Das bedeutet, wenn Benutzer nach einem genauen Ausdruck suchen, möchten sie alle Suchbegriffe in der bestimmten Reihenfolge finden, in der sie erschienen sind. Auf dieser Webseite werden Informationen darüber weitergegeben, wie Benutzer Geschäftsanwendungen und Tools für die effiziente Suche nach Dokumenten und Webseiten mithilfe der Java-API entwickeln können. GroupDocs.Search für Java ist eine sehr gut organisierte und effiziente Java-API, die es Softwareentwicklern ermöglicht, einfache bis fortgeschrittene Textsuchoperationen in ihren eigenen Apps durchzuführen, ohne Software von Drittanbietern zu installieren. Die API enthält zahlreiche wertvolle Funktionen für die Dokumentensuche, wie z. B. einfache oder boolesche Suche, Fuzzy-Suche, Suche mit Berücksichtigung der Groß-/Kleinschreibung, Synonyme, Homophone, Platzhalter, Objekttypsuche, Festlegen des Datenbereichs und andere Arten von Abfragen, um Informationen schnell und elegant zu finden. Darüber hinaus unterstützt es auch die Erkennung von Suchanfragen, die in einer Sprache verfasst sind, die nicht zu Ihrem Tastaturlayout passt.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Führen Sie eine Wortgruppensuche in RTF-Dokumenten über Java durch"
      content_left: |
       Die Java-API von GroupDocs.Search bietet vollständige Unterstützung für erweiterte Suchfunktionen, die es Softwareexperten ermöglichen, leistungsstarke Softwareanwendungen mit Suchfunktionen und Benutzerfreundlichkeit zu erstellen. Der folgende Java-Code zeigt, wie Sie mit nur wenigen Codezeilen eine Phrasensuche in Text- und Objektform durchführen.

      title_right: "Exakte Satzsuche in RTF Dateien"
      content_right: |
         * Pfad zum Indexordner & Dokumentenordner definieren.
         * Erstellen eines Indexes im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)).
         * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)).
         * Suche mit Textabfrage durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)).
         * Suchen Sie nach dem Ausdruck „Phrasentext“ in Objektform
         * Erstellen von Wort1, Wort2 und Unterabfrage 3 durch Aufrufen der Methode [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)).
         * Kombinieren von Unterabfragen zum Erstellen einer neuen Suchabfrage durch Aufrufen von [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) Methode
         * Suche starten und Suchergebnisse anzeigen
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "Wenden Sie die Wildcard-Phrasensuche durch RTF-Dateien über Java an"
      content_left: |
        GroupDocs.Search für Java gibt Software-Programmierern die Möglichkeit, Platzhalter-Suchfunktionen hinzuzufügen, während sie RTF-Dateien in der Java-Anwendung durchsuchen. Die folgenden Java-Codebeispiele demonstrieren, wie die Platzhalter-Phrasensuche in verschiedenen Dokumenttypen mithilfe der Java-API angewendet wird. 

      title_right: "Phrasensuche mit Platzhaltern in Java"
      content_right: |
        * Pfad zum Indexordner & Dokumentenordner definieren.
        * Erstellen eines Indexes im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)).
        * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)).
        * Suche mit Textabfrage durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)).
        * Suchen Sie nach dem Ausdruck „Phrasentext“ in Objektform
        * Erstellen von Wort1 und Wort3 durch Aufrufen der Methode [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)).
        * Erstellen von Wildcard2 durch Aufrufen der Methode [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)).
        * Kombinieren von Unterabfragen zum Erstellen einer neuen Phrasensuchabfrage durch Aufrufen von [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) Methode
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "Java-API zur Kombination von Phrasensuche und anderen Suchtypen"
      content_left: |
        Die Java-API von GroupDocs.Search ermöglicht es Softwareprogrammierern, die Wortgruppensuche mühelos mit anderen Suchtypen zu kombinieren. Der folgende Java-Code zeigt, wie eine Wortgruppensuche über Platzhalter durchgeführt wird, die Wörter und Zeichen in Wörtern darstellen.

      title_right: "So kombinieren Sie die Phrasensuche und andere Suchen"
      content_right: |
        * Pfad zum Indexordner & Dokumentenordner definieren.
        * Erstellen eines Indexes im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)).
        * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)).
        * Suche mit Textabfrage durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)).
        * Suchen Sie nach dem Ausdruck „Phrasentext“ in Objektform
        * Wortmuster definieren und String anhängen & Wildcard anhängen
        * Erstellen von WordPattern1 und Erstellen von Word3 durch Aufrufen der Methode [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern)).
        * Erstellen von Wildcard2 durch Aufrufen der Methode [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)).
        * Kombinieren von Unterabfragen zum Erstellen einer neuen Phrasensuchabfrage durch Aufrufen von [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) Methode
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

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