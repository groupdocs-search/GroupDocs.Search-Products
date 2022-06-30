---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/java/document/msg"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Java 앱 내부에 문서 인덱싱 및 검색 작업 추가"
head_description: "GroupDocs.Search Java API는 PDF DOC, DOCX, RTF, XLSX, CSV, PPTX, EML, MSG 등과 같은 문서 형식에 대한 문서 인덱싱 및 검색 작업을 지원합니다."

############################# Header ############################
title: "MSG 문서 인덱싱 및 검색 작업을 위한 Java API"
description: "GroupDocs.Search Java API를 사용하면 개발자가 강력한 문서 검색 및 색인 작업을 앱에 통합할 수 있습니다. PDF DOC, DOCX, RTF, XLSX, CSV, PPTX MSG, EML 등의 파일 형식을 지원합니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "Java APP에 문서 인덱싱 및 검색 작업을 추가하는 방법"
    content: |
       데이터와 정보의 양은 날이 갈수록 빠르게 증가하고 있습니다. 따라서 최소한의 비용과 노력으로 적시에 정확한 정보를 검색하는 것이 매우 중요합니다. 이 웹 페이지는 사용자가 효율적인 문서 검색 기능을 개발하고 비즈니스 응용 프로그램에 추가하는 방법에 대한 정보를 제공합니다. . 목표는 사용자의 쿼리와 관련된 정보를 빠르고 정확하게 찾아 표시하는 것입니다. GroupDocs.Search for Java는 소프트웨어 개발자가 타사 소프트웨어를 설치하지 않고도 자체 앱 내에서 기본에서 고급 수준의 텍스트 검색 작업을 수행하는 데 도움이 되는 Java API를 사용하는 것이 매우 효율적이고 간단합니다. Java API는 여러 색인을 공통 색인으로 병합, 다른 키보드 레이아웃의 검색 쿼리 인식, 형태학적 워드 형식 지원 등과 같은 검색과 관련된 몇 가지 유용한 기능을 제공했습니다. 단순, 부울, 정규식(Regex), 퍼지, 대소문자 구분 검색, 동의어, 동음이의어, 와일드카드, 개체 유형 검색, 데이터 범위 설정 및 기타 유형의 쿼리를 지원하여 정보를 빠르고 우아하게 검색합니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java를 통해 새 검색 색인 생성 또는 기존 색인 로드"
      content_left: |
       GroupDocs.Search Java를 사용하면 소프트웨어 개발자가 새 검색 색인을 생성하거나 자체 Java 앱 내부에 기존 검색 색인을 로드할 수 있습니다. 아래 Java 코드 예제는 몇 줄의 Java 코드를 사용하여 기존 인덱스를 로드하는 것 뿐만 아니라 새 인덱스를 생성하는 방법을 보여줍니다.

      title_right: "Java를 통해 새 검색 색인 생성 또는 기존 검색 색인 로드"
      content_right: |
         * 먼저 인덱스 폴더의 경로를 지정해야 합니다.
         * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스 생성
         * 위는 메모리나 디스크에 인덱스를 생성하고 기존 인덱스를 로드할 수도 있습니다.
       
      gisthash: "02615fe51a919acdc5363d46c181dc7f"
      gistfile: "create_or_load_search_index.java"

    - title_left: "Java를 통한 동기식 MSG 문서 색인 생성"
      content_left: |
       GroupDocs.Search Java API를 사용하면 소프트웨어 프로그래머가 자체 Java 앱 내에서 단 몇 줄의 코드로 문서를 동기식으로 인덱싱할 수 있습니다. 아래 Java 코드 예제는 문서 인덱싱을 동기식으로 쉽게 수행하는 방법을 보여줍니다.

      title_right: "MSG 문서를 검색 색인에 동기적으로 추가"
      content_right: |
        * 먼저 인덱스 폴더의 경로를 지정해야 합니다.
        * 검색할 문서가 있는 폴더의 경로 지정
        * [Index(indexFolder)](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스 생성
        * 위는 메모리나 디스크에 인덱스를 생성하거나 기존 인덱스를 엽니다.
        * 지정된 폴더에서 동기식 인덱싱 문서
     
      gisthash: "7079bf3c06128a69b842150d080e5e0b"
      gistfile: "Add_files_synchronously_to_indexing.java"
      
    - title_left: "Java를 통해 비동기 문서 인덱싱 수행"
      content_left: |
        GroupDocs.Search Java API를 사용하면 소프트웨어 전문가가 자체 Java 앱 내에서 비동기 문서 인덱싱을 수행할 수 있습니다. 아래 자바 코드는 개발자가 몇 줄의 자바 코드로 비동기식으로 문서를 인덱싱하는 방법을 보여줍니다.

      title_right: "비동기식으로 검색 색인에 MSG 문서 추가"
      content_right: |
        * 먼저 인덱스 폴더의 경로를 지정해야 합니다.
        * 검색할 문서가 있는 폴더의 경로 지정
        * [Index(indexFolder)](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) 클래스의 인스턴스 생성
        * 이벤트 신청
        * 작업 완료를 나타내는 코드 작성 필요
        * 비동기 인덱싱을 위한 플래그 설정
        * 지정된 폴더에서 문서를 비동기식으로 인덱싱
     
      gisthash: "7079bf3c06128a69b842150d080e5e0b"
      gistfile: "Add_files_asynchronously_to_indexing.java"

    - title_left: "Java 앱에서 검색 결과를 강조 표시하는 방법"
      content_left: |
       GroupDocs.Search Java API를 사용하면 개발자가 검색 결과를 해석하고 찾은 문서와 단어 및 구를 나열할 수 있습니다. MSG 문서의 텍스트를 강조 표시하는 것도 가능합니다. 다음은 몇 줄의 코드로 찾은 문서를 나열하고 검색 결과를 강조 표시하는 방법을 보여주는 Java 코드 예제입니다.

      title_right: "Java를 통한 검색 결과 강조 표시"
      content_right: |
        * 색인에서 검색 수행
        * 검색 성공 후 결과 출력
        * 문서를 반복하고 찾은 문서 표시
        * 텍스트의 강조 표시
        * 강조 표시된 검색 결과로 출력 HTML 형식 문서 생성
     
      gisthash: "cc88d485f007d6da0d943043c8e13a52"
      gistfile: "how_to_highlight_search_result.java"

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