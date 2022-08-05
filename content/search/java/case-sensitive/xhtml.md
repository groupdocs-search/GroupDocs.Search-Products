---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/java/case-sensitive/xhtml"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP  MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Java API to Perform Case-Sensitive Text Search in XHTML Documents"
head_description: "GroupDocs.Search Java API enables programmers to perform case-sensitive text search & discover the exact structure of words in XHTML documents via Java."

############################# Header ############################
title: "Perform Case-Sensitive Search Through XHTML  Documents in Java Apps"
description: "GroupDocs.Search Java API allows software developers to apply case-sensitive text search through various document types like  PDF, HTML, DOCX, PPTX,  XLSX & more in Java Apps."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Perform Case-Sensitive Search  in Java Apps?”"
    content: |
      Case Sensitivity is a very useful searching technique that describes a program’s capability to differentiate between uppercase (capital) and lowercase (small) letters in web, database or document searches. It is very important to remember that by default the search engine is case-insensitive, which means searching for word Computer will give both fragments having a key name or text having the words Computer and computer. Let’s suppose we need to narrow down the search results to the ones with capital letter ‘Computer’ which means we need case sensitive search. GroupDocs.Search for Java is an effective document searching & indexing API that enables software developer to develop applications that can accomplish text search and indexing for some of the most popular documents types like PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and many more. Moreover, it can identify search queries written in a language that does not match your keyboard layout.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Case-Sensitive Search in XHTML Documents via Java"
      content_left: |
       GroupDocs.Search Java API has incorporated complete support for basic as well as advanced searching features allowing software developers to make case-sensitive searches inside their java applications with just a couple of lines of code.
       
       The following Java code example shows how to achieve case-sensitive search with a query in the text in XHTML files with just a couple of lines of code.

      title_right: "Perform Case-Sensitive Search in XHTML Files"
      content_right: |
         * Identify path to the index folder as well as document folder.
         * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
         * Indexing documents from the specified folder by calling instance of [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) class
         * Initiate new instance of [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) class
         * Enabling case sensitive search option by calling [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) method
         * Define searching query and Start searching
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Make Case Sensitive Search in Object Form via Java"
      content_left: |
        GroupDocs.Search Java gives software developers the power to include searching functionality for various document formats inside their own applications. The following Java code example demonstrates how to perform case sensitive searches with a query in object form through XHTML documents. 

      title_right: "Apply Case Sensitive Search in XHTML Documents"
      content_right: |
        * Identify path to the index folder as well as document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Indexing documents from the specified folder by calling instance of [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) class
        * Initiate new instance of [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) class
        * Enabling case sensitive search option by calling [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) method
        * Creating search query in object by calling [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) method
        * Define searching query and Start searching
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

    - title_left: "System Requirements"
      content_left: |
        GroupDocs.Search for Java is supported on all major platforms and operating systems. For complete system requirements guide, please visit [system requirements](https://docs.groupdocs.com/search/java/system-requirements/) before executing the code below, please make sure that you have the following prerequisites installed on your system:
         * Operating Systems: Microsoft Windows, Linux, MacOS
         * Java Versions Support: J2SE 7.0 (1.7), J2SE 8.0 (1.8) or above
         * Get the latest version of GroupDocs.Search for Java APIs from GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
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