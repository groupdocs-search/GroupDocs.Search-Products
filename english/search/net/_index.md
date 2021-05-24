---
############################# Static ############################
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "C# .NET Text Search & Indexing API for Word Excel PDF Email HTML"
head_description: "C# .NET text searching API to smartly index & retrieve data from PDF, Microsoft Office Word, Excel, presentations, OneNote, Email, ZIP, EPUB & web files."

############################# Header ############################
title: ".NET API to Search & Index Documents"
description: "‎API to Index Data & Perform Text Search in all Popular Document Formats using .NET Applications."
button:
    enable: true

############################# SubMenu ############################
submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-net.png"
        product: "GroupDocs.Search"
        platform: ".NET"

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
            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "Pricing"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

############################# Overview ############################
overview:
    enable: true
    content: |
      GroupDocs.Search for .NET is a document and text search API for business applications developed in C#, ASP.NET and other .NET technologies. This .NET API supports basic to advanced search features, e.g., creation and merging of multiple indexes, searching through indexes using Simple, Boolean, Fuzzy, Regular Expression (regex) and other query types to fetch your required data, from files, documents and emails, through smart search. If you want to build a fast, reliable, smart and feature-rich search application for your end-users, supporting all popular file formats, GroupDocs.Search for .NET is all that you need.
    tabs:
      enable: true
      
      ## TAB ONE ##
      tab_one:
        description: |
          Following is an overview of GroupDocs.Search for .NET:
      
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
          GroupDocs.Search for .NET supports following [document file formats](https://docs.groupdocs.com/search/net/supported-document-formats/):

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
          GroupDocs.Search for .NET supports following Operating Systems, Frameworks & Package Managers:‎
        
        left:
          enable: true
          table:
            # table loop
            - icon: "fab fa-windows"
              title: "Operating Systems"
              content: |
                * Windows Desktop
                * Windows Server
                * Windows Azure
                * Linux

            # table loop
            - icon: "fas fa-code"
              title: "Supported Frameworks"
              content: |
                * .NET Framework 2.0 or higher
                * Mono Framework 1.2 or higher
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            # table loop
            - icon: "fas fa-box"
              title: "Package Manager"
              content: |
                * NuGet

            # table loop
            - icon: "fas fa-tools"
              title: "Development Environments"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

############################# Features ############################
features:
    enable: true
    title: "GroupDocs.Search for .NET Features"

    feature:
      # feature loop
      - icon: "fas fa-copy"
        content: "Create Index in Memory or on Disk & Perform Multi-threaded Indexing & Merging"

      # feature loop
      - icon: "fas fa-eye"
        content: "Prevent Indexing for Already Indexed Files or with a Specific String in its Name"

      # feature loop
      - icon: "fas fa-bolt"
        content: "View Progress Percentage of Index Creation and Updation & Get Search Report"
      
      # feature loop
      - icon: "fas fa-file-powerpoint"
        content: "Faster Indexing by Excluding Specific Words & Index Status Notification for Recently Processed Files"

      # feature loop
      - icon: "fas fa-code"
        content: "Index ZIP Archives within ZIP Archives & Get List of Indexed Files contained in an Archive"

      # feature loop
      - icon: "fas fa-cloud"
        content: "Use List or Import to Replace Characters during Indexing & Export them to a File"

      # feature loop
      - icon: "fas fa-remove-format"
        content: "Index & Search Password Protected Files & Compact Indexing to Save Disk Space"

      # feature loop
      - icon: "fas fa-comment-slash"
        content: "Extract Text from Index or Source File & Automatically Save Text File Encoding in Index‎"

      # feature loop
      - icon: "fas fa-location-arrow"
        content: "Add Arbitrary Additional Fields to each Document during Indexing"

      # feature loop
      - icon: "fas fa-border-all"
        content: "Set up Document Filtering in Search Results"

      # feature loop
      - icon: "fas fa-wrench"
        content: "Handle Typing Mistakes through Fuzzy Search, Set Similarity Level in Fuzzy Search & Display Best Results Only"

      # feature loop
      - icon: "fas fa-columns"
        content: "Index Documents from Streams and Data Structures"

      # feature loop
      - icon: "fas fa-file-word"
        content: "Search Complete Phrase with Stop Words and Combine Faceted Search with Boolean Search"

      # feature loop
      - icon: "fas fa-envelope"
        content: "Search based on Homophonic Terms, Synonyms, Date Range, Wild Cards & Case Sensitivity"

      # feature loop
      - icon: "fas fa-print"
        content: "Index & Search Emails from Outlook & Browse using Aspose.Email API"

      # feature loop
      - icon: "fas fa-file-archive"
        content: "Supports Spell Check & Wild Cards in Search Queries & Skip Special Characters in Search Phrases"

      # feature loop
      - icon: "fas fa-lock"
        content: "Limit Results for Each Term in Search Query as well as for All Results"

      # feature loop
      - icon: "fas fa-file-code"
        content: "Extract HTML Text to a File & Generate URL to Navigate HTML-Formatted Search Results"
      
      # feature loop
      - icon: "fas fa-fill-drip"
        content: "Combine Multiple Queries into Single Object Tree"

      # feature loop
      - icon: "fas fa-file-excel"
        content: "Alert User for Non-Supportive Settings & Auto-Index Reload in case of Indexing Error"

      # feature loop
      - icon: "fas fa-heading"
        content: "Enable Exact Number of Occurrences for each Found Word to Offer Alternative Word Suggestions in case of Misspelling"

      # feature loop
      - icon: "fas fa-project-diagram"
        content: "Add Text Attributes to Indexed Documents without Re-indexing"

      # feature loop
      - icon: "fas fa-cube"
        content: "Perform Indexing and Searching Operations Based on Characters"

      # feature loop
      - icon: "fab fa-uncharted"
        content: "Index Metadata of Non-Textual Document Formats"

    more_feature:
      # more_feature_loop
      - title: "Indexing & Search"
        content: |
          GroupDocs.Search for .NET API frequently uses index in order to perform search. Indexes are used to collect, parse or store data for fast and accurate searching.

          * **Create Index**: Create Index folder and add/index documents to that folder.
          * **Load Index**: Load an existing Index.
          * **Add Documents to Index**: Add documents to existing Index, asynchronously.
          * **Update Index**: Update existing Index, whenever a document is modified, added or deleted. This keeps search results up to date.

          ```cs
          // Create index
          Index  index = new Index(@"c:\MyIndex");
          // Add documents to index
          index.AddToIndex(@"c:\MyDocuments");
          // Search in index
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      # more_feature_loop
      - title: "Merge Multiple Indices to Improve Search Efficiency"
        content: "GroupDocs.Search for .NET is able to merge multiple indices into a singular index. If an index is frequently updated, it has several delta indices, but this approach reduces search performance. GroupDocs.Search for .NET API merges all delta indices into one consolidated index. The primary merged index will contain all the information from the merged delta indices; however, the delta indices will remain unchanged. This approach used by our API considerably improves the search efficiency. Index merging feature, provides numerous functionalities to tweak to further tweak this process.‎"

      # more_feature_loop
      - title: "Store Text in Index to Generate HTML Markup"
        content: "GroupDocs.Search for .NET can cache text of indexed documents in an index. This cached text is then used to rapidly generate HTML markup by highlighting search results. This approach is lot faster than extracting text directly from files. Retrieving text from cache will be available even if the source files are no longer available. The cached text can be stored by applying various compression levels to occupy lesser disk space and faster indexing time."

      # more_feature_loop
      - title: "Get Related Documents by Fuzzy & Regex Search"
        content: "When you perform Fuzzy or Regex search, you can get the list of documents that exactly matches your provided input. However, you will also get a list of documents that contain words or terms similar to your input. For example, if using GroupDocs.Search for .NET, you perform fuzzy search for query “cost”, you will get documents containing word “cost” and documents containing similar words such as “coat”. The results will be dependent on what level of fuzziness you have configured using this API."

      # more_feature_loop
      - title: "Recognize Search Queries of Different Keyboard Layout"
        content: "GroupDocs.Search for .Net can recognize search queries written in a language that does not match your keyboard layout. Currently, this .NET API can successfully recognize 88 languages and 164 different keyboard layouts."

      # more_feature_loop
      - title: "Search Using Morphological Word Form"
        content: "GroupDocs.Search for .NET API allows you to search for various word forms. For example, for a noun you can search for its singular and plural forms. For a verb, you can search for all forms of that verb. You can also search for root, third-person singular, simple past and various other forms. For languages other than English, you can implement customized word forms."

############################# Support ############################
support:
    enable: true

############################# Solutions ############################
solutions:
    enable: true
    title: "GroupDocs.Search offers document viewing APIs for other popular development environments"

    solution:
        # solution loop
        - img_alt: "GroupDocs.Search for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-java.png"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java"

############################# Back to top ###############################
back_to_top:
  enable: true
---