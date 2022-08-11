---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/net/filters/pps/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Passen Sie die Suchergebnisse an, indem Sie die Dokumentfilterung in .NET-Apps festlegen"
head_description: "GroupDocs.Search .NET API ermöglicht Softwareentwicklern, PPS Documents-Dokumente zu durchsuchen und die Suchergebnisse anzupassen, indem sie die Dokumentfilterung in .NET-Apps anwenden."

############################# Header ############################
title: "Legen Sie die Dokumentfilterung fest, um Suchergebnisse in .NET-Apps anzupassen"
description: "Die .NET-API von GroupDocs.Search hilft Softwarefachleuten, Suchfunktionen für Dokumente hinzuzufügen und Suchergebnisse anzupassen, indem sie die Dokumentfilterung in ihren .NET-Apps anwenden."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Wie wende ich die Dokumentfilterung im Suchergebnis über .NET an?"
    content: |
      Das Filtern ist eine sehr nützliche Technik, mit der Benutzer die Funktionalität überprüfen und verarbeiten können. Die Dokumentenfilterung bietet Benutzern eine einfache Möglichkeit, durch ihre Ergebnisse zu navigieren und zu finden, wonach sie suchen. Es gibt Benutzern auch die Möglichkeit, ihre Suche auf einen bestimmten Abschnitt oder einen bestimmten Dokumenttyp zu beschränken. GroupDocs.Search für .NET ist eine funktionsreiche Hochleistungs-API für die Dokumentensuche, die es Softwareentwicklern ermöglicht, Anwendungen zu erstellen, die eine Textsuche und Indexierung ermöglichen. Es unterstützt einige der gängigsten Dokumentenformate wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblätter, PowerPoint-Präsentationen, Outlook MSG, PST und viele mehr. Die API unterstützt die Einstellung der Dokumentenablage für Suchergebnisse vollständig. Sie können verschiedene Arten von Filern verwenden, um Ihre Suchergebnisse anzupassen, z. B. Dateipfadfilter, Dateierweiterungsfilter, Attributfilter und viele mehr. Es ist auch möglich, Suchdokumentfilter zu kombinieren, indem Sie die booleschen Operatoren AND, OR & NOT usw. verwenden.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Legen Sie den Dokumentfilter bei der Suche nach PPS-Dokumenten über .NET fest"
      content_left: |
       GroupDocs.Search .NET API hilft Softwareentwicklern, Suchfunktionen in ihre .NET-Anwendung einzufügen. Das folgende .NET-Codebeispiel zeigt, wie Dokumentfilter beim Durchsuchen verschiedener Arten von Dokumenten mit nur wenigen Codezeilen angewendet werden.

      title_right: "Dokumentfilter beim Durchsuchen von PPS Dokumenten anwenden"
      content_right: |
       * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
        * Erstellen eines Index im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
        * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
        * Erstellen eines Suchoptionsobjekts [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
        * Dokumentfilter durch Aufruf von [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) setzen
        * Suche starten und Suchergebnisse anzeigen
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: "So kombinieren Sie Suchdokumentfilter über .NET"
      content_left: |
        GroupDocs.Search for .NET ermöglicht Softwareprogrammierern, Suchdokumentfilter während der Suche zu kombinieren, um zu steuern, welche der gefundenen Dokumente als Ergebnis der Suche in der C# .NET-Anwendung zurückgegeben werden sollen. Die folgenden .NET-Codebeispiele zeigen, wie Suchdokumentfilter mit booleschen Operatoren AND, OR, NOT usw. in C#-Anwendungen kombiniert werden. 

      title_right: "Kombinieren Sie Suchdokumentfilter beim Durchsuchen von PPS-Dateien"
      content_right: |
       * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
       * Erstellen eines UND-Verbundfilters, der alle FB2- und EPUB-Dokumente zurückgibt, die das Wort „Einstein“ in ihren vollständigen Pfaden enthalten
       * Filter1 erstellen durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Erstellen Sie filter2 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Kombinieren Sie Filter, indem Sie die Methode [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand) aufrufen
       * Erstellen eines zusammengesetzten ODER-Filters, der alle DOC-, DOCX-, PDF- und alle Dokumente zurückgibt, die das Wort Einstein in ihren vollständigen Pfaden enthalten
       * Erstellen Sie filter3 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Erstellen Sie filter4 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Kombinieren Sie Filter, indem Sie die Methode [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor) aufrufen
       * Erstellen eines Filters, der alle gefundenen Dokumente mit Ausnahme von TXT-Dokumenten zurückgibt
       * Erstellen Sie filter4 durch Aufrufen von [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Filtern Sie nicht, indem Sie die Methode [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot) aufrufen

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
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