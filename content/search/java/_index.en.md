---
############################# Static ############################
layout: "landing"
date: 2024-12-11T15:07:52
draft: false

lang: en
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Java Document Search & Indexing Solution for PDFs, Office Files, and Web Content"
head_description: "Powerful text search and indexing for Java applications. Easily search and organize data in PDFs, Word, Excel, presentations, emails, and web formats."

############################# Header ############################
title: "Efficient Document Search and Indexing with Java API"
description: "Empower Java applications with robust text search features across all popular document formats."
words:
  for: "for"

actions:
  main: "Download Maven for Free"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Start Your Journey Today!"
  description: "Explore the capabilities of GroupDocs.Search for free or secure a license to unlock its full potential."

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"

code:
  title: "Search Files in a Directory with Java"
  more: "More examples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Create an index for your documents
    Index index = new Index("c:/MyIndex");

    // Add documents to the index for efficient searching
    index.add("c:/MyDocuments");
    
    // Search for specific words or phrases, such as
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Overview"
  description: "Discover the powerful text search capabilities of the Java Java library."
  features:
    # feature loop
    - title: "Indexing and Search Operations in Java"
      content: "With GroupDocs.Search for Java, you can collect, store, and analyze data efficiently to create detailed indexes for faster, more accurate searches."

    # feature loop
    - title: "Optimize Search by Merging Indexes"
      content: "Easily combine multiple indexes with GroupDocs.Search for Java to streamline searches. Reduce the impact of smaller delta indexes by consolidating them into a single, high-performance index."

    # feature loop
    - title: "Support for Multilingual Keyboard Layouts"
      content: "Search across different languages and keyboard layouts with GroupDocs.Search for Java. It supports 88 languages and 164 keyboard configurations for unmatched versatility."

    # feature loop
    - title: "Morphological Search Capabilities"
      content: "Find different word forms like singular/plural nouns or verb variations using GroupDocs.Search for Java. Customize search options for English and other languages."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Search for Java is compatible with major operating systems and package managers."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    Work with a wide range of file formats using GroupDocs.Search for Java. [View the full list](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Features of GroupDocs.Search for Java"
  description: "Manage document content effectively with advanced search capabilities supporting formats like PDF, DOCX, XLSX, PPTX, and more."

  items:
    # feature loop
    - icon: "document_info"
      title: "Customizable Search Parameters"
      content: "Refine searches using date ranges and case sensitivity filters."

    # feature loop
    - icon: "detect"
      title: "Enhanced Spell Check"
      content: "Search efficiently with spell check, wildcards, and by ignoring special characters."

    # feature loop
    - icon: "collect"
      title: "Filtered Search Results"
      content: "Apply filters to focus search results based on specific document types or criteria."

    # feature loop
    - icon: "get"
      title: "Import and Export Index Data"
      content: "Easily import data for indexing or export results to files for further use."

    # feature loop
    - icon: "remove"
      title: "Skip Unneeded Files"
      content: "Optimize indexing by excluding specific files or words."

    # feature loop
    - icon: "style"
      title: "HTML and URL Processing"
      content: "Extract HTML content to files and generate URLs for navigation through search results."

    # feature loop
    - icon: "detect"
      title: "Fast Search in Large Indexes"
      content: "Speed up search operations by dividing large indexes into manageable chunks."

    # feature loop
    - icon: "manipulate"
      title: "Stream-Based Indexing"
      content: "Index data directly from streams or data structures."

    # feature loop
    - icon: "compare"
      title: "Handle Misspelled Queries"
      content: "Detect misspellings and suggest alternative words for better search accuracy."

    # feature loop
    - icon: "unreadable_characters"
      title: "Comprehensive Archive Support"
      content: "Index nested archives and retrieve detailed lists of files within ZIP files."

    # feature loop
    - icon: "hidden_print"
      title: "Space-Saving Indexing"
      content: "Compact indexes to save disk space and process password-protected files."

    # feature loop
    - icon: "style"
      title: "Custom Synonym Support"
      content: "Expand the synonym dictionary to enhance search accuracy with tailored options."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Try out GroupDocs.Search for Java features with these code examples."
  items:
    # code sample loop
    - title: "Boost Search Accuracy with Fuzzy Matching"
      content: |
        Explore the flexibility of GroupDocs.Search for Java for managing content with advanced fuzzy search capabilities. [Learn more](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="How to process search result">}}
        ```java {style=abap}
        // Create an index
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Set up search options
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Search for documents containing the word 'water' or the phrase 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Process search result
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Refine Results with Regular Expressions"
      content: |
        Use regular expressions in GroupDocs.Search for Java to create precise and detailed search results. [Discover advanced techniques](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="How to search using regular expressions">}}
        ```java {style=abap}   
        // Create an index
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Search for the phrase in text form

        // The first caret character at the beginning indicates that this is a regular expression search query
        String query = "^^(.)\\1{1,}";
        // Search for two or more identical characters at the beginning of a word
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
