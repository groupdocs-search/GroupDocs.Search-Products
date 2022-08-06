---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/java/case-sensitive/dotm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB8 

############################# Head ############################
head_title: "DOTM 문서에서 대소문자 구분 텍스트 검색을 수행하는 Java API"
head_description: "GroupDocs.Search Java API를 사용하면 프로그래머가 대소문자를 구분하는 텍스트 검색을 수행하고 Java를 통해 DOTM 문서에서 단어의 정확한 구조를 찾을 수 있습니다."

############################# Header ############################
title: "Java 앱에서 DOTM 문서를 통해 대소문자 구분 검색 수행"
description: "GroupDocs.Search Java API를 사용하면 소프트웨어 개발자가 Java 앱에서 PDF, HTML, DOCX, PPTX, XLSX 등과 같은 다양한 문서 유형을 통해 대소문자 구분 텍스트 검색을 적용할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java 앱에서 대소문자 구분 검색을 수행하는 방법은 무엇입니까?"
    content: |
      대소문자 구분은 웹, 데이터베이스 또는 문서 검색에서 대문자(대문자)와 소문자(소문자)를 구별하는 프로그램의 기능을 설명하는 매우 유용한 검색 기술입니다. 기본적으로 검색 엔진은 대소문자를 구분하지 않는다는 점을 기억하는 것이 중요합니다. 즉, Computer라는 단어를 검색하면 키 이름이 있는 두 조각 또는 Computer와 computer라는 단어가 있는 텍스트가 모두 표시됩니다. 대소문자를 구분하는 검색이 필요함을 의미하는 대문자 'Computer'로 검색 결과를 좁혀야 한다고 가정해 보겠습니다. GroupDocs.Search for Java는 소프트웨어 개발자가 PDF, HTML, Outlook 전자 메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook MSG, PST 등. 또한 키보드 레이아웃과 일치하지 않는 언어로 작성된 검색어를 식별할 수 있습니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java를 통한 DOTM 문서의 대소문자 구분 검색"
      content_left: |
       GroupDocs.Search Java API는 기본 및 고급 검색 기능에 대한 완전한 지원을 통합하여 소프트웨어 개발자가 몇 줄의 코드로 Java 애플리케이션 내에서 대소문자를 구분하여 검색할 수 있도록 합니다.
       
       다음 Java 코드 예제는 몇 줄의 코드로 DOTM 파일의 텍스트에서 쿼리를 사용하여 대소문자 구분 검색을 수행하는 방법을 보여줍니다.

      title_right: "DOTM 파일에서 대소문자 구분 검색 수행"
      content_right: |
         * 색인 폴더와 문서 폴더의 경로를 식별합니다.
         * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
         * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 클래스의 인스턴스를 호출하여 지정된 폴더에서 문서 인덱싱
         * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 클래스의 새 인스턴스 시작
         * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) 메서드를 호출하여 대소문자 구분 검색 옵션 활성화
         * 검색 쿼리 정의 및 검색 시작
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Java를 통해 개체 형식에서 대소문자 구분 검색 만들기"
      content_left: |
        GroupDocs.Search Java는 소프트웨어 개발자에게 자신의 응용 프로그램 내에서 다양한 문서 형식에 대한 검색 기능을 포함할 수 있는 기능을 제공합니다. 다음 Java 코드 예제는 DOTM 문서를 통해 개체 형식의 쿼리로 대소문자 구분 검색을 수행하는 방법을 보여줍니다.

      title_right: "DOTM 문서에서 대소문자 구분 검색 적용"
      content_right: |
        * 색인 폴더와 문서 폴더의 경로를 식별합니다.
        * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 클래스의 인스턴스를 호출하여 지정된 폴더에서 문서 인덱싱
        * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 클래스의 새 인스턴스 시작
        * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch) 메서드를 호출하여 대소문자 구분 검색 옵션 활성화
        * [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String)) 메소드를 호출하여 객체에 검색어 생성
        * 검색 쿼리 정의 및 검색 시작
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

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