---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/net/boolean/pptx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Fügen Sie boolesche Suchoperatoren (AND, OR, NOT) in Suchanfragen über .NET hinzu"
head_description: "GroupDocs.Search .NET API ermöglicht es Softwareentwicklern, boolesche Suchen hinzuzufügen oder neue Abfragen mit booleschen Operatoren UND, ODER, NICHT in ihren .NET-Apps zu entwickeln."

############################# Header ############################
title: "Entwickeln Sie komplexe Suchabfragen mit booleschen Operatoren UND, ODER, NICHT in .NET-Apps"
description: "GroupDocs.Search .NET API ermöglicht Computerprogrammierern komplexe Suchabfragen mit booleschen Operatoren (AND, OR, NOT) in ihren .NET-Anwendungen zu entwickeln. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Was ist eine boolesche Suche und wie werden boolesche Operatoren verwendet?"
    content: |
       Die boolesche Suche ist ein sehr nützliches Suchverfahren, das es Benutzern ermöglicht, verschiedene Schlüsselwörter mit Operatoren zu kombinieren, um die Suchergebnisse einzugrenzen, zu erweitern und zu definieren. Boolesche Operatoren wie AND, OR, NOT und NEAR usw. helfen Benutzern, ein breiteres Spektrum an Ergebnissen zu erhalten oder die Anzahl nicht zusammenhängender Suchergebnisse zu reduzieren, indem sie Einschränkungen definieren. GroupDocs.Search für .NET ist eine leistungsstarke Hochleistungs-API für die Dokumentensuche, die es Softwareentwicklern ermöglicht, Anwendungen zu entwickeln, die eine Textsuche und Indizierung in einigen der gängigsten Dokumentdateiformate wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word und Excel-Arbeitsblättern durchführen können , PowerPoint-Präsentationen, Outlook MSG, PST und viele mehr. Der boolesche UND-Operator kann verwendet werden, um Ergebnisse für alle von Ihnen eingegebenen Wörter anzuzeigen, der ODER-Operator liefert Ergebnisse für jedes der von Ihnen eingegebenen Wörter, der NICHT-Operator kann verwendet werden, um Suchergebnisse für kein Vorkommen anzuzeigen und so weiter. Eine großartige Funktion ist, dass es Suchanfragen erkennen kann, die in einer Sprache geschrieben sind, die nicht mit Ihrem Tastaturlayout übereinstimmt. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Verwenden Sie den booleschen UND-Operator in Suchanfragen über .NET"
      content_left: |
       GroupDocs.Search .NET API bietet vollständige Unterstützung für das Hinzufügen von booleschen Suchfunktionen in ihre .NET-Anwendung. Das folgende C#-Codebeispiel zeigt, wie der boolesche „AND“-Operator in Text- und Objektformabfragen in eigenen .NET-Anwendungen erstellt wird. 

      title_right: "Durchsuchen Sie PPTX Dokumente mit dem booleschen Operator AND"
      content_right: |
         * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
         * Erstellen eines Index im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
         * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
         * Erstellen von Unterabfrage 1 und Erstellen von Unterabfrage 2 durch Aufrufen der Klasse [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery).
         * Kombinieren von Unterabfragen zu einer Abfrage durch Aufrufen der Methode [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
         * Suche starten und Suchergebnisse anzeigen
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "So verwenden Sie den booleschen Operator ODER über .NET"
      content_left: |
       GroupDocs.Search für .NET ist eine leistungsstarke API, mit der Softwareprogrammierer viele gängige Dokumentformate durchsuchen können. Die folgenden C# .NET-Codebeispiele zeigen, wie der boolesche „ODER“-Operator in Text- und Objektformularabfragen in C#-Anwendungen verwendet wird. 

      title_right: "Verwenden Sie den booleschen OR-Operator, um PPTX-Dateien zu durchsuchen"
      content_right: |
        * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
        * Erstellen eines Index im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
        * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
        * Erstellen von Unterabfrage 1 und Erstellen von Unterabfrage 2 durch Aufrufen der Klasse [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery).
        * Kombinieren von Unterabfragen zu einer Abfrage durch Aufrufen der Methode [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery).
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "Erstellen Sie komplexe Suchanfragen mit booleschen Operatoren"
      content_left: |
        GroupDocs.Search .NET ermöglicht Computerprogrammierern, verschiedene boolesche Operatoren zu kombinieren, um komplexe Suchabfragen in ihren eigenen .NET-Apps zu erstellen. Die folgenden .NET-Codebeispiele zeigen, wie Sie Suchfunktionen für komplexe Dokumente nutzen können, ohne externe Software oder Tools zu installieren.

      title_right: "Durchsuchen Sie PPTX Dokumente über komplexe Suchanfragen"
      content_right: |
        * Zuerst müssen Sie den Pfad zum Indexordner und Dokumentenordner angeben.
        * Erstellen eines Index im angegebenen Ordner durch Aufrufen der Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
        * Indexieren von Dokumenten aus dem angegebenen Ordner durch Aufrufen der Methode [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
        * Starten Sie die Suche und zeigen Sie die Textabfrage der Suchergebnisse an
        * Suche mit Objektabfrage
        * Erstellen von WordQuery und relativityWordQuery durch Aufrufen der Klasse [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery).
        * Kombinieren von Unterabfragen zu einer Abfrage durch Aufrufen der Methode [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search).
        * Erstellen von einsteinWordQuery und albertWordQuery durch Aufrufen der Klasse [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery).
        * Kombinieren von Unterabfragen zu einer Abfrage durch Aufrufen der Methode [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery).
        * Kombinieren von Unterabfragen zu einer Abfrage durch Aufrufen der Methode [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery).
        * Suche starten und Suchergebnisse anzeigen
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

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