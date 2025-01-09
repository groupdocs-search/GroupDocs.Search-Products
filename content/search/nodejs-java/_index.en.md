---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: en
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Text Search & Indexing Library for Documents, PDF, Office & Web"
head_description: "Advanced text search solution for Node.js applications to search, index & collect data from documents: PDF, Word, Excel, presentations, email & web file formats."

############################# Header ############################
title: "Search & Index Documents using Node.js API"
description: "Enhance Node.js Applications by implementing Text Search in All Popular Document Formats."
words:
  for: "for"

actions:
  main: "Free NPM Download"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Start Your Journey Today!"
  description: "Explore the capabilities of GroupDocs.Search for free or secure a license to unlock its full potential."

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Perform Text Search in a Folder with JavaScript"
  more: "More examples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Create an index for your documents
    const index = new searchLib.Index('c:/MyIndex');

    // Add documents to the index for efficient searching
    index.add('c:/MyDocuments');
    
    // Search for specific words or phrases, such as
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Overview"
  description: "Node.js JavaScript library for text search"
  features:
    # feature loop
    - title: "Node.js Indexing and Search Operations"
      content: "Indexing in GroupDocs.Search for Node.js via Java collects, stores, and parses data for precise and efficient search operations. These indexes are frequently used to perform searches."

    # feature loop
    - title: "Merge Multiple Indexes to Enhance Search Efficiency"
      content: "GroupDocs.Search for Node.js via Java API allows the merging of multiple indexes into one. Frequent modifications create several delta indexes, which can slow down search performance. Our solution merges these delta indexes into a common index, containing all the information from the merged delta indexes, significantly improving search efficiency while keeping the delta indexes unchanged. Various functionalities can be configured to fine-tune this process."

    # feature loop
    - title: "Recognize Search Queries from Different Keyboard Layouts"
      content: "GroupDocs.Search for Node.js via Java recognizes search queries that do not match the keyboard layout. Currently, 88 languages and 164 different keyboard layouts are supported."

    # feature loop
    - title: "Search Using Morphological Word Forms"
      content: "With GroupDocs.Search for Node.js via Java, you can search for various word forms, such as singular and plural nouns, or all forms of a verb. English and non-English languages can be customized for specific word forms."

############################# Platforms ############################
platforms:
  enable: true
  title: "Platform independence"
  description: "GroupDocs.Search for Node.js via Java supports all popular operating systems and package managers."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Supported file formats"
  description: |
    GroupDocs.Search for Node.js via Java enables processing a wide range of file formats. [Explore the full list](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
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
  title: "GroupDocs.Search for Node.js via Java Features"
  description: "Control business document content using our advanced search engine, supporting popular file formats including PDF, DOCX, XLSX, PPTX, and more."

  items:
    # feature loop
    - icon: "document_info"
      title: "Flexible Parameters"
      content: "Use Date Range & Case Sensitivity as Search Parameters"

    # feature loop
    - icon: "detect"
      title: "Spell Check Search"
      content: "Use Search Phrases with Spell Check and Wildcards & Skip Special Characters in Queries"

    # feature loop
    - icon: "collect"
      title: "Results Filtering"
      content: "Set up Document Filtering in Search Results"

    # feature loop
    - icon: "get"
      title: "Import & Export"
      content: "Perform Import or Use List to Modify Characters during Indexing & Export to a File"

    # feature loop
    - icon: "remove"
      title: "Skip Unnecessary Data"
      content: "Selectively Skip Indexing for Specific Files & Skip Specific Words to Index Faster"

    # feature loop
    - icon: "style"
      title: "URL Processing"
      content: "Extract HTML Formatted Text to a File & Generate URL to Navigate Search Results in HTML"

    # feature loop
    - icon: "detect"
      title: "Rapid Search"
      content: "Divide Search into Smaller Chunks to Rapidly Search Large Indexes"

    # feature loop
    - icon: "manipulate"
      title: "Stream Processing"
      content: "Index Documents from Streams and Data Structures"

    # feature loop
    - icon: "compare"
      title: "Handle Misspelling"
      content: "Enable Exact Number of Occurrences for each Found Word to Offer Alternative Word Suggestions in case of Misspelling"

    # feature loop
    - icon: "unreadable_characters"
      title: "Archive Support"
      content: "Index Zipped Archives inside other ZIP Archives & Retrieve List of Indexed Files in an Archive"

    # feature loop
    - icon: "hidden_print"
      title: "Disk Space Saving"
      content: "Save Space with Compact Indexing & Index Password Secured Documents"

    # feature loop
    - icon: "style"
      title: "Custom Synonyms"
      content: "Add English Synonyms to Default Synonym Dictionary"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Explore GroupDocs.Search for Node.js via Java functionalities with examples"
  items:
    # code sample loop
    - title: "Use 'fuzzy' search to enhance productivity"
      content: |
        Enjoy flexible GroupDocs.Search for Node.js via Java functionality to enhance documents content control by sophisticated search algorithms. [Learn more](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="How to process search result">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Create an index
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Set up search options
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Search for documents containing the word 'water' or the phrase 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Process search result
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Regular expressions are available for advanced search scenarios"
      content: |
        GroupDocs.Search for Node.js via Java allows us to use regular expressions in order to narrow search result. [Dive into advanced search techniques](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="How to search using regular expressions">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Create an index
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Search for the phrase in text form

        // The first caret character at the beginning indicates that this is a regular expression search query
        const query = '^^(.)\\1{1,}';
        // Search for two or more identical characters at the beginning of a word
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
