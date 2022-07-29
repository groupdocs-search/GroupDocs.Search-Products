---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/net/case-sensitive/dot/"
otherformats: PDF DOC DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: ".NET을 통해 DOT 문서를 통해 대소문자 구분 텍스트 검색 적용"
head_description: "GroupDocs.Search .NET API를 사용하면 소프트웨어 프로그래머가 대소문자를 구분하는 텍스트 검색을 적용하고 .NET API를 통해 DOT 문서에서 정확한 단어 시퀀스를 찾을 수 있습니다."

############################# Header ############################
title: ".NET 앱 내에서 DOT 문서를 통해 대소문자 구분 검색을 적용하는 방법은 무엇입니까?"
description: "GroupDocs.Search .NET API를 사용하면 소프트웨어 개발자가 .NET 앱 내에서 PDF, HTML, DOCX, PPTX, XLSX 등과 같은 다양한 문서 유형을 통해 대소문자 구분 텍스트 검색을 적용할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "대소문자 구분 검색이란 무엇이며 .NET을 통해 검색하는 방법은 무엇입니까?"
    content: |
      사용자가 다양한 유형의 문서에서 단어 또는 기타 데이터의 특정 조합을 검색하는 데 도움이 되는 유용한 검색 기술이 많이 있습니다. 대소문자 구분 검색은 사용자가 대문자와 소문자가 다른지 또는 같은지 여부에 관계없이 문서 및 웹 페이지를 검색할 수 있는 매우 유용한 기술입니다. 예를 들어 "Computer", "computer" 및 "COMPUTER"는 문자 "C"가 첫 번째 경우 대문자, 두 번째 경우 소문자, 세 번째 경우 모두 대문자이기 때문에 다른 단어로 처리됩니다. GroupDocs.Search for .NET은 편리한 고성능 문서 검색 API로, 소프트웨어 작성자가 텍스트 검색과 문서 인덱싱을 쉽게 수행할 수 있는 소프트웨어 응용 프로그램과 도구를 만들 수 있습니다. API는 PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook MSG, PST 등과 같이 가장 일반적으로 사용되는 파일 형식을 지원합니다. 또 다른 유용한 기능은 키보드 레이아웃과 일치하지 않는 언어로 작성된 검색어를 식별할 수 있다는 것입니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET을 통해 DOT 문서에서 대소문자 구분 검색 수행"
      content_left: |
       GroupDocs.Search .NET API를 사용하면 소프트웨어 프로그래머가 자체 C# .NET 응용 프로그램 내부에 대소문자 구분 검색 기능을 추가할 수 있습니다. 다음 .NET 코드 예제는 몇 줄의 코드로 DOT 파일의 텍스트 형식 쿼리를 사용하여 대소문자 구분 검색을 수행하는 방법을 보여줍니다.

      title_right: "DOT 문서에서 대소문자 구분 검색 적용"
      content_right: |
         * 색인 폴더와 문서 폴더의 경로를 식별합니다.
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
         * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 클래스의 인스턴스를 호출하여 지정된 폴더에서 문서 인덱싱
         * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다.
         * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecaseSensitivesearch) 메서드를 호출하여 대소문자 구분 검색b 활성화
         * 검색 문자열 정의 및 검색 시작
         
        
      gisthash: "805df69ebb1145d5c15c212431de1395"
      gistfile: "case-sensitive_in_text_queries_dotnet.cs"

    - title_left: ".NET을 통해 개체 형식에서 대소문자 구분 검색 수행"
      content_left: |
        GroupDocs.Search .NET은 소프트웨어 개발자에게 .NET 응용 프로그램 내에서 대문자와 소문자를 염두에 두고 단어를 검색할 수 있는 기능을 제공합니다. 다음 .NET 코드 예제는 DOT 문서에서 개체 형식의 쿼리로 대소문자 구분 검색을 적용하는 방법을 보여줍니다.

      title_right: "DOT 문서에서 대소문자 구분 검색"
      content_right: |
        * 색인 폴더와 문서 폴더의 경로를 식별합니다.
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1) 클래스의 인스턴스를 호출하여 지정된 폴더에서 문서 인덱싱
        * [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions) 클래스의 새 인스턴스를 초기화합니다.
        * [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecaseSensitivesearch) 메서드를 호출하여 대소문자 구분 검색b 활성화
        * [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) 메소드를 호출하여 객체 형태의 검색어 생성
        * 검색 시작 및 검색 결과 표시
     
      gisthash: "846d0dd11f88a59d62f083e33e84286b"
      gistfile: "case-sensitive_search_in_object_queries_dotnet.cs"

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