
---
############################# Static ############################
layout: "format"
date:  2025-01-23T14:09:57
draft: false
lang: en
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search PDF in .NET using boolean operators"
head_description: "The GroupDocs.Search for .NET API allows C# developers to search document content using boolean operators like AND, OR, and NOT."

############################# Header ############################
title: "Boolean logic text search" 
description: "GroupDocs.Search for .NET makes it simple to create advanced search queries using boolean operators (AND, OR, NOT) within your .NET applications."
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
       [GroupDocs.Search for .NET](/search/net/) is a comprehensive library for searching and indexing text in documents. It supports over 70 file formats, such as PDF, Word, Excel, images, and ZIP files, enabling efficient processing of large amounts of information.

############################# Steps ############################
steps:
    enable: true
    title: "How to search PDF document content using boolean logic"
    content: |
      [GroupDocs.Search](/search/net/) makes searching PDF document content straightforward. It provides Boolean logic search conditions to refine results in .NET applications.
      
      1. Specify the folder to store the search index.
      2. Choose the folder containing PDF files.
      3. Run the search and retrieve results.
      4. Process the results.
   
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
        // Set the path to the index folder
        Index index = new Index("c:/MyIndex");

        // Specify the folder containing documents to search
        index.Add("c:/MyDocuments");

        // Run a search using a complex query
        SearchResult result = index.Search("theory AND relativity");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explore advanced features for document search and indexing"
  description: "The GroupDocs.Search for .NET library simplifies text search and indexing for more than 70 file formats. Easily locate and manage information with advanced search tools."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Main features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Powerful text search"
      content: "Search for text across various file types, including PDFs, Word documents, and spreadsheets. Use features like exact matches, fuzzy searches, and wildcards to refine results."

    # feature loop
    - title: "Index large data sets"
      content: "Create and maintain indexes for quicker searches. Indexing structures and organizes data, making it easier to search extensive document collections."

    # feature loop
    - title: "Supports multiple languages"
      content: "Search documents in over 80 languages, with support for different keyboard layouts and morphological word forms to enhance search accuracy."

    # feature loop
    - title: "Customizable search options"
      content: "Adjust search settings with features like case sensitivity, date range filters, and the ability to exclude specific words or data during indexing."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Using advanced boolean search queries"
      content: |
        This example demonstrates how to apply boolean queries for searching PDF documents.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Set the folder for the search index
          Index index = new Index("c:/MyIndex");
              
          // Specify the path to the documents to be searched
          index.Add("c:/MyDocuments");

          // Create a search query using Boolean logic
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Retrieve the search results
          SearchResult result = index.Search(booleanQuery);
          
          // Process the search results
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
    title: "Discover key features"
    exclude: "boolean"
    description: "Explore advanced and efficient search functionalities."
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
    title: "Search across popular document formats"
    exclude: "PDF"
    description: "GroupDocs.Search supports over 70 file formats. Customize search rules and leverage indexing to save time and effort."
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