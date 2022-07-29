---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/net/case-sensitive/xlt/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Wenden Sie die Textsuche mit Berücksichtigung der Groß-/Kleinschreibung in XLT-Dokumenten über .NET an"
head_description: "Die .NET-API von GroupDocs.Search ermöglicht es Softwareprogrammierern, die Textsuche mit Berücksichtigung der Groß-/Kleinschreibung anzuwenden und die genaue Wortfolge in XLT-Dokumenten über die .NET-API zu finden."

############################# Header ############################
title: "Wie wende ich die Suche mit Berücksichtigung der Groß- und Kleinschreibung in XLT-Dokumenten in .NET-Apps an?"
description: "Die .NET-API von GroupDocs.Search ermöglicht Softwareentwicklern die Textsuche mit Berücksichtigung der Groß- und Kleinschreibung in verschiedenen Dokumenttypen wie PDF, HTML, DOCX, PPTX, XLSX und mehr in .NET-Apps."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Was ist die Suche mit Berücksichtigung der Groß-/Kleinschreibung und wie wird sie über .NET erreicht?"
    content: |
      Es gibt zahlreiche nützliche Suchtechniken, die Benutzern helfen können, verschiedene Arten von Dokumenten nach einer bestimmten Kombination von Wörtern oder anderen Daten zu durchsuchen. Case-Sensitive Search ist eine sehr nützliche Technik, die es Benutzern ermöglicht, Dokumente und Webseiten zu durchsuchen, unabhängig davon, ob Groß- und Kleinbuchstaben als unterschiedlich oder gleich behandelt werden. Beispielsweise werden „Computer“, „Computer“ und „COMPUTER“ als unterschiedliche Wörter behandelt, da der Buchstabe „C“ in erster Instanz großgeschrieben, in zweiter Instanz kleingeschrieben und in dritter Instanz ausschließlich in Großbuchstaben geschrieben wird. GroupDocs.Search für .NET ist eine praktische Hochleistungs-API für die Dokumentensuche, die es Softwareentwicklern ermöglicht, Softwareanwendungen und Tools für die Textsuche sowie die Indexierung von Dokumenten mit Leichtigkeit zu erstellen. Die API bietet Unterstützung für einige der am häufigsten verwendeten Dateiformate wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblätter, PowerPoint-Präsentationen, Outlook MSG, PST und viele mehr. Eine weitere nützliche Funktion ist, dass Suchanfragen identifiziert werden können, die in einer Sprache geschrieben sind, die nicht mit Ihrem Tastaturlayout übereinstimmt.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Führen Sie eine Suche mit Berücksichtigung der Groß- und Kleinschreibung in XLT-Dokumenten über .NET durch"
      content_left: |
       GroupDocs.Search .NET API ermöglicht Softwareprogrammierern, Suchfunktionen mit Berücksichtigung der Groß- und Kleinschreibung in ihre eigene C# .NET-Anwendung einzufügen. Das folgende .NET-Codebeispiel veranschaulicht, wie Sie mit nur wenigen Codezeilen eine Suche mit Berücksichtigung der Groß-/Kleinschreibung mit einer Abfrage in Textform in XLT-Dateien erreichen.

      title_right: "Wenden Sie die Suche mit Berücksichtigung der Groß-/Kleinschreibung in XLT Dokumenten an"
      content_right: |
         * Identifizieren Sie den Pfad zum Indexordner sowie zum Dokumentenordner.
         * Generieren Sie einen Index im angegebenen Ordner, indem Sie eine Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) aufrufen
         * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Instanz der Klasse [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1).
         * Initialisiert eine neue Instanz der Klasse [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
         * Aktivieren der Suche mit Berücksichtigung der Groß-/Kleinschreibungb durch Aufrufen der Methode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch).
         * Suchstring definieren und Suche starten
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: "Führen Sie eine Suche mit Berücksichtigung der Groß- und Kleinschreibung in Objektform über .NET durch"
      content_left: |
        GroupDocs.Search .NET gibt Softwareentwicklern die Möglichkeit, Wörter zu finden, die Groß- und Kleinbuchstaben in .NET-Anwendungen berücksichtigen. Das folgende .NET-Codebeispiel veranschaulicht, wie die Suche mit Berücksichtigung der Groß-/Kleinschreibung mit einer Abfrage in Objektform in XLT-Dokumenten angewendet wird. 

      title_right: "Suchen Sie in XLT Dokumenten nach Groß- und Kleinschreibung"
      content_right: |
        * Identifizieren Sie den Pfad zum Indexordner sowie zum Dokumentenordner.
        * Generieren Sie einen Index im angegebenen Ordner, indem Sie eine Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) aufrufen
        * Indizieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Instanz der Klasse [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1).
        * Initialisiert eine neue Instanz der Klasse [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions).
        * Aktivieren der Suche mit Berücksichtigung der Groß-/Kleinschreibungb durch Aufrufen der Methode [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch).
        * Erstellen einer Suchabfrage in Objektform durch Aufrufen der Methode [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery).
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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