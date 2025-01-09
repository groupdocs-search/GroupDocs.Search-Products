---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: en
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET Document Search and Indexing Library for PDFs, Office Files, and More"
head_description: "Powerful .NET solution for text search and indexing in documents like PDFs, Word, Excel, presentations, emails, and web formats."

############################# Header ############################
title: "Advanced Document Search and Indexing with .NET API"
description: "Boost .NET applications with cutting-edge text search capabilities across popular document formats."
words:
  for: "for"

actions:
  main: "Download Nuget for Free"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Start Your Journey Today!"
  description: "Explore the capabilities of GroupDocs.Search for free or secure a license to unlock its full potential."

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Search Text in Directory Files"
  more: "More examples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Create an index for your documents
    Index index = new Index("c:/MyIndex");

    // Add documents to the index for efficient searching
    index.Add("c:/MyDocuments");
    
    // Search for specific words or phrases, such as
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Overview"
  description: "Explore .NET C# library for robust text search and indexing."
  features:
    # feature loop
    - title: ".NET Indexing and Search Features"
      content: "Efficiently index, store, and process document data with GroupDocs.Search for .NET for highly accurate and fast search operations."

    # feature loop
    - title: "Combine Indexes for Better Search Speed"
      content: "GroupDocs.Search for .NET lets you merge multiple indexes to optimize performance. Reduce the impact of delta indexes by combining them into a comprehensive index for smoother searches."

    # feature loop
    - title: "Search Across Different Keyboard Layouts"
      content: "Easily handle search queries across 88 languages and 164 keyboard layouts with GroupDocs.Search for .NET’s intelligent recognition."

    # feature loop
    - title: "Morphological Word Searches"
      content: "GroupDocs.Search for .NET supports searches for word variations like singular/plural nouns and different verb forms, customizable for various languages."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Search for .NET works seamlessly across major operating systems and package managers."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    Process an extensive range of file formats with GroupDocs.Search for .NET. [View all supported formats](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Popular Office Formats
        * **Portable:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Text:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Media Formats
        * **Popular image formats:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Multi-page images:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Video:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Other
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Others:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Key Features of GroupDocs.Search for .NET"
  description: "Streamline document management with advanced search capabilities in popular formats like PDF, DOCX, XLSX, PPTX, and more."

  items:
    # feature loop
    - icon: "document_info"
      title: "Flexible Search Parameters"
      content: "Use filters like date ranges and case sensitivity to refine your search."

    # feature loop
    - icon: "detect"
      title: "Smart Spell Check"
      content: "Search phrases with spell correction, wildcards, and ignored special characters."

    # feature loop
    - icon: "collect"
      title: "Filtered Search Results"
      content: "Customize and filter search results by document type or criteria."

    # feature loop
    - icon: "get"
      title: "Index Import & Export"
      content: "Import data, modify indexing settings, and export indexed results."

    # feature loop
    - icon: "remove"
      title: "Exclude Irrelevant Data"
      content: "Optimize indexing by skipping specific files or words."

    # feature loop
    - icon: "style"
      title: "URL Extraction"
      content: "Convert HTML-formatted text to files and generate links for search results."

    # feature loop
    - icon: "detect"
      title: "High-Speed Search"
      content: "Divide large indexes into smaller parts for faster processing."

    # feature loop
    - icon: "manipulate"
      title: "Streamlined Data Handling"
      content: "Index documents directly from data streams and structures."

    # feature loop
    - icon: "compare"
      title: "Misspelling Detection"
      content: "Suggest alternative words and track occurrences for improved accuracy."

    # feature loop
    - icon: "unreadable_characters"
      title: "Archive Support"
      content: "Index nested ZIP archives and retrieve file details within them."

    # feature loop
    - icon: "hidden_print"
      title: "Efficient Indexing"
      content: "Save disk space with compact indexing and process password-protected documents."

    # feature loop
    - icon: "style"
      title: "Custom Synonyms"
      content: "Add and manage synonyms for tailored search results."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Discover the powerful capabilities of GroupDocs.Search for .NET with hands-on examples."
  items:
    # code sample loop
    - title: "Boost Productivity with Fuzzy Search"
      content: |
        Leverage GroupDocs.Search for .NET for flexible and accurate content control through advanced search algorithms. [Explore more](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="How to process search result">}}
        ```csharp {style=abap}
        // Create an index
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Set up search options
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Search for documents containing the word 'water' or the phrase 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Process search result
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Advanced Search with Regular Expressions"
      content: |
        GroupDocs.Search for .NET supports regular expressions for precise searches. [Learn advanced techniques](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="How to search using regular expressions">}}
        ```csharp {style=abap}   
        // Create an index
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Search for the phrase in text form

        // The first caret character at the beginning indicates that this is a regular expression search query
        string query = "^^(.)\\1{1,}";
        // Search for two or more identical characters at the beginning of a word
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
