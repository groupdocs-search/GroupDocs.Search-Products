---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/java/document/dotm"
otherformats: PDF DOC DOT DOCX DOCM DOTX TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB8 

############################# Head ############################
head_title: "Add Documents Indexing and Search Operations inside Java Apps"
head_description: "GroupDocs.Search Java API supports documents indexing & searching operations for documents formats like PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG and more."

############################# Header ############################
title: "Java API for DOTM Documents Indexing & Searching Operations "
description: "GroupDocs.Search Java API allows developers to integrate robust documents searching & indexing operations to their apps. It supports file formats like PDF DOC, DOCX, RTF, XLSX, CSV, PPTX MSG, EML & many more."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Add Documents Indexing & Searching Operations to Java APPs"
    content: |
       The amount of data and information is rapidly increasing with every passing day.  Therefore, it is very important to retrieve the correct information in a timely manner with minimum cost and effort. This webpage is going to provide information about how users can develop and add efficient documents searching capabilities to their business applications. . The aim is to quickly and accurately find and display information related to user’s queries.  GroupDocs.Search for Java is very efficient and simple to use Java API that helps software developers to operate basic to advanced level text search operations inside their own apps without installing any third party software.  The Java API has provided several useful features related to searching such as merge multiple indexes into a common index, search queries recognition of different keyboard layout, morphological Word Form support and so on.  It supports simple, Boolean, regular expression (Regex), fuzzy, case sensitive search, synonym, homophone, wildcard, object type search, setting data range and other types of queries to quickly and elegantly search out information.. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Create New Search Index or Load Existing One via Java"
      content_left: |
       GroupDocs.Search Java enables software developers to generate a new search Index or load an existing search index inside their own java apps. The below Java code example shows the creation of a new index as well as loading the existing one using just a couple of lines of java code. 

      title_right: "Create New or Load Existing Search Index via Java"
      content_right: |
         * First you need to Specify the path to the index folder
         * Create an instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
         * Above will create an index in memory or on a disk and can also load an existing index.
       
      gisthash: "02615fe51a919acdc5363d46c181dc7f"
      gistfile: "create_or_load_search_index.java"

    - title_left: "Synchronous DOTM Documents Indexing via Java"
      content_left: |
       GroupDocs.Search Java API facilitates software programmers to synchronously index documents with just a couple of lines of code inside their own Java apps. The below Java code examples demonstrates how to perform documents indexing synchronously with ease. 

      title_right: "Add DOTM Document to Search Index Synchronously"
      content_right: |
        * First you need to Specify the path to the index folder
        * Specify path to a folder containing documents to search
        * Create an instance of [Index(indexFolder)](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Above will create an index in memory or on a disk or open an existing index. 
        * Synchronous indexing documents from the specified folder
     
      gisthash: "7079bf3c06128a69b842150d080e5e0b"
      gistfile: "Add_files_synchronously_to_indexing.java"
      
    - title_left: "Perform Asynchronous Document Indexing  via Java"
      content_left: |
        GroupDocs.Search Java API allows software professionals to perform asynchronous document indexing inside their own Java apps. The below java code demonstrates how developers can index documents asynchronously with just a couple of lines of java code.

      title_right: "Add DOTM Document to Search Index Asynchronously"
      content_right: |
        * First you need to Specify the path to the index folder
        * Specify path to a folder containing documents to search
        * Create an instance of [Index(indexFolder)](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Subscribing to the event
        * Need to write Code indicating the completion of the operation
        * Setting the flag for asynchronous indexing 
        * Asynchronous indexing documents from the specified folder
     
      gisthash: "7079bf3c06128a69b842150d080e5e0b"
      gistfile: "Add_files_asynchronously_to_indexing.java"

    - title_left: "How to Highlight Search Results in Java Apps"
      content_left: |
       GroupDocs.Search Java API allows developers to interpret a search result and list down the found documents as well as the words and phrases. It is also possible to highlight the text of the DOTM document. Below is the Java code example that demonstrates how to list down the found documents and highlight search results with just a couple of lines of code.

      title_right: "Highlight Search Results via Java"
      content_right: |
        * Peform Search in index
        * After succesful Search, Print the result
        * Iterate through the documents and display the found documents
        * Highlighting occurrences in text
        * Generating output HTML formatted document with highlighted search results
     
      gisthash: "cc88d485f007d6da0d943043c8e13a52"
      gistfile: "how_to_highlight_search_result.java"

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