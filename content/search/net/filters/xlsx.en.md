
---
############################# Static ############################
layout: "format"
date:  2025-01-30T15:48:03
draft: false
lang: en
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search in XLSX documents using .NET"
head_description: "GroupDocs.Search for .NET is able to enrich C# applications by efficient text searches in various business document formats."

############################# Header ############################
title: "Search for text in business documents" 
description: "GroupDocs.Search for .NET provides text search in your documents, by powerful and flexible queries. Add search ability to .NET applications."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "What is GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) is a mature library designed for efficient text search and documents indexing. We support over 70 file formats, including such industry standard docs as PDF, Word, Excel, Presentation, etc. Fast and accurate search might improve your solution.

############################# Steps ############################
steps:
    enable: true
    title: "How to search in XLSX data"
    content: |
      [GroupDocs.Search](/search/net/) provides efficient search for XLSX documents, which could be used in .NET apps.
      
      1. Set up the folder to store the search index.
      2. Choose the folder containing files.
      3. Provide search options to process only XLSX documents.
      4. Get search results.
   
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
        // Path for the reusable search index
        Index index = new Index("c:/MyIndex");

        // Folder with documents
        index.Add("c:/MyDocuments");

        // Search only in documents with demanded format
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".xlsx");

        // Get search result
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced searching features"
  description: "GroupDocs.Search for .NET implements sophisticated text search across more than 70 file formats. Index constructing increases efficiency of locating and managing document information."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Main features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Advanced text search"
      content: "Get suitable text from business documents of popular types, including PDFs, Word, Presentations and spreadsheets. Many types of search like fuzzy search, homophone search, wildcards, etc. are supported."

    # feature loop
    - title: "Building search index increase usability"
      content: "Build and reuse search indexes in order to increase efficiency. Indexing optimizes searches across extensive document collections."

    # feature loop
    - title: "Frequently used languages support"
      content: "Searches in documents written on over 80 languages. Use different keyboard layouts and word variations to improve accuracy."

    # feature loop
    - title: "Flexible search settings"
      content: "Reduce amount of result data by using various options, settings, filters, regular expressions."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter documents to be processed"
      content: |
        Examine how to reduce number of processed docs by filters.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Provide search index not considering some formats.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Path to documents
          index.Add("c:/MyDocuments");

          // Retrieve search results
          SearchResult result = index.Search("Lorem");
          
          // Use search results
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
            link: "/examples/search/formats/searchfilters.xlsx"
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
    title: "Key features"
    exclude: "filters"
    description: "Use effective data search procedures."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Find data in your business documents"
    exclude: "XLSX"
    description: "Supporting 70+ file formats GroupDocs.Search enable processing of the most popular office documents."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---