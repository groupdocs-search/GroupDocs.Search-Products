---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "search/java/filters/ppt"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Integrate PPT Document Filtering in Search Result via Java API?"
head_description: "GroupDocs.Search Java API helps software developers to add PPT documents searching capabilities & apply document filtering to customize search results via Java API."

############################# Header ############################
title: "How to Integrate Document Filtering to Customize Search Results inside Java Apps"
description: "GroupDocs.Search Java API allows programmers  to Integrate advanced PPT document searching functionalities as well as  customize searching results by setting document filtering in their Java apps."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "How to Integrate Document Filtering to Customize Search Results inside Java Apps"
    content: |
       Document filtering is a very useful activity that enables software applications to search & retrieve documents to the relevant sequence of words entered by a user in the text of indexed documents. A filter contains a set of rules that define criterion used to select records. The document filtering enables users to limit their search to a certain section or a particular document type as well as navigate through the results and find what they’re looking for. GroupDocs.Search for Java is feature rich high performance document indexing & searching API that enables software developer to create applications that can achieve text indexing and searching for some of the most popular documents file formats.  It fully supports various document types such as PDF, HTML, Outlook email, Microsoft Office Word, Excel worksheets, PowerPoint presentations, Outlook MSG, PST and so on.  There are various kinds of filers for available for user to customize the search results such as File path filters, file extension filter, attribute filter and many more. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Apply Document Filter in Searching PPT Documents via Java"
      content_left: |
       GroupDocs.Search Java API helps software developers to create powerful applications with searching capabilities using Java API. The below Java code example shows how to apply document filter for searching various kind of documents with just a couple of lines of code.

      title_right: "Document Filter Setting in Searching PPT Documents"
      content_right: |
       * First you need to Specify the path to the index folder & document folder.
       * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
       * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
       * Creating a search options object by calling [earchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions) class 
       * Set document filter by calling [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) method 
       * Start searching and display text documents if find any
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "Combine Search Document Filters to Create Composite Filter via Java"
      content_left: |
        GroupDocs.Search for Java allows software programmers to add advanced searching capability and apply custom filters for document searching inside their Java application. Users can create composite filter by combining various types of search filters. The following Java code demonstrates how to combine search document filters to create composite filter using Boolean operators AND, OR, NOT etc. with just a couple of lines of code.

      title_right: "Create Composite Filter to Search PPT Files"
      content_right: |
       * First you need to Specify the path to the index folder & document folder.
       * Creating an AND composite filter that returns all FB2 and EPUB documents that have the word 'Einstein' in their full paths
       * Create filter1 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Create filter2 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Combine filters by calling [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...)) method
       * Create an OR composite filter that returns all DOC, DOCX, PDF and all documents that have the word Einstein in their full paths
       * Create filter3 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Create filter4 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Combine filters by calling [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...)) method
       * Creating a filter that returns all found documents except of TXT documents
       * Create filter4 by calling [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))
       * Appy Not filter by calling [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter)) method

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
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