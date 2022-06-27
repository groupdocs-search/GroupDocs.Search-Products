---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "de/search/net/document/chm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MD EPUB  FB2 

############################# Head ############################
head_title: "Erstellen und Hinzufügen von Dokumenten Suchen und Indizieren in .NET-Anwendungen"
head_description: "GroupDocs.Search .NET API ermöglicht das sofortige Hinzufügen von Dokumenten durch die Suche nach unterstützenden Formaten wie PDF DOC, DOCX, RTF, XLSX, CSV, PPTX und E-Mail-Nachrichten in .NET Apps."

############################# Header ############################
title: "So fügen Sie die Instant Documents Search über die C# .NET API zu CHM hinzu "
description: "GroupDocs.Search .NET API ermöglicht es Entwicklern, ihren Apps robuste Funktionen zum Suchen und Indexieren von Dokumenten hinzuzufügen. Es unterstützt Dokumente wie PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, MSG, EML und viele mehr."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Wie erstelle und füge ich Dokumente zum Suchen und Indizieren mit der .NET-API hinzu?"
    content: |
       Auf dieser Seite erfahren Benutzer, wie sie mit geringem Aufwand und geringen Kosten Funktionen zum Suchen und Indizieren von Dokumenten in ihre eigenen Anwendungen einfügen können. Indizierung ist der Prozess, der von Suchmaschinen verwendet wird, mit dem die Daten organisiert und strukturiert werden, damit sie relevante Suchergebnisse generieren können. Ziel ist es, Informationen zu Benutzeranfragen schnell und genau zu finden und anzuzeigen. GroupDocs.Search für .NET ist eine leistungsstarke API für die Dokumentensuche, die es Softwareentwicklern ermöglicht, erweiterte Such- und Indizierungsvorgänge auf der Grundlage von Fuzzy- und Synonymalgorithmen in ihren eigenen Anwendungen durchzuführen. Es muss kein Tool von Drittanbietern oder externe Software auf dem Computer des Benutzers installiert werden. Es bietet Unterstützung für einige der am häufigsten verwendeten Dokumentformate wie PDF, HTML, Outlook-E-Mail, Microsoft Office Word, Excel-Arbeitsblätter, PowerPoint-Präsentationen, Outlook MSG, PST und viele mehr. Es unterstützt verschiedene Arten von Suchen, wie z. B. einfache Wortsuche, boolesche Suche, Suche nach regulären Ausdrücken, Suche nach Groß- und Kleinschreibung, flexible Fuzzy-Suche, Synonyme, Homophone, Platzhalter, Suche nach Blöcken, Suche nach Objekttypen, Festlegen des Datenbereichs und so weiter. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Suchindexerstellung für CHM Document über .NET API"
      content_left: |
       GroupDocs.Search .NET API bietet vollständige Unterstützung für das Erstellen neuer Indizes oder das Öffnen vorhandener Suchindizes in Ihren eigenen Apps. Das folgende C#-Codebeispiel zeigt, wie Sie mit nur wenigen Codezeilen einen neuen Index erstellen und einen vorhandenen Index öffnen. 

      title_right: "So erstellen Sie einen neuen oder öffnen einen vorhandenen Suchindex"
      content_right: |
         * Zuerst müssen Sie den Pfad zum Indexordner angeben
         * Erstellen Sie eine Instanz der Klasse [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2).
         * Oben erstellt einen Index im Speicher oder auf einer Festplatte und kann auch einen vorhandenen Index öffnen.
       
      gisthash: "9651c19a9436afee860b7f39197f8399"
      gistfile: "create_or_open_new_search_index.cs"

    - title_left: "So fügen Sie CHM Dokumente synchron zum Suchindex hinzu"
      content_left: |
       GroupDocs.Search .NET ermöglicht es Softwareentwicklern, die Indexierung von Dokumenten synchron in ihren eigenen .NET-Apps durchzuführen. Die folgenden C# .NET-Codebeispiele zeigen, wie die Indizierung problemlos synchron durchgeführt werden kann. 

      title_right: "Synchrone Indexierung von Dokumenten über C#"
      content_right: |
        * Zuerst müssen Sie den Pfad zum Indexordner angeben
        * Geben Sie den Pfad zu einem Ordner an, der zu durchsuchende Dokumente enthält
        * Erstellen Sie eine Instanz der Klasse [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2).
        * Oben erstellt einen Index im Speicher oder auf einer Festplatte oder öffnet einen bestehenden Index.
        * Synchrone Indizierung von Dokumenten aus dem angegebenen Ordner
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_synchronously_to_indexing.cs"
      
    - title_left: "Führen Sie die Dokumentenindizierung asynchron über .NET durch"
      content_left: |
        GroupDocs.Search .NET ermöglicht Computerprogrammierern die asynchrone Indexierung von Dokumenten innerhalb ihrer eigenen .NET-Apps. Die folgenden .NET-Codebeispiele zeigen, wie Sie mit nur wenigen Codezeilen eine asynchrone Indexierung von Dokumenten erreichen.

      title_right: "Asynchrone CHM Dokumentindizierung über C#"
      content_right: |
        * Zuerst müssen Sie den Pfad zum Indexordner angeben
        * Geben Sie den Pfad zu einem Ordner an, der zu durchsuchende Dokumente enthält
        * Erstellen Sie eine Instanz der Klasse [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2).
        * Abonnieren der Veranstaltung
        * Es muss ein Code geschrieben werden, der den Abschluss der Operation angibt
        * Setzen des Flags für asynchrone Indizierung
        * Asynchrone Indizierung von Dokumenten aus dem angegebenen Ordner
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_asynchronously_to_indexing.cs"

    - title_left: "So verwenden und markieren Sie Suchergebnisse in CHM Docs .NET"
      content_left: |
       GroupDocs.Search .NET API ermöglicht Programmierern, ein Suchergebnis zu interpretieren und die Ergebnisse anhand einer einfachen Liste der gefundenen Dokumente oder der gefundenen Wörter und Phrasen anzuzeigen. Sie können den Text des Dokuments auch ganz einfach hervorheben. Die folgenden .NET-Codebeispiele zeigen, wie gefundene Dokumente aufgelistet und Suchergebnisse mit nur wenigen Codezeilen hervorgehoben werden.

      title_right: "Suchergebnisse in CHM-Dateien über C# hervorheben "
      content_right: |
        * Suche im Index durchführen
        * Drucken Sie nach erfolgreicher Suche das Ergebnis aus
        * Iterieren Sie durch die Dokumente und zeigen Sie die gefundenen Dokumente an
        * Hervorhebung von Vorkommen im Text
        * Generieren von Ausgabedokumenten im HTML-Format mit hervorgehobenen Suchergebnissen
     
      gisthash: "a5d1ad6eedd2acf12a33b541e763cdb4"
      gistfile: "how_to_list_search_result.cs"

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