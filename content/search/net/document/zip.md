---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/net/document/zip"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Create & Add Documents Searching & indexing inside .NET Applications"
head_description: "GroupDocs.Search .NET API allows to add  instant documents searching supporting formats like PDF DOC, DOCX, RTF, XLSX, CSV, PPTX & Email messages inside .NET Apps."

############################# Header ############################
title: "How to Add Instant Documents Search to ZIP via C# .NET API "
description: "GroupDocs.Search .NET API allows developers to add robust documents searching & indexing capability to their apps. It supports documents like PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, MSG, EML and many more. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Create & Add Documents Searching & Indexing using .NET API?"
    content: |
       This page will help users to learn about how to add documents searching and indexing capability inside their own applications with little effort and cost.  Indexing is the process that is used by search engines by which the data is organized and structured so that it can generate relevant search results. The aim is to quickly and accurately find and display information related to user’s queries.  GroupDocs.Search for .NET is powerful high performance document searching API that enables software developer to perform advance searching and indexing operations on the basis of fuzzy and synonym algorithms inside their own applications. It does not require any third-party tool or external software to be installed on the user’s machine.  It has included support for some of the most commonly used documents formats, such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and many more. It supports several types of searches such as simple word, Boolean, regular expression search, case sensitive search, flexible fuzzy, synonym, homophone, wildcard, search by chunks, object type search, setting data range and so on. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Search Index Creation for ZIP Document via .NET API"
      content_left: |
       GroupDocs.Search .NET API provides complete support for creating new Index or opening existing search index inside your own apps. The below C# code example shows how to create a new index and open an existing index using just a couple of lines of code. 

      title_right: "How to Create New or Open Existing Search Index"
      content_right: |
         * First you need to Specify the path to the index folder
         * Create an instance of [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) class
         * Above will create an index in memory or on a disk and can also open an existing index.
       
      gisthash: "9651c19a9436afee860b7f39197f8399"
      gistfile: "create_or_open_new_search_index.cs"

    - title_left: "How to Add Documents Synchronously to Search Index"
      content_left: |
       GroupDocs.Search .NET allows software developers to perform Document indexing synchronously inside their own .NET apps. The below C# .NET code examples shows how to perform indexing synchronously with ease. 

      title_right: "Synchronously Document Indexing via C#"
      content_right: |
        * First you need to Specify the path to the index folder
        * Specify path to a folder containing documents to search
        * Create an instance of [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) class
        * Above will create an index in memory or on a disk or open an existing index. 
        * Synchronous indexing documents from the specified folder
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_synchronously_to_indexing.cs"
      
    - title_left: "Perform Document Indexing Asynchronously via .NET"
      content_left: |
        GroupDocs.Search .NET enables computer programmers to perform asynchronousl document indexing inside their own .NET apps. The following .NET code examples shows how to achieve asynchronously documents indexing with just a couple of lines of code.

      title_right: "Asynchronously Document Indexing via C#"
      content_right: |
        * First you need to Specify the path to the index folder
        * Specify path to a folder containing documents to search
        * Create an instance of [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) class
        * Subscribing to the event
        * Need to write Code indicating the completion of the operation
        * Setting the flag for asynchronous indexing 
        * Asynchronous indexing documents from the specified folder
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_asynchronously_to_indexing.cs"

    - title_left: "How to Use & Highlight Search Results in .NET Apps"
      content_left: |
       GroupDocs.Search .NET API allows programmers to interpret a sarch result and show the results by a simple list of documents found, or the words and phrases found. You can also highlight the text of the document with ease. The following .NET code examples shows how to list found documents and highlight search results with just a couple of lines of code.

      title_right: "Highlight Search Results via C# "
      content_right: |
        * Peform Search in index
        * After succesful Search, Print the result
        * Iterate through the documents and display the found documents
        * Highlighting occurrences in text
        * Generating output HTML formatted document with highlighted search results
     
      gisthash: "a5d1ad6eedd2acf12a33b541e763cdb4"
      gistfile: "how_to_list_search_result.cs"

    - title_left: "System Requirements"
      content_left: |
        GroupDocs.Search for .NET is supported on all major platforms and operating systems. For complete system requirements guide, please visit [system requirements](https://docs.groupdocs.com/search/net/system-requirements/) before executing the code below, please make sure that you have the following prerequisites installed on your system:
         * Operating Systems: Microsoft Windows, Linux, MacOS
         * Development Environment: Visual Studio, Xamarin, MonoDevelop etc
         * Frameworks: .NET Framework, .NET Standard, .NET Core, Mono
         * Get the latest version of GroupDocs.Search for .NET APIs from [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
      title_right: "Why Use GroupDocs.Assembly"
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