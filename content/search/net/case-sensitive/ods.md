---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/net/case-sensitive/ods"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Apply Case-Sensitive Text Search Through ODS Documents via .NET"
head_description: "GroupDocs.Search .NET API enable software programmers to apply case-sensitive Text Search and find the exact sequence of words in ODS documents via .NET API."

############################# Header ############################
title: "How to Apply Case-Sensitive Search Through ODS Documents inside .NET Apps?"
description: "GroupDocs.Search .NET API allows software developers to apply case-sensitive text search through various documents type like  PDF, HTML, DOCX, PPTX,  XLSX & more inside .NET Apps."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "What is Case-Sensitive Search & How to Achieve It via .NET?"
    content: |
      There are numerous useful searching techniques that can help users to search through various types of documents for a particular combination of words or other data. Case-Sensitive Search is a very useful technique that allows users to search out documents & web pages whether uppercase and lowercase letters are treated as different or equal. For example, "Computer", "computer" and "COMPUTER" will be treated as dissimilar words because the letter "C" is uppercase in the first instance, lowercase in the second and all uppercase letters in the 3rd one. GroupDocs.Search for .NET is convenient high performance document searching API that empowers software creator to make software applications and tools for accomplishing text search as well as documents indexing with ease. The API provides supports for some of the most commonly used file formats such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and many more.  One other useful feature is that it can identify search queries written in a language that does not match your keyboard layout.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Perform Case-Sensitive Search in ODS Documents via .NET"
      content_left: |
       GroupDocs.Search .NET API enables software programmers to add case-sensitive search functionality inside their own C# .NET application. The following .NET code example illustrates how to achieve case-sensitive search with a query in the text form in ODS files with just a couple of lines of code.

      title_right: "Apply Case-Sensitive Search in ODS Documents"
      content_right: |
         * Identify path to the index folder as well as document folder.
         * Generate an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
         * Indexing documents from the specified folder by calling instance of [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) class
         * Initializes a new instance of [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) class
         * Enabling case sensitive searchb by calling [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) method
         * Define searching string and Start searching
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: "Perform Case-Sensitive Search in Object Form via .NET"
      content_left: |
        GroupDocs.Search .NET gives software developers the power to discover words bearing in mind uppercase and lowercase letters inside .NET application. The following .NET code example illustrates how to apply case-sensitive search with a query in object form in ODS documents. 

      title_right: "Make Case-Sensitive Search in ODS Documents"
      content_right: |
        * Identify path to the index folder as well as document folder.
        * Generate an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
        * Indexing documents from the specified folder by calling instance of [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) class
        * Initializes a new instance of [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) class
        * Enabling case sensitive searchb by calling [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) method
        * Creating search query in object form by calling [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) method
        * Start searching and display search results
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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