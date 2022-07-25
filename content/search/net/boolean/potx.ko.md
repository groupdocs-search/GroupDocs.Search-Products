---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/net/boolean/potx/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: ".NET을 통해 검색 쿼리에 부울 검색 연산자(AND, OR, NOT) 추가"
head_description: "GroupDocs.Search .NET API를 사용하면 소프트웨어 개발자가 .NET 앱 내부가 아닌 부울 연산자 AND, OR를 사용하여 부울 검색을 추가하거나 새 쿼리를 개발할 수 있습니다."

############################# Header ############################
title: ".NET 앱이 아닌 부울 연산자 AND, OR를 사용하여 복잡한 검색 쿼리 개발"
description: "GroupDocs.Search .NET API를 사용하면 컴퓨터 프로그래머가 .NET 응용 프로그램 내에서 부울 연산자(AND, OR, NOT)를 사용하여 복잡한 검색 쿼리를 개발할 수 있습니다."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "부울 검색이란 무엇이며 부울 연산자를 사용하는 방법은 무엇입니까?"
    content: |
       부울 검색은 사용자가 다양한 키워드를 연산자와 결합하여 검색 결과를 바인딩, 확장 및 정의할 수 있는 매우 유용한 검색 절차입니다. AND, OR, NOT, NEAR 등과 같은 부울 연산자는 사용자가 더 넓은 범위의 결과를 얻거나 제한을 정의하여 관련 없는 검색 결과의 수를 줄이는 데 도움이 됩니다. GroupDocs.Search for .NET은 소프트웨어 개발자가 PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트와 같은 가장 일반적인 문서 파일 형식 중 일부에서 텍스트 검색 및 인덱싱을 수행할 수 있는 응용 프로그램을 개발할 수 있도록 하는 강력한 고성능 문서 검색 API입니다. , PowerPoint 프레젠테이션, Outlook MSG, PST 등. 부울 AND 연산자는 입력한 모든 단어에 대한 결과를 표시하는 데 사용할 수 있고 OR 연산자는 입력한 단어에 대한 결과를 제공하며 NOT 연산자는 발생하지 않은 검색 결과를 표시하는 데 사용할 수 있습니다. 한 가지 훌륭한 기능은 키보드 레이아웃과 일치하지 않는 언어로 작성된 검색어를 인식할 수 있다는 것입니다. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET을 통한 검색 쿼리에서 부울 AND 연산자 사용"
      content_left: |
       GroupDocs.Search .NET API는 .NET 응용 프로그램 내부에 부울 검색 기능을 추가하기 위한 완벽한 지원을 제공합니다. 아래 C# 코드 예제에서는 자체 .NET 응용 프로그램 내에서 텍스트 및 개체 양식 쿼리에서 부울 "AND" 연산자를 만드는 방법을 보여줍니다.

      title_right: " 부울 연산자를 통해 POTX 문서 검색 AND"
      content_right: |
         * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
         * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
         * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 클래스를 호출하여 하위 쿼리 1 생성 및 하위 쿼리 2 생성
         * [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 하위 쿼리를 하나의 쿼리로 결합
         * 검색 시작 및 검색 결과 표시
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "부울 연산자 또는 .NET을 통해 사용하는 방법"
      content_left: |
       GroupDocs.Search for .NET은 소프트웨어 프로그래머가 널리 사용되는 여러 문서 형식을 검색할 수 있게 해주는 강력한 API입니다. 아래 C# .NET 코드 예제에서는 C# 응용 프로그램 내에서 텍스트 및 개체 양식 쿼리에서 부울 "OR" 연산자를 사용하는 방법을 보여줍니다.

      title_right: "부울 OR 연산자를 사용하여 POTX 파일 검색"
      content_right: |
        * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
        * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 클래스를 호출하여 하위 쿼리 1 생성 및 하위 쿼리 2 생성
        * [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) 메서드를 호출하여 하위 쿼리를 하나의 쿼리로 결합
        * 검색 시작 및 검색 결과 표시
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "부울 연산자를 사용하여 복잡한 검색 쿼리 만들기"
      content_left: |
        GroupDocs.Search .NET을 사용하면 컴퓨터 프로그래머가 다양한 부울 연산자를 결합하여 자신의 .NET 앱 내에서 복잡한 검색 쿼리를 만들 수 있습니다. 다음 .NET 코드 예제는 외부 소프트웨어나 도구를 설치하지 않고 복잡한 문서 검색 기능을 보여줍니다.

      title_right: "복잡한 검색어를 통해 POTX 문서 검색"
      content_right: |
        * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
        * 검색 시작 및 검색 결과 텍스트 쿼리 표시
        * 객체 쿼리로 검색
        * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 클래스를 호출하여 WordQuery 및 relativityWordQuery 생성
        * [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 하위 쿼리를 하나의 쿼리로 결합
        * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) 클래스를 호출하여 einsteinWordQuery 및 albertWordQuery 생성
        * [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) 메서드를 호출하여 하위 쿼리를 하나의 쿼리로 결합
        * [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) 메서드를 호출하여 하위 쿼리를 하나의 쿼리로 결합
        * 검색 시작 및 검색 결과 표시
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

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