---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/net/filters/txt"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Customize Search Results by Setting Document Filtering in .NET Apps"
head_description: "GroupDocs.Search .NET API allows software developers to search out TXT Documents documents and customize the search results by applying document Filtering in .NET Apps."

############################# Header ############################
title: "Set Document Filtering to Customize Search Results inside .NET Apps"
description: "GroupDocs.Search .NET API help software professions to add documents searching capabilities  & customize search result by applying document Filtering inside their .NET Apps."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Apply Document Filtering in Search Result via .NET?"
    content: |
       Filtering is a very useful technique that empowers users to inspect and process functionality. Document filtering offers users an easy way to navigate their results and find what they’re looking for. It also gives users that power to limit their search to a certain section or a particular document type. GroupDocs.Search for .NET is feature rich high performance document searching API that empowers software developer to build applications that can achieve text search and indexing. It supports some of the most popular documents formats such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and many more. The API fully supports setting document fileting for search results. You can use several kinds of filers to customize your search results such as File path filters, file extension filter, attribute filter and many more. It is also possible to combine search document filters by using Boolean operator AND, OR & NOT etc.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Set Document Filter in Searching TXT Documents via .NET"
      content_left: |
       GroupDocs.Search .NET API helps software developers to add searching capabilities inside their .NET application. The following .NET code example demonstrates how to apply document filter in searching various kind of documents with just a couple of lines of code.

      title_right: "Apply Document Filter in Searching TXT Documents"
      content_right: |
       * First you need to Specify the path to the index folder & document folder.
       * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
       * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
       * Creating a search options object [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 
       * Set document filter by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Start searching and display search results
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: "How to Combine Search Document Filters via .NET"
      content_left: |
        GroupDocs.Search for .NET allows software programmers to combine search document filters while searching  to control which of the documents found should be returned as a result of the search inside C# .NET application. The following .NET code examples shows how to combine search document filters using Boolean operators AND, OR, NOT etc. inside C# applications. 

      title_right: "Combine Search Document Filters in Searching TXT Files"
      content_right: |
       * First you need to Specify the path to the index folder & document folder.
       * Creating an AND composite filter that returns all FB2 and EPUB documents that have the word 'Einstein' in their full paths
       * Create filter1 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Create filter2 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Combine filters by calling [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand) method
       * Creating an OR composite filter that returns all DOC, DOCX, PDF and all documents that have the word Einstein in their full paths
       * Create filter3 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Create filter4 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Combine filters by calling [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor) method
       * Creating a filter that returns all found documents except of TXT documents
       * Create filter4 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)
       * Appy Not filter by calling [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot) method

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
    - title_left: "System Requirements"
      content_left: |
        GroupDocs.Search for .NET is supported on all major platforms and operating systems. For complete system requirements guide, please visit [system requirements](https://docs.groupdocs.com/search/net/system-requirements/) before executing the code below, please make sure that you have the following prerequisites installed on your system:
         * Operating Systems: Microsoft Windows, Linux, MacOS
         * Development Environment: Visual Studio, Xamarin, MonoDevelop etc
         * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
         * Get the latest version of GroupDocs.Search for .NET APIs from [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
      title_right: "Why Use GroupDocs.Search"
      content_right: |
        * Search Index creation in memory as well as on disk.
        * Ability of indexing from a file, stream or structure.
        * Password protected documents indexing support.
        * Support for merging of several indexes.
        * Filter Document during search indexing.
        * Spell check support during the search.
        * Blended characters are fully supported
        * Combining different types of search into one search query.
        * Simple word  and regular expression searches support
        * Fully support alias replacement in search queries.

demos:
    enable: true
        

about_formats:
    enable: true


more_formats:
    enable: true


back_to_top:
    enable: true
---