---
############################# Static ############################
layout: "landing"
date: 2024-07-01T18:29:53
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
description: "Improve Node.js Applications by implementing Text Search in All Popular Document Formats."
words:
  for: "for"

actions:
  main: "Free NPM Download"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Licensing"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"

release:
  title: "Version {0} released"
  notes: "See what’s new"
  downloads: "Downloads"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Search in folder with JavaScript"
  more: "More examples"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // Creating index
    var index = new Index("c:\\MyIndex");

    // Adding documents to index
    index.addToIndex("c:\\MyDocuments");
    
    // Searching for various words like
    // 'affect', 'effect', 'principles', 'principally'
    var results = index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search at a glance"
  description: "Node.js JavaScript library for text search"
  features:
    # feature loop
    - title: "Node.js Indexing and Search Operation"
      content: "Indexing is used by GroupDocs.Search for Node.js via Java to collect data, as well as store and parse it for accurate and efficient search operations. GroupDocs.Search for Node.js via Java uses such Indexes frequently for performing search."

    # feature loop
    - title: "Merge Multiple Indexes to Improve Search Efficiency"
      content: "GroupDocs.Search for Node.js via Java API provides the feature to merge multiple indexes into a common index. For an index which is modified frequently, several delta indexes are created. This approach however, makes the search performance slow. GroupDocs.Search for Node.js via Java overcomes this bottle-neck by creating one common index through merging various delta indexes. This common merged index contains all the information of the merged delta indexes. This approach keeps the delta indexes unchanged while remarkably improving the search efficiency. You can configure various functionalities to further tweak this process."

    # feature loop
    - title: "Recognize Search Queries of Different Keyboard Layout"
      content: "GroupDocs.Search for Node.js via Java recognizes search queries that do not match your keyboard layout. At the moment, 88 languages and 164 different keyboard layouts can successfully be recognized by our solution."

    # feature loop
    - title: "Search Using Morphological Word Form"
      content: "Using GroupDocs.Search for Node.js via Java, you have freedom of searching for various word forms. You may search for singular and plural form of specific noun. Or you can choose to search all forms of a verb. Root, third-person singular and simple past along with various other forms can also be searched. For non English languages, you can configure customized word forms."

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
    GroupDocs.Search for Node.js via Java empowers you to process a diverse range of file formats. [Explore the full list](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "GroupDocs.Search for Node.js via Java: Feature Set"
  description: "Control business documents content using advanced search engine. Our solution supports most of the popular file formats including: PDF, DOCX, XLSX, PPTX, etc."

  items:
    # feature loop
    - icon: "watermark_add"
      title: "Flexible Parameters"
      content: "Use Date Range & Case Sensitivity as Search Parameters"

    # feature loop
    - icon: "watermark_style"
      title: "Spell Check Search"
      content: "Use Search Phrases with Spell Check and Wild Cards & Skip Special Characters in Queries"

    # feature loop
    - icon: "hidden_print"
      title: "Results Filtering"
      content: "Set up Document Filtering in Search Results"

    # feature loop
    - icon: "image_only"
      title: "Import & Export"
      content: "Perform Import or Use List to Modify Characters during Indexing & Export to a File"

    # feature loop
    - icon: "image_frame"
      title: "Skip Unnecessary Data"
      content: "Selectively Skip Indexing for Specific Files & Skip Specific Words to Index Faster"

    # feature loop
    - icon: "attachments"
      title: "URL Processing"
      content: "HTML Formatted Text Extraction to a File & Produce URL to Navigate Search Results in HTML"

    # feature loop
    - icon: "pdf_objects"
      title: "Rapid Search"
      content: "Divide Search in Smaller Chunks to Rapidly Search Huge Indexes"

    # feature loop
    - icon: "doc_background"
      title: "Stream Processing"
      content: "Index Documents from Streams and Data Structures"

    # feature loop
    - icon: "unreadable_characters"
      title: "Handle Misspelling"
      content: "Enable Exact Number of Occurrences for each Found Word to Offer Alternative Word Suggestions in case of Misspelling"

    # feature loop
    - icon: "watermark_text_search"
      title: "Archive Support"
      content: "Index Zipped Archives inside other ZIP Archives & Get List of Indexed Files in an Archive"

    # feature loop
    - icon: "watermark_image_search"
      title: "Disk Space Saving"
      content: "Save up Space by Compact Indexing & Password Secured Documents Indexing"

    # feature loop
    - icon: "document_info"
      title: "Custom Synonyms"
      content: "Add English Synonyms to Default Synonym Dictionary"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Code samples"
  description: "Investigate GroupDocs.Search for Node.js via Java functionalities with examples"
  items:
    # code sample loop
    - title: "Use 'fuzzy' search to increase productivity"
      content: |
        Enjoy flexible GroupDocs.Search for Node.js via Java functionality to enhance documents content control by sophisticated search algorithms. [Learn more](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="How to process search result">}}
        ```javascript {style=abap}
        // Create an index
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");

        // Set up search options
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Search for documents containing the word 'water' or the phrase 'Lorem ipsum'
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // Process search result
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Regular expressions are available for advanced search scenarios"
      content: |
        GroupDocs.Search for Node.js via Java allows us to use regular expressions in order to narrow search result. [Deep into advanced search techniques](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="How to search using regular expressions">}}
        ```javascript {style=abap}   
        // Create an index
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");
 
        // Search for the phrase in text form

        // The first caret character at the beginning indicates that this is a regular expression search query
        var query = "^^(.)\\1{1,}";
        // Search for two or more identical characters at the beginning of a word
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
