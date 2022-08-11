---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/net/filters/epub/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML CHM FB2 

############################# Head ############################
head_title: ".NET 앱에서 문서 필터링을 설정하여 검색 결과 사용자 지정"
head_description: "GroupDocs.Search .NET API를 사용하면 소프트웨어 개발자가 EPUB 문서 문서를 검색하고 .NET 앱에서 문서 필터링을 적용하여 검색 결과를 사용자 지정할 수 있습니다."

############################# Header ############################
title: ".NET 앱 내에서 검색 결과를 사용자 지정하도록 문서 필터링 설정"
description: "GroupDocs.Search .NET API는 소프트웨어 전문가가 문서 검색 기능을 추가하고 .NET 앱 내부에 문서 필터링을 적용하여 검색 결과를 사용자 지정할 수 있도록 도와줍니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NET을 통해 검색 결과에 문서 필터링을 적용하는 방법은 무엇입니까?"
    content: |
      필터링은 사용자가 기능을 검사하고 처리할 수 있는 매우 유용한 기술입니다. 문서 필터링은 사용자에게 결과를 탐색하고 원하는 것을 쉽게 찾을 수 있는 방법을 제공합니다. 또한 사용자에게 특정 섹션이나 특정 문서 유형으로 검색을 제한할 수 있는 권한을 제공합니다. GroupDocs.Search for .NET은 소프트웨어 개발자가 텍스트 검색 및 인덱싱을 수행할 수 있는 응용 프로그램을 빌드할 수 있도록 하는 기능이 풍부한 고성능 문서 검색 API입니다. PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook MSG, PST 등과 같은 가장 널리 사용되는 문서 형식을 지원합니다. API는 검색 결과에 대한 문서 파일링 설정을 완벽하게 지원합니다. 여러 종류의 파일러를 사용하여 파일 경로 필터, 파일 확장자 필터, 속성 필터 등과 같은 검색 결과를 사용자 정의할 수 있습니다. 부울 연산자 AND, OR & NOT 등을 사용하여 검색 문서 필터를 결합하는 것도 가능합니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET을 통해 EPUB 문서 검색에서 문서 필터 설정"
      content_left: |
       GroupDocs.Search .NET API는 소프트웨어 개발자가 .NET 응용 프로그램 내부에 검색 기능을 추가하는 데 도움이 됩니다. 다음 .NET 코드 예제는 몇 줄의 코드로 다양한 종류의 문서를 검색할 때 문서 필터를 적용하는 방법을 보여줍니다.

      title_right: "EPUB 문서 검색 시 문서 필터 적용"
      content_right: |
       * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
       * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
       * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
       * 검색 옵션 객체 생성 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)를 호출하여 문서 필터 설정
       * 검색 시작 및 검색 결과 표시
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: ".NET을 통해 검색 문서 필터를 결합하는 방법"
      content_left: |
       .NET용 GroupDocs.Search를 사용하면 소프트웨어 프로그래머가 검색하는 동안 검색 문서 필터를 결합하여 C# .NET 응용 프로그램 내에서 검색한 결과로 반환되어야 하는 문서를 제어할 수 있습니다. 다음 .NET 코드 예제에서는 C# 응용 프로그램 내에서 부울 연산자 AND, OR, NOT 등을 사용하여 검색 문서 필터를 결합하는 방법을 보여줍니다.

      title_right: "EPUB 파일 검색에서 검색 문서 필터 결합"
      content_right: |
       * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
       * 전체 경로에 'Einstein'이라는 단어가 있는 모든 FB2 및 EPUB 문서를 반환하는 AND 복합 필터 만들기
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)를 호출하여 filter1 생성
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)를 호출하여 filter2 생성
       * [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand) 메소드를 호출하여 필터 결합
       * 전체 경로에 Einstein이라는 단어가 포함된 모든 DOC, DOCX, PDF 및 모든 문서를 반환하는 OR 복합 필터 만들기
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)를 호출하여 filter3 생성
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)를 호출하여 filter4 생성
       * [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor) 메소드를 호출하여 필터 결합
       * TXT 문서를 제외한 모든 발견된 문서를 반환하는 필터 만들기
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter)를 호출하여 filter4 생성
       * [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot) 메서드를 호출하여 필터링하지 않음 적용

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
    - title_left: "시스템 요구 사항"
      content_left: |
       GroupDocs.Search for .NET은 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 전체 시스템 요구 사항 가이드를 보려면 아래 코드를 실행하기 전에 [시스템 요구 사항](https://docs.groupdocs.com/search/net/system-requirements/)을 방문하십시오. 다음 전제 조건이 컴퓨터에 설치되어 있는지 확인하십시오. 체계:
         * 운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
         * 개발 환경: Visual Studio, Xamarin, MonoDevelop 등
         * 프레임워크: .NET Framework, .NET Standard, .NET Core, Mono
         * 최신 버전의 GroupDocs.Search for .NET API를 [NuGet](https://www.nuget.org/packages/GroupDocs.search/)에서 가져옵니다.
        
      title_right: "GroupDocs.Search 를 사용하는 이유"
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