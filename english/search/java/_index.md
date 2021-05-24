---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Java Text Search & Indexing API for Documents, PDF, Office & Web"
head_description: "Advanced text search API for Java applications to search, index & retrieve data from documents: PDF, Word, Excel, presentations, email & web file formats."

############################# Header ############################
title: "Search & Index Documents via Java API"
description: "‎Build Java Applications to perform Text Search Manipulation in All Popular Document Formats.‎"
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-java.png"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            # button loop
            - link: "#overview"
              text: "Overview"

            # button loop
            - link: "#features"
              text: "Features"

            # button loop
            - link: "#support"
              text: "Support"

            # button loop
            - link: "https://products.groupdocs.app/search"
              text: "Live Demo"

            # button loop
            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Search for Java allows you to produce business applications that allow your end-users to perform search operations like never before. Our Java API enables users to operate basic to advanced level text search functions. Create and merge multiple indexes. Use Simple, Boolean, Regular Expression (Regex), Fuzzy and other types of queries to rapidly and smartly search through indexes. You can fetch your required information, from files, documents, emails, and archives, as GroupDocs.Search for Java supports all popular file formats.
    tabs:
      enable: true     
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Search for Java:

        left:
          enable: true
          icon: "fas fa-search"
          title: "Indexing"
          content: |
            * Create & Manage
            * Merge Multiple Indexes
            * Multi-Threading Async Indexing
            * Compact Indexing
            * Archived Files Indexing
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "Advanced Search & Search Queries"
          content: |
            * Fuzzy Search
            * Synonym Search
            * Email Search
            * Handling of Homophonic Terms
            * Searching Protected Files
            * Simple
            * Wild Card
            * Regular Expression (Regex)
            * Faceted & Boolean
            * Case Sensitive
      
      ## TAB TWO ##
      tab_two:
        description: |
          GroupDocs.Search for Java supports all popular [document file formats](https://docs.groupdocs.com/search/java/supported-document-formats/) including: Microsoft Office, images, diagrams and many others.

        left:
          enable: true
          table:
            # table loop
            - title: "Microsoft Office Formats"
              content: |
                * **Word**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Project**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: ONE

        right:
          enable: true
          table:
            # table loop
            - title: "OpenDocument & Other Formats"
              content: |
                * **Portable Document Format**: PDF
                * **OpenDocument**: ODT, OTT, ODS, OTS, ODP
                * **Email**: PST, OST, MSG, EML, EMLX
                * **Web File Formats**: XML, HTM, HTML, XHTML, MHT, MHTML
                * **Audio**: MP3, WAV
                * **Video**: AVI, MOV, QT, FLV, ASF
                * **Text**: TXT
                * **Rich Text Format**: RTF
                * **Markdown Documentation File**: MD
                * **Images**: BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **Others**: TORRENT, ZIP, DCM, DJVU, EPUB, FB2

      ## TAB THREE ##
      tab_three:
        description: |
          GroupDocs.Search for Java supports following Operating Systems, Frameworks & Package ‎Managers:‎
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Microsoft Windows Desktop
                * Microsoft Windows Server
                * Linux
                * MacOS

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * Java 7 (1.7) and above

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-cogs"
              title: "Development Environments"
              content: |
                * NetBeans
                * IntelliJ IDEA
                * Eclipse
            # table loop
            - icon: "fas fa-tools"
              title: "Build Automation Tool"
              content: |
                * Maven

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Search for Java Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Build Index on Disk or in Memory with Async Multithreading"

      # feature loop
      - icon: "fas fa-eye"
        content: "View Index Creation & Updation Progress"

      # feature loop
      - icon: "fas fa-bolt"
        content: "Selectively Skip Indexing for Specific Files & Skip Specific Words to Index Faster"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Perform Import or Use List to Modify Characters during Indexing & Export to a File"

      # feature loop
      - icon: "fas fa-code"
        content: "Reload Index in case of Error Indexing & Alert User for Contradictory Settings"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Index Status Notification regarding Latest Processed Files"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Index Zipped Archives inside other ZIP Archives & Get List of Indexed Files in an Archive"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Save up Space by Compact Indexing & Password Secured Documents Indexing‎"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Document Text Extraction from Index or Source File"

      # feature loop
      - icon: "fas fa-border-all"
        content: "HTML Formatted Text Extraction to a File & Produce URL to Navigate Search Results in HTML"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Add Arbitrary Additional Fields to each Document during Indexing"

      # feature loop
      - icon: "fas fa-columns"
        content: "Configure Similarity Level for Fuzzy Search & Show Best Results"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Smart Management of Typos through Fuzzy Search"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Use Faceted & Boolean Search Simultaneously"

      # feature loop
      - icon: "fas fa-print"
        content: "Configure & Perform Synonyms Search & Smartly Deal with Homophonic Terms"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Use Date Range & Case Sensitivity as Search Parameters"

      # feature loop
      - icon: "fas fa-lock"
        content: "Make Index to Search & Browse Email Messages via Aspose.Email API"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Use Search Phrases with Spell Check and Wild Cards & Skip Special Characters in Queries"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Make Single Object Tree by Combining Multiple Queries"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Divide Search in Smaller Chunks to Rapidly Search Huge Indexes"

      # feature loop
      - icon: "fas fa-heading"
        content: "Index Documents from Streams and Data Structures"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Set up Document Filtering in Search Results"

      # feature loop
      - icon: "fas fa-cube"
        content: "Add English Synonyms to Default Synonym Dictionary"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Enable Exact Number of Occurrences for each Found Word to Offer Alternative Word Suggestions in case of Misspelling"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Add Text Attributes to Indexed Documents without Re-indexing"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Perform Indexing and Searching Operations Based on Characters"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Index Metadata of Non-Textual Document Formats"

    more_feature:
      # more_feature_loop
      - title: "Indexing and Search Operation"
        content: |
          Indexing is used by GroupDocs.Search for Java to collect data, as well as store and parse it for accurate and efficient search operations. GroupDocs.Search for Java uses such Indexes frequently for performing search.

          * **Create Index**: Create Index folder and add/index documents to that folder.
          * **Load Index**: Load an existing Index.
          * **Add Documents to Index**: Add documents to existing Index, asynchronously.
          * **Update Index**: Update existing Index, whenever a document is modified, added or deleted. This keeps search results up to date.
          
          ```java
          / Creating index
          Index index = new Index("c:\\MyIndex");
          // Adding documents to index
          index.addToIndex("c:\\MyDocuments");
          // Searching for words 'affect' or 'effect' in a document with 'principal', 'principle', 'principles', or 'principally'
          SearchResults results = index.search("?ffect & princip?(2~4)");
          ```
      # more_feature_loop
      - title: "Merge Multiple Indices to Improve Search Efficiency"
        content: "GroupDocs.Search for Java API provides the feature to merge multiple indexes into a common index. For an index which is modified frequently, several delta indexes are created. This approach however, makes the search performance slow. GroupDocs.Search for Java overcomes this bottle-neck by creating one common index through merging various delta indexes. This common merged index contains all the information of the merged delta indexes. This approach keeps the delta indexes unchanged while remarkably improving the search efficiency. You can configure various functionalities to further tweak this process.‎‎"

      # more_feature_loop
      - title: "Recognize Search Queries of Different Keyboard Layout"
        content: "GroupDocs.Search for Java recognizes search queries that do not match your keyboard layout. At the moment, 88 languages and 164 different keyboard layouts can successfully be recognized by GroupDocs.Search for Java.‎"

      # more_feature_loop
      - title: "Search Using Morphological Word Form"
        content: "Using GroupDocs.Search for Java, you have freedom of searching for various word forms. You may search for singular and plural form of specific noun. Or you can choose to search all forms of a verb. Root, third-person singular and simple past along with various other forms can also be searched. For non English languages, you can configure customized word forms."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-net.png"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net"

############################# Back to top ###############################
back_to_top:
  enable: true
---