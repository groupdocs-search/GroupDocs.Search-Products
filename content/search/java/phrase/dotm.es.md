---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/java/phrase/dotm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB8 

############################# Head ############################
head_title: "Java API to Search & Find Exact Phrase in DOTM Documents"
head_description: "GroupDocs.Search Java API helps programmers to embed Phrase search & discover a given sequence of words or exact phrase in the text of DOTM documents via Java."

############################# Header ############################
title: "How to Search & View Exact Sentence or Phrase in DOTM Documents via Java API?"
description: "GroupDocs.Search Java API has provided complete support for advanced searching capabilities empowering software developers to Search out exact sentence or phrase in DOTM documents via phrase search or exact sentence search."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "What is Phrase Search and How to Use It in Java Apps?"
    content: |
       Phrase search is a very effective way of searching inside documents or web pages for an exact sentence or phrase, rather than a keyword. It means when user search for an exact phrase, they want to find all the search terms in that particular order in which they appeared. This webpage is going share information about how users can develop business applications & tools for efficient documents & web pages searching using Java API. GroupDocs.Search for Java is very well-organized and efficient Java API that enables software developers to operate basic to advanced level text search operations inside their own apps without installing any third party software. The API has included numerous valuable features related to documents searching such as simple or Boolean search, fuzzy, case sensitive search, synonym, homophone, wildcard, object type search, setting data range and other types of queries to quickly and elegantly search out information. Moreover, it also supports the recognition of search queries written in a language that does not match your keyboard layout. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Make Phrase Search in DOTM Documents via Java"
      content_left: |
       GroupDocs.Search Java API has included complete support for advanced searching that enables software professionals to create powerful software applications with searching capabilities and ease of use. The below Java code shows how to perform Phrase search in text & object form with just a couple of lines of code.

      title_right: "Exact Sentence Search in DOTM Files"
      content_right: |
         * Define path to the index folder & document folder.
         * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
         * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
         * Search with text query by calling [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) method 
         * Search for the phrase 'phrase text' in object form
         * Creating word1, word2  and Creating subquery 3 by calling [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) method
         *  Combining subqueries to create new search query by calling [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) method 
         * Start searching and display search results
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "Apply Wildcards Phrase Search Through DOTM Files via Java"
      content_left: |
        GroupDocs.Search for Java gives software programmers the power to add wildcards phrase search functionality while searching DOTM files inside Java application. The following Java code examples demonstrates how to apply wildcards phrase search in various documents types using Java API. 

      title_right: "Phrase Search with Wildcards in Java"
      content_right: |
        * Define path to the index folder & document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
         * Search with text query by calling [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) method 
         * Search for the phrase 'phrase text' in object form
         * Creating word1  and word3 by calling [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) method
         * Creating wildcard2 by calling [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) method
         *  Combining subqueries to create new phrase search query by calling [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) method 
         * Start searching and display search results
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "Java API to Combine Phrase Search & Other Types of Searches"
      content_left: |
        GroupDocs.Search Java API allows software programmers to combine phrase search with other types of searches with ease. The following Java code shows how to perform phrase search via wildcards representing words and characters in words.

      title_right: "How to Combine Phrase Search & Other Searches"
      content_right: |
        * Define path to the index folder & document folder.
        * Creating an index in the specified folder by calling instance of [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) class
        * Indexing documents from the specified folder by calling [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) method 
         * Search with text query by calling [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) method 
         * Search for the phrase 'phrase text' in object form
        * Define Word Pattern and append string & append Wildcard to it
        * Creating wordPattern1 and Creating word3 by calling [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern)) method
        * Creating  wildcard2 by calling [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) method
        * Combining subqueries to create new phrase search query by calling [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) method 
        * Start searching and display search results
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

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