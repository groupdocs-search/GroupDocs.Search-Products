
---
############################# Static ############################
layout: "format"
date:  2025-02-13T15:29:06
draft: false
lang: en
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Search phrases in PPTX using .NET"
head_description: "GroupDocs.Search for .NET enhances C# applications with powerful phrase search capabilities for document content."

############################# Header ############################
title: "Search for phrases in documents" 
description: "Find specific phrases quickly with GroupDocs.Search for .NET. Integrate efficient search functionality into your .NET applications."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search features"
    link: "/search/net/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) is a powerful library for indexing and searching text in documents. It supports over 70 file formats, including PDFs, Word documents, Excel sheets, images, and ZIP files, enabling fast and accurate search results.

############################# Steps ############################
steps:
    enable: true
    title: "How to search phrases in PPTX documents"
    content: |
      [GroupDocs.Search](/search/net/) simplifies searching in PPTX documents. Use various options to refine search results in .NET applications.
      
      1. Set up the search index folder.
      2. Specify the folder containing PPTX files.
      3. Configure search settings.
      4. Retrieve and process search results.
   
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
        // Path to store the search index
        Index index = new Index("c:/MyIndex");

        // Folder containing documents
        index.Add("c:/MyDocuments");

        // Configure search options
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Execute the search
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Discover .NET document search engine"
  description: "GroupDocs.Search for .NET enables phrase searches across 70+ file formats. Easily locate and manage data with advanced search capabilities."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Key features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Phrase search"
      content: "Search for exact phrases in business documents, including PDFs, Word files, presentations, and spreadsheets. Use wildcards and other options if the exact phrase is unknown."

    # feature loop
    - title: "Efficient data indexing"
      content: "Create and reuse search indexes to speed up document searches. Indexing structures data efficiently, making phrase searches faster."

    # feature loop
    - title: "Multi-language support"
      content: "Search documents in over 80 languages. Supports different keyboard layouts and morphological word forms for better search accuracy."

    # feature loop
    - title: "Flexible search options"
      content: "Customize searches with features like case sensitivity, fuzzy and homophone search, document filtering, and more."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Using advanced search techniques"
      content: |
        Learn how to create queries for searching in PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Specify the folder for the search index
          Index index = new Index("c:/MyIndex");
              
          // Set the path to documents for search
          index.Add("c:/MyDocuments");

          // Create a query for a specific phrase
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Retrieve the search results
          SearchResult result = index.Search(query);
          
          // Process and utilize the results
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
            link: "/examples/search/formats/searchphrase.pptx"
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
    title: "Advanced features"
    exclude: "phrase"
    description: "Utilize powerful and efficient search functionalities."
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Phrase search in business documents"
    exclude: "PPTX"
    description: "GroupDocs.Search supports searches in 70+ document formats. Use advanced options and indexing to streamline your search process."
    items: 
        # format loop 1
        - name: "DOCX phrase search"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "PDF phrase search"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTX phrase search"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "TXT phrase search"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "XLSX phrase search"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---