---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/net/phrase/potx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Wie füge ich eine Wortgruppensuche in POTX-Dokumenten in .NET-Apps hinzu?"
head_description: "Die .NET-API von GroupDocs.Search ermöglicht es Softwarefachleuten, eine Wortgruppensuche hinzuzufügen und die genaue Wortgruppe oder die bereitgestellte Wortfolge in POTX-Dokumenten über die .NET-API zu finden."

############################# Header ############################
title: "Genauen Satz oder Wortgruppe hinzufügen Suche in POTX Dokumenten in .NET Apps?"
description: "Die .NET-API von GroupDocs.Search ermöglicht es Programmierern, die bereitgestellte Wortfolge in POTX-Dokumenten über die Wortgruppensuche oder Suche nach genauen Sätzen in .NET-Apps herauszufinden."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Wie verwende ich die Suche nach genauen Sätzen oder Ausdrücken in .NET-Apps?"
    content: |
       Die Suche nach genauen Sätzen oder Ausdrücken ist eine Art von Suche, die es Benutzern ermöglicht, Dokumente, Web oder Datenbanken mit einem genauen Satz oder Ausdruck zu durchsuchen, der eine bestimmte Reihenfolge und Kombination von Wörtern enthält, die von den Verbrauchern definiert wurden. Es ist ein sehr gebräuchlicher Begriff in der Suchmaschinenterminologie und ermöglicht es Benutzern, Dokumente nach einer bestimmten Wortfolge im Text von indizierten Dokumenten zu suchen. GroupDocs.Search für .NET ist eine sehr nützliche Hochleistungs-API für die Dokumenten- und Textsuche, die vollständige Funktionalität für die Entwicklung von Anwendungen für die Textsuche und Indexierung bietet und einige der gängigsten Dokumenttypen wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblätter, PowerPoint-Präsentationen, Outlook MSG, PST und so weiter. Es hat Unterstützung für mehrere Funktionen im Zusammenhang mit der Phrasensuche enthalten, wie z. B. die Suche nach Abfragen in Text- und Objektform, die Verwendung von Platzhaltern bei der Phrasensuche und so weiter.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "So führen Sie eine Wortgruppensuche in POTX-Dokumenten über .NET durch"
      content_left: |
       GroupDocs.Search .NET API ermöglicht Softwareentwicklern das Hinzufügen von Phrasensuchfunktionen in ihre eigene C# .NET-Anwendung. Das folgende .NET-Codebeispiel zeigt, wie Sie mit nur wenigen Codezeilen eine Wortgruppensuche in Text und Objekt durchführen.

      title_right: "Suche nach exakten Ausdrücken in POTX Dokumenten"
      content_right: |
         * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
         * Erstellen eines Index im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
         * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
         * Suchen Sie nach der Phrasenabfrage „Phrasentext“ in Textform
         * Suchen Sie nach dem Ausdruck „Phrasentext“ in Objektform
         * Erstellen von Wort1, Wort2 und Unterabfrage 3 durch Aufrufen der Methode [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery).
         * Kombinieren von Unterabfragen zum Erstellen einer neuen Suchabfrage durch Aufrufen der Methode [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery).
         * Suche starten und Suchergebnisse anzeigen
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: "Wildcard-Phrasensuche in POTX-Dokumenten über .NET"
      content_left: |
        GroupDocs.Search für .NET ermöglicht Softwareprogrammierern das Hinzufügen von Phrasensuchfunktionen mithilfe von Platzhaltern innerhalb der C# .NET-Anwendung. Die folgenden .NET-Codebeispiele zeigen, wie die Platzhalter-Phrasensuche in POTX-Dokumenten in C#-Anwendungen angewendet wird.

      title_right: "Wenden Sie die Wildcard-Phrasensuche in der Datei POTX an"
      content_right: |
        * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
        * Indexerstellung im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
        * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
        * Suchen Sie nach der Phrasenabfrage „Phrasentext“ in Textform
        * Suchen Sie nach dem Ausdruck „Phrasentext“ in Objektform
        * Erstellen von Wort1 und Unterabfrage 3 durch Aufrufen der Methode [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery).
        * Erstellen von Wildcard2 durch Aufrufen der Methode [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1).
        * Kombinieren von Unterabfragen zum Erstellen einer neuen Suchabfrage durch Aufrufen der Methode [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery).
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: "Kombinieren Sie die Phrasensuche mit anderen Suchtypen über .NET"
      content_left: |
        GroupDocs.Search .NET gibt Softwareprogrammierern die Möglichkeit, die Wortgruppensuche mit anderen Suchtypen innerhalb der .NET-Anwendung zu kombinieren. Die folgenden .NET-Codebeispiele zeigen, wie sowohl Platzhalter für Wörter als auch Zeichen in Wörtern angewendet werden.

      title_right: ".NET-API zum Kombinieren der Phrasensuche mit anderen Suchen"
      content_right: |
        * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
        * Indexerstellung im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
        * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
        * Suche nach dem Ausdruck in Textform
        * Suche nach dem Ausdruck in Objektform
        * Wortmuster definieren und Zeichenfolge anhängen.
        * Erstellen von WordPattern1 und Erstellen von Word3 durch Aufrufen der Methode [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery).
        * Erstellen von Wildcard2 durch Aufrufen der Methode [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1).
        * Kombinieren von Unterabfragen zum Erstellen einer neuen Suchabfrage durch Aufrufen der Methode [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery).
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

    - title_left: "System Anforderungen"
      content_left: |
       GroupDocs.Search für .NET wird auf allen wichtigen Plattformen und Betriebssystemen unterstützt. Um den vollständigen Leitfaden zu den Systemanforderungen zu erhalten, besuchen Sie bitte [Systemanforderungen](https://docs.groupdocs.com/search/net/system-requirements/), bevor Sie den folgenden Code ausführen. Stellen Sie bitte sicher, dass die folgenden Voraussetzungen auf Ihrem installiert sind System:
         * Betriebssysteme: Microsoft Windows, Linux, MacOS
         * Entwicklungsumgebung: Visual Studio, Xamarin, MonoDevelop usw
         * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
         * Holen Sie sich die neueste Version von GroupDocs.Search für .NET-APIs von [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
      title_right: "Warum GroupDocs.Assembly verwenden"
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