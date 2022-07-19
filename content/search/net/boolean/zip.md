---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/net/boolean/zip"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Add Boolean Search Operators (AND, OR, NOT) in Search Queries via .NET"
head_description: "GroupDocs.Search .NET API enables software developers to add Boolean search or develop new queries using Boolean operators AND, OR, NOT inside their .NET Apps."

############################# Header ############################
title: "Develop Complex Search Queries using Boolean Operators AND, OR, NOT in .NET Apps"
description: "GroupDocs.Search .NET API allows computer programmers to develop complex search queries using Boolean operators (AND, OR, NOT) inside their .NET applications. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "What is Boolean Search and How to Use Boolean Operators?"
    content: |
       Boolean search is a very useful search procedure that allows users to combine different keywords with operator to bound, broaden, and define the search results. The Boolean operator such as AND, OR, NOT, and NEAR etc. helps users to get a broader range of results, or reduce the number of unrelated search results by defining limitations. GroupDocs.Search for .NET is powerful high performance document searching API that enables software developer to develop applications that can accomplish text search and indexing on some of the most common documents file formats like PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and many more.  The Boolean AND operator can be used to display results for all the words you have entered, the OR operator gives results for any of the words you have entered, the NOT operator can be used to display search results for no occurrences and so on.  One great feature is that it can recognize search queries written in a language that does not match your keyboard layout.  

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Use Boolean AND Operator in Search Queries via .NET"
      content_left: |
       GroupDocs.Search .NET API provides complete support for adding Boolean search capabilities inside their .NET application. The below C# code example shows how to create Boolean "AND" Operator in text and object form queries inside their own .NET applications. 

      title_right: " Search ZIP Documents via Boolean Operator AND "
      content_right: |
         * First you need to Specify the path to the index folder & document folder.
         * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
         * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
         * Creating subquery 1 and Creating subquery 2 by calling [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) class
         *  Combining subqueries into one query by calling [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
         * Start searching and display search results
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "How to Use Boolean Operator OR via .NET"
      content_left: |
       GroupDocs.Search for .NET is a powerful API that enables software programmers to search through many popular documents formats. The below C# .NET code examples shows how to use Boolean "OR" operator in text and object form queries inside C# applications. 

      title_right: "Use Boolean OR Operator to Search ZIP Files"
      content_right: |
        * First you need to Specify the path to the index folder & document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
        * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
        * Creating subquery 1 and Creating subquery 2 by calling [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) class
        *  Combining subqueries into one query by calling [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) method 
        * Start searching and display search results
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "Create Complex Search Queries using Boolean Operators"
      content_left: |
        GroupDocs.Search .NET enables computer programmers to combine different Boolean operators to created complex search queries inside their own .NET apps. The following .NET code examples shows how to complex documents searching capabilities without installing any external software or tools.

      title_right: "Search ZIP Documents via Complex Search Queries"
      content_right: |
        * First you need to Specify the path to the index folder & document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
        * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
        * Start searching and display search results text query
        * Search with object query
        * Creating WordQuery and relativityWordQuery by calling [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) class
        *  Combining subqueries into one query by calling [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
        * Creating einsteinWordQuery and albertWordQuery by calling [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) class
        *  Combining subqueries into one query by calling [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) method
        *  Combining subqueries into one query by calling [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) method 
        * Start searching and display search results
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

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