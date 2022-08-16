---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/java/filters/xltm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Java API를 통해 검색 결과에 XLTM 문서 필터링을 통합하시겠습니까?"
head_description: "GroupDocs.Search Java API를 사용하면 소프트웨어 개발자가 XLTM 문서 검색 기능을 추가하고 문서 필터링을 적용하여 Java API를 통해 검색 결과를 사용자 정의할 수 있습니다."

############################# Header ############################
title: "Java 앱 내에서 검색 결과를 사용자 정의하기 위해 문서 필터링을 통합하는 방법"
description: "GroupDocs.Search Java API를 사용하면 프로그래머가 고급 XLTM 문서 검색 기능을 통합하고 Java 앱에서 문서 필터링을 설정하여 검색 결과를 사용자 정의할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java 앱 내에서 검색 결과를 사용자 정의하기 위해 문서 필터링을 통합하는 방법"
    content: |
       문서 필터링은 소프트웨어 응용 프로그램이 색인된 문서의 텍스트에서 사용자가 입력한 관련 단어 시퀀스에 대해 문서를 검색 및 검색할 수 있도록 하는 매우 유용한 활동입니다. 필터에는 레코드를 선택하는 데 사용되는 기준을 정의하는 규칙 집합이 포함되어 있습니다. 문서 필터링을 통해 사용자는 검색을 특정 섹션이나 특정 문서 유형으로 제한하고 결과를 탐색하고 원하는 것을 찾을 수 있습니다. GroupDocs.Search for Java는 소프트웨어 개발자가 텍스트 인덱싱을 수행하고 가장 인기 있는 문서 파일 형식 중 일부를 검색할 수 있는 응용 프로그램을 만들 수 있도록 하는 기능이 풍부한 고성능 문서 인덱싱 및 검색 API입니다. PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook MSG, PST 등과 같은 다양한 문서 유형을 완벽하게 지원합니다. 사용자가 파일 경로 필터, 파일 확장자 필터, 속성 필터 등과 같은 검색 결과를 사용자 정의할 수 있는 다양한 종류의 파일러가 있습니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java를 통해 XLTM 문서 검색에 문서 필터 적용"
      content_left: |
       GroupDocs.Search Java API는 소프트웨어 개발자가 Java API를 사용하여 검색 기능을 갖춘 강력한 응용 프로그램을 만들 수 있도록 도와줍니다. 아래 자바 코드 예제는 몇 줄의 코드만으로 다양한 종류의 문서를 검색하기 위해 문서 필터를 적용하는 방법을 보여줍니다.

      title_right: "XLTM 문서 검색 시 문서 필터 설정"
      content_right: |
       * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
       * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
       * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
       * [searchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions) 클래스를 호출하여 검색 옵션 객체 생성
       * [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) 메서드를 호출하여 문서 필터 설정
       * 검색을 시작하고 텍스트 문서를 찾으면 표시
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "Combine Search Document Filters to Create Composite Filter via Java"
      content_left: |
        GroupDocs.Search for Java allows software programmers to add advanced searching capability and apply custom filters for document searching inside their Java application. Users can create composite filter by combining various types of search filters. The following Java code demonstrates how to combine search document filters to create composite filter using Boolean operators AND, OR, NOT etc. with just a couple of lines of code.

      title_right: "XLTM 파일 검색을 위한 복합 필터 생성"
      content_right: |
       * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
       * 전체 경로에 'Einstein'이라는 단어가 있는 모든 FB2 및 EPUB 문서를 반환하는 AND 복합 필터 만들기
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))를 호출하여 filter1 생성
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))를 호출하여 filter2 생성
       * [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...)) 메서드를 호출하여 필터 결합
       * 전체 경로에 Einstein이라는 단어가 포함된 모든 DOC, DOCX, PDF 및 모든 문서를 반환하는 OR 복합 필터 만들기
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))를 호출하여 filter3 생성
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))를 호출하여 filter4 생성
       * [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...)) 메서드를 호출하여 필터 결합
       * TXT 문서를 제외한 모든 발견된 문서를 반환하는 필터 만들기
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter))를 호출하여 filter4 생성
       * [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter)) 메서드를 호출하여 필터링하지 않음 적용

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
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