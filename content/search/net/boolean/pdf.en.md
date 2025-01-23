
---
############################# Static ############################
layout: "format"
date:  2025-01-23T10:13:32
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search in PDF docs via .NET using boolean operators"
head_description: "GroupDocs.Search for .NET API enables C# developers to search for data in document content with queries based on Boolean operators AND, OR, NOT."

############################# Header ############################
title: "Text search with boolean conditions" 
description: "GroupDocs.Search for .NET makes it easy to develop complex search queries using boolean operators (AND, OR, NOT) inside their .NET applications."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for free"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Search"
    link: "/search/net/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) is a powerful library for text search and data indexing in documents. It supports over 70 file formats, including PDF, Word, Excel, images, and ZIP files. With our solution, you can efficiently search through large volumes of information.

############################# Steps ############################
steps:
    enable: true
    title: "How to search in PDF document content using boolean logic"
    content: |
      [GroupDocs.Search](/search/net/) makes it easy to text search through PDF documents content. To improve search results in .NET applications many options like boolean logic search conditions are presented.
      
      1. Provide folder where searching index will be build.
      2. Point th a folder where PDF files are situated.
      3. Perform search procedure and get result.
      4. Process the result.
   
    code:
      platform: "net"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Search result"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Specify the path to the index folder
        Index index = new Index("c:/MyIndex");

        // Specify the path to a folder containing documents to search
        index.Add("c:/MyDocuments");

        // Perform search with complex query
        SearchResult result = index.Search("theory AND relativity");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Discover Powerful Features for Document Search and Indexing"
  description: "The GroupDocs.Search for .NET library is built to make text search and data indexing easy and efficient for 70+ file formats. Find and manage information quickly with advanced search capabilities."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Advanced Text Search"
      content: "Quickly search for text across multiple file formats, including PDFs, Word documents, spreadsheets, and more. Use flexible options like exact matches, fuzzy search, and wildcards to find what you need."

    # feature loop
    - title: "Index Large Volumes of Data"
      content: "Create and manage indexes for faster searches. Indexing organizes and stores data, making it easier to search through large collections of documents efficiently."

    # feature loop
    - title: "Support for Multiple Languages"
      content: "Search documents in different languages with support for over 80 languages and various keyboard layouts. Improve results with morphological word forms for specific languages."

    # feature loop
    - title: "Customizable Search Options"
      content: "Tailor your search experience with features like case sensitivity, date range filtering, and the ability to skip certain words or data during indexing."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to use compound search queries"
      content: |
        This example shows how to use boolean queries for PDF search.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Provide folder for search index
          Index index = new Index("c:/MyIndex");
              
          // Pass path to documents to be processed
          index.Add("c:/MyDocuments");

          // Use object query for search
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Get search results
          SearchResult result = index.Search(booleanQuery);
          
          // Process search result
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Copy"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pdf"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"
  items:
    #  loop
    - title: "Nuget download"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Explore Our Key Features"
    exclude: "boolean"
    description: "Discover powerful and efficient search capabilities"
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search in documents of popular formats"
    exclude: "PDF"
    description: "GroupDocs.Search supports searching in over 70 file formats. Customize search rules and use indexing to save time and effort."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---