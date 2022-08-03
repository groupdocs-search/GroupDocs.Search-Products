---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/java/phrase/dot/"
otherformats: PDF DOC DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: "DOT 문서에서 정확한 구문을 검색하고 찾기 위한 Java API"
head_description: "GroupDocs.Search Java API는 프로그래머가 구문 검색을 포함하고 자바를 통해 DOT 문서의 텍스트에서 주어진 단어 또는 정확한 구문을 검색할 수 있도록 도와줍니다."

############################# Header ############################
title: "Java API를 통해 DOT 문서에서 정확한 문장 또는 구문을 검색하고 보는 방법은 무엇입니까?"
description: "GroupDocs.Search Java API는 고급 검색 기능을 완벽하게 지원하여 소프트웨어 개발자가 구문 검색 또는 정확한 문장 검색을 통해 DOT 문서에서 정확한 문장이나 구문을 검색할 수 있도록 합니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "구문 검색이란 무엇이며 Java 앱에서 사용하는 방법은 무엇입니까?"
    content: |
       구문 검색은 문서나 웹 페이지 내에서 키워드가 아닌 정확한 문장이나 구문을 검색하는 매우 효과적인 방법입니다. 이는 사용자가 정확한 구문을 검색할 때 나타나는 특정 순서로 모든 검색어를 찾고 싶어 함을 의미합니다. 이 웹 페이지는 사용자가 Java API를 사용하여 효율적인 문서 및 웹 페이지 검색을 위한 비즈니스 응용 프로그램 및 도구를 개발하는 방법에 대한 정보를 공유합니다. GroupDocs.Search for Java는 소프트웨어 개발자가 타사 소프트웨어를 설치하지 않고도 자체 앱 내에서 기본에서 고급 수준의 텍스트 검색 작업을 수행할 수 있도록 하는 매우 잘 조직되고 효율적인 Java API입니다. API에는 단순 또는 부울 검색, 퍼지, 대소문자 구분 검색, 동의어, 동음이의어, 와일드카드, 개체 유형 검색, 데이터 범위 설정 및 기타 유형의 쿼리와 같은 문서 검색과 관련된 수많은 유용한 기능이 포함되어 있어 정보를 빠르고 우아하게 검색할 수 있습니다. 또한 키보드 레이아웃과 일치하지 않는 언어로 작성된 검색어 인식도 지원합니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java를 통해 DOT 문서에서 구문 검색 만들기"
      content_left: |
       GroupDocs.Search Java API에는 고급 검색에 대한 완벽한 지원이 포함되어 있어 소프트웨어 전문가가 검색 기능과 사용 편의성을 갖춘 강력한 소프트웨어 응용 프로그램을 만들 수 있습니다. 아래 Java 코드는 몇 줄의 코드로 텍스트 및 개체 형식의 Phrase 검색을 수행하는 방법을 보여줍니다.

      title_right: "DOT 파일에서 정확한 문장 검색"
      content_right: |
         * 인덱스 폴더 및 문서 폴더의 경로를 정의합니다.
         * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
         * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
         * [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) 메소드를 호출하여 텍스트 쿼리로 검색
         * 객체 형태로 'phrase text'구를 검색
         * [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) 메서드를 호출하여 word1, word2 생성 및 하위 쿼리 3 생성
         * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...))를 호출하여 하위 쿼리를 결합하여 새 검색어를 만듭니다. 방법
         * 검색 시작 및 검색 결과 표시
         
        
      gisthash: "396c41cda822cf79f31dd37c6740fa03"
      gistfile: "phrase_search_in_text_queries_java.java"

    - title_left: "Java를 통해 DOT 파일을 통해 와일드카드 구문 검색 적용"
      content_left: |
        GroupDocs.Search for Java는 소프트웨어 프로그래머에게 Java 애플리케이션 내에서 DOT 파일을 검색하는 동안 와일드카드 구문 검색 기능을 추가할 수 있는 기능을 제공합니다. 다음 Java 코드 예제는 Java API를 사용하여 다양한 문서 유형에서 와일드카드 구문 검색을 적용하는 방법을 보여줍니다.

      title_right: "Java에서 와일드카드를 사용한 구 검색"
      content_right: |
        * 인덱스 폴더 및 문서 폴더의 경로를 정의합니다.
        * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
         * [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) 메소드를 호출하여 텍스트 쿼리로 검색
         * 객체 형태로 'phrase text'구를 검색
         * [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) 메소드를 호출하여 word1, word3 생성
         * [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) 메소드를 호출하여 wildcard2 생성
         * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) 를 호출하여 하위 쿼리를 결합하여 새 구문 검색 쿼리 생성 ) 방법
         * 검색 시작 및 검색 결과 표시
     
      gisthash: "f21c8c4572883fecc0eeef82c2b814b1"
      gistfile: "use_wildcards_in_phrase_search_java.java"
      
    - title_left: "구문 검색 및 기타 유형의 검색을 결합하는 Java API"
      content_left: |
        GroupDocs.Search Java API를 사용하면 소프트웨어 프로그래머가 구문 검색을 다른 유형의 검색과 쉽게 결합할 수 있습니다. 다음 Java 코드는 단어와 단어의 문자를 나타내는 와일드카드를 통해 구 검색을 수행하는 방법을 보여줍니다.

      title_right: "구문 검색 및 기타 검색을 결합하는 방법"
      content_right: |
        * 인덱스 폴더 및 문서 폴더의 경로를 정의합니다.
        * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
         * [Search](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#search(com.groupdocs.search.SearchQuery)) 메소드를 호출하여 텍스트 쿼리로 검색
         * 객체 형태로 'phrase text'구를 검색
        * 단어 패턴 정의 및 문자열 추가 및 와일드카드 추가
        * [CreateWordPatternQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordPatternQuery(com.groupdocs.search.common.WordPattern)) 메소드를 호출하여 wordPattern1 생성 및 word3 생성
        * [createWildcardQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWildcardQuery(int,%20int)) 메소드를 호출하여 wildcard2 생성
        * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createPhraseSearchQuery(com.groupdocs.search.SearchQuery...)) 를 호출하여 하위 쿼리를 결합하여 새로운 구문 검색 쿼리 생성 ) 방법
        * 검색 시작 및 검색 결과 표시
     
      gisthash: "dbd0f2eb292796e63e6213461f080e0c"
      gistfile: "combine_phrase_search_with_others_java.java"

    - title_left: "시스템 요구 사항"
      content_left: |
       GroupDocs.Search for Java는 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 전체 시스템 요구 사항 가이드를 보려면 아래 코드를 실행하기 전에 [시스템 요구 사항](https://docs.groupdocs.com/search/java/system-requirements/)을 방문하십시오. 다음 전제 조건이 컴퓨터에 설치되어 있는지 확인하십시오. 체계:
         * 운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
         * 자바 버전 지원: J2SE 7.0(1.7), J2SE 8.0(1.8) 이상
         * GroupDocs[Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)에서 최신 버전의 GroupDocs.Search for Java API 다운로드
        
      title_right: "GroupDocs.Search를 사용하는 이유"
      content_right: |
        * 메모리와 디스크에서 검색 인덱스 생성.
        * 파일, 스트림 또는 구조에서 인덱싱하는 기능.
        * 암호로 보호된 문서 색인 생성 지원.
        * 여러 인덱스 병합 지원.
        * 검색 인덱싱 중에 문서를 필터링합니다.
        * 검색 중 맞춤법 검사 지원.
        * 혼합 문자가 완전히 지원됩니다.
        * 다양한 검색 유형을 하나의 검색어로 결합합니다.
        * 간단한 단어 및 정규식 검색 지원
        * 검색 쿼리에서 별칭 대체를 완벽하게 지원합니다.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---