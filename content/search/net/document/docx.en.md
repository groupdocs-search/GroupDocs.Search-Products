
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: en
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search DOCX documents in .NET with GroupDocs.Search"
head_description: "Use GroupDocs.Search for .NET to perform efficient text searches in various document formats with C#."

############################# Header ############################
title: "Advanced document text search" 
description: "GroupDocs.Search for .NET simplifies text search in popular document formats, allowing you to create powerful search queries in your .NET applications."
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
       [GroupDocs.Search for .NET](/search/net/) is a powerful library designed for full-text search and indexing in documents. It supports over 70 file formats, including PDF, Word, PowerPoint, Excel, images, and ZIP files, ensuring fast and accurate search results.

############################# Steps ############################
steps:
    enable: true
    title: "How to perform text search in DOCX documents"
    content: |
      [GroupDocs.Search](/search/net/) enables advanced content search operations in DOCX documents, allowing refined search results in .NET applications.
      
      1. Set up the folder to store the search index.
      2. Choose the folder containing DOCX files.
      3. Configure additional search options.
      4. Run the search and review results.
   
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
        // Define the path for the search index
        Index index = new Index("c:/MyIndex");

        // Select the folder containing documents to be searched
        index.Add("c:/MyDocuments");

        // Enable homophone search to find words that sound alike
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Execute a complex search query
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Advanced search and indexing features"
  description: "GroupDocs.Search for .NET enhances text search and indexing across more than 70 file formats, providing efficient tools for locating and managing information."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Key Features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Powerful text search"
      content: "Search for text across multiple document types, including PDFs, Word documents, PowerPoint presentations, and spreadsheets. Use features like exact matches, fuzzy search, and wildcards to refine your results."

    # feature loop
    - title: "Fast indexing for large data sets"
      content: "Create and manage search indexes for quick retrieval of information. Indexing optimizes searches across extensive document collections."

    # feature loop
    - title: "Multi-language support"
      content: "Perform searches in over 80 languages, with support for different keyboard layouts and word variations to improve accuracy."

    # feature loop
    - title: "Customizable search settings"
      content: "Fine-tune search parameters with options like case sensitivity, date range filters, and word exclusions for better results."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Executing advanced search queries"
      content: |
        This example demonstrates how to apply search queries for DOCX documents.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Define the folder for the search index
          Index index = new Index("c:/MyIndex");
              
          // Specify the path to the document files
          index.Add("c:/MyDocuments");

          // Provide a password for protected documents
          index.Dictionaries.DocumentPasswords.Add("protected.docx", "123456");

          // Enable fuzzy search to find similar words
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Retrieve search results
          SearchResult result = index.Search("Loarem", options);
          
          // Process the search output
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
            link: "/examples/search/formats/searchdocument.docx"
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
    title: "Explore key features"
    exclude: "document"
    description: "Take advantage of advanced and high-performance search functionalities."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Search across your business documents"
    exclude: "DOCX"
    description: "GroupDocs.Search supports more than 70 file formats, including office documents, enabling quick and efficient searches with indexing capabilities."
    items: 
        # format loop 1
        - name: "Search in DOCX document"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF document"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX document"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT document"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX document"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---