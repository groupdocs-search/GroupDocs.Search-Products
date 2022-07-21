---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/net/phrase /pst"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM PST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "How to Add Phrase Search in PST Documents in .NET Apps?"
head_description: "GroupDocs.Search .NET API enable software professions to add Phrase search and find the exact phrase or the provided sequence of words in PST documents via .NET API."

############################# Header ############################
title: "Add Exact Sentence or phrase Search in PST Documents inside .NET Apps?"
description: "GroupDocs.Search .NET API allows programmers to find out the provided sequence of words in PST documents via phrase search or exact sentence search inside .NET Apps. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Use Exact Sentence or Phrase Search in .NET Apps?"
    content: |
       Exact sentence or Phrase search is a kind of search that enables users to search out documents, web or database having an exact sentence or phrase that contains a specific order and combination of words defined by the consumers. It is a very common term in search engine terminology and allows users to search out documents for specified sequence of words in the text of indexed documents. GroupDocs.Search for .NET is a very useful high performance documents & text searching API that provided complete functionality for developing applications for text search and indexing supporting some of the most common documents types such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and so on. It has included support for several features related to phrase search such as searching query in text and object form, using wildcards in phrase search and so on.  

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "How to Perform Phrase Search in PST Documents via .NET"
      content_left: |
       GroupDocs.Search .NET API enables software developers to add Phrase search functionalities inside their own C# .NET application. The following .NET code example demonstrates how to perform Phrase Search in text & object with just a couple of lines of code.

      title_right: "Exact Phrase Search in PST Documents"
      content_right: |
         * First you need to Specify the path to the index folder & document folder.
         * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
         * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
         * Search for the phrase query 'phrase text' in text form
         * Search for the phrase 'phrase text' in object form
         * Creating word1, word2  and Creating subquery 3 by calling [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) method
         *  Combining subqueries to create new search query by calling [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) method 
         * Start searching and display search results
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: "Wildcards Phrase Search in PST Documents via .NET"
      content_left: |
        GroupDocs.Search for .NET enables software programmers to add Phrase search functionalities using Wildcards inside C# .NET application. The following .NET code examples shows how to apply wildcards phrase search in PST Documents inside C# applications. 

      title_right: "Apply Wildcards Phrase Search in PST File"
      content_right: |
        * First you need to Specify the path to the index folder & document folder.
        * Index Creation in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
        * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
        * Search for the phrase query 'phrase text' in text form
        * Search for the phrase 'phrase text' in object form
        * Creating word1  and Creating subquery 3 by calling [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) method
        * Creating  wildcard2 by calling [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) method
        *  Combining subqueries to create new search query by calling [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) method 
        * Start searching and display search results
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: "Combine Phrase Search with Other Types of Searches via .NET"
      content_left: |
        GroupDocs.Search .NET gives software programmers the power to combine phrase search with other types of searches inside .NET application. The following .NET code examples show how to apply both wildcards representing words and characters in words.

      title_right: ".NET API to Combine Phrase Search with Other Searches"
      content_right: |
        * First you need to Specify the path to the index folder & document folder.
        * Index Creation in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
        * Indexing documents from the specified folder by calling [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) method 
        * Search for the phrase in text form
        * Search for the phrase in object form
        * Define Word Pattern and append string.
        * Creating wordPattern1 and Creating word3 by calling [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery) method
        * Creating  wildcard2 by calling [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) method
        *  Combining subqueries to create new search query by calling [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) method 
        * Start searching and display search results
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

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