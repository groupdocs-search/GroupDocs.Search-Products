---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/java/boolean/pst"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM PST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Create Search Queries using Boolean Operators (AND, OR, NOT) via Java"
head_description: "Using GroupDocs.Search Java API programmers can create advanced search queries to find out documents via Boolean operators AND, OR, NOT inside their Java Apps."

############################# Header ############################
title: "Create Advanced Search Queries via Boolean Operators AND, OR, NOT  in Java Apps"
description: "GroupDocs.Search Java API enables programmers to create simple & complex search queries using Boolean operators (AND, OR, NOT) via Java APIs."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Create Advanced Search Queries via Boolean Operators in Java?"
    content: |
      Boolean search is a very valuable technique that is often used by portals  and search engines to produce the more relevant results by combining keywords with operators such as AND, NOT and OR. It is a structured search process that helps consumers to get a wider range of results, or reduce the number of unrelated search results by defining limitations. GroupDocs.Search for .NET is a leading document and text parsing and searching API that empower software professionals to create fast, reliable, smart and feature-rich business software applications for documents searching as well as indexing. It has included support for many popular documents file formats such as PDF, Microsoft Office Word, Excel worksheets, PowerPoint presentations, HTML, Outlook email, Outlook MSG, PST and many more.  It has included several important search features for examining indexes  using simple, Boolean, fuzzy, regular expression and other query types to get the required data. Moreover, it is also possible to identify search queries written in a language that does not match your keyboard layout.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Use Boolean AND Operator in Search Queries via Java"
      content_left: |
       GroupDocs.Search Java API allows software developers to add Boolean and other searches abilities inside Java application. The below Java code example demonstrates how to use Boolean "AND" Operator to create complex queries for text and object form searches inside their own Java applications. 

      title_right: "Search PST Documents via Boolean AND Operator"
      content_right: |
         * First you need to Specify the path to the index folder & document folder.
         * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
         * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
         * Search with text query by calling [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) method 
         * Creating subquery 1 and Creating subquery 2 by calling [SearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery) class
         *  Combining subqueries into one query by calling [CreateAndQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createAndQuery(com.groupdocs.search.SearchQuery,%20com.groupdocs.search.SearchQuery)) method 
         * Start searching and display search results
         
        
      gisthash: "e00f3c3e17fce2acf29197be6226314d"
      gistfile: "add_boolean_and_operator_java.java"

    - title_left: "Use Boolean OR Operator to Search PST Documents"
      content_left: |
       GroupDocs.Search for Java provides complete support for searching through many popular documents formats. The Boolean OR operator helps users to search all records that encompass any of the provided search terms. The below Java code examples illustrates how to use Boolean "OR" operator in text and object form queries inside Java applications.  

      title_right: "Boolean OR Operator for Searching PST Files"
      content_right: |
        * First you need to Specify the path to the index folder & document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
        * Search with text query by calling [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) method 
        * Creating subquery 1 and Creating subquery 2 by calling [SearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery) class
        *  Combining subqueries into one query by calling [CreateOrQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createOrQuery(com.groupdocs.search.SearchQuery,%20com.groupdocs.search.SearchQuery))) method 
        * Start searching and display search results
     
      gisthash: "f9f1dde116d8239202efa798daf659aa"
      gistfile: "add_boolean_or_operator_java.java"
      
    - title_left: "Generate Complex Search Queries via Boolean Operators in Java"
      content_left: |
        GroupDocs.Search for Java fully supports combining various Boolean operators to generate complex search queries using couple of lines of java code. The below Java code examples demonstrates how developers can create complex Search without installing any 3rd party external app or tool.

      title_right: "Search PST Documents via Complex Search Queries"
      content_right: |
        * First you need to Specify the path to the index folder & document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
        * Search with text query by calling [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) method 
        * Search with object query and Create theoryWordQuery & relativityWordQuery by calling [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) method
        *  Combining subqueries into one query by calling [CreateAndQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createAndQuery(com.groupdocs.search.SearchQuery,%20com.groupdocs.search.SearchQuery)) method 
        * Creating einsteinWordQuery  and Creating albertWordQuery by calling [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) class
        *  Combining subqueries into one query by calling [CreateOrQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createOrQuery(com.groupdocs.search.SearchQuery,%20com.groupdocs.search.SearchQuery)) method 
        *  Creates an inverted query that will find the rest documents in an index[createNotQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createNotQuery(com.groupdocs.search.SearchQuery)) method 
        * Start searching and display search results
     
      gisthash: "31fffc6f2c2dcd8995f6dabdbe8f460b"
      gistfile: "create_complex_queries_boolean_operator_java.java"

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