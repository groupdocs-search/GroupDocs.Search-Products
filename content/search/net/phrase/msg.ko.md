---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/net/phrase/msg/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: ".NET 앱의 MSG 문서에 구문 검색을 추가하는 방법은 무엇입니까?"
head_description: "GroupDocs.Search .NET API를 사용하면 소프트웨어 전문가가 구문 검색을 추가하고 .NET API를 통해 MSG 문서에서 정확한 구문 또는 제공된 단어 시퀀스를 찾을 수 있습니다."

############################# Header ############################
title: ".NET 앱 내부의 MSG 문서에서 정확한 문장 또는 구 검색을 추가하시겠습니까?"
description: "GroupDocs.Search .NET API를 사용하면 프로그래머가 .NET 앱 내에서 구문 검색 또는 정확한 문장 검색을 통해 MSG 문서에서 제공된 단어 시퀀스를 찾을 수 있습니다. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NET 앱에서 정확한 문장 또는 구 검색을 사용하는 방법은 무엇입니까?"
    content: |
       정확한 문장 또는 구 검색은 사용자가 소비자가 정의한 특정 순서와 단어 조합을 포함하는 정확한 문장이나 구를 가진 문서, 웹 또는 데이터베이스를 검색할 수 있는 일종의 검색입니다. 이것은 검색 엔진 용어에서 매우 일반적인 용어이며 사용자가 색인된 문서의 텍스트에서 지정된 단어 시퀀스에 대해 문서를 검색할 수 있도록 합니다. GroupDocs.Search for .NET은 PDF, HTML, Outlook 전자 메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook MSG, PST 등. 여기에는 텍스트 및 개체 형식의 쿼리 검색, 구문 검색에서 와일드카드 사용 등과 같은 구문 검색과 관련된 여러 기능에 대한 지원이 포함되었습니다. 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET을 통해 MSG 문서에서 구문 검색을 수행하는 방법"
      content_left: |
       GroupDocs.Search .NET API를 사용하면 소프트웨어 개발자가 자신의 C# .NET 응용 프로그램 내에 구문 검색 기능을 추가할 수 있습니다. 다음 .NET 코드 예제는 몇 줄의 코드로 텍스트 및 개체에서 구문 검색을 수행하는 방법을 보여줍니다.

      title_right: "MSG 문서에서 정확한 구문 검색"
      content_right: |
         * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
         * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
         * 텍스트 형식의 구문 쿼리 '구문 텍스트' 검색
         * 객체 형태로 'phrase text'구를 검색
         * [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) 메서드를 호출하여 word1, word2 및 하위 쿼리 3 생성
         * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) 메서드를 호출하여 하위 쿼리를 결합하여 새 검색어 생성
         * 검색 시작 및 검색 결과 표시
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: ".NET을 통한 MSG 문서에서 와일드카드 구문 검색"
      content_left: |
        GroupDocs.Search for .NET을 사용하면 소프트웨어 프로그래머가 C# .NET 응용 프로그램 내에서 와일드카드를 사용하여 구문 검색 기능을 추가할 수 있습니다. 다음 .NET 코드 예제는 C# 애플리케이션 내의 MSG 문서에서 와일드카드 구문 검색을 적용하는 방법을 보여줍니다.

      title_right: "MSG 파일에서 와일드카드 구문 검색 적용"
      content_right: |
        * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
        * 텍스트 형식의 구문 쿼리 '구문 텍스트' 검색
        * 객체 형태로 'phrase text'구를 검색
        * [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery) 메서드를 호출하여 word1 생성 및 하위 쿼리 3 생성
        * [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) 메소드를 호출하여 wildcard2 생성
        * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) 메서드를 호출하여 하위 쿼리를 결합하여 새 검색어 생성
        * 검색 시작 및 검색 결과 표시
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: ".NET을 통해 다른 유형의 검색과 구문 검색 결합"
      content_left: |
        GroupDocs.Search .NET은 소프트웨어 프로그래머에게 .NET 응용 프로그램 내에서 다른 유형의 검색과 구문 검색을 결합할 수 있는 기능을 제공합니다. 다음 .NET 코드 예제는 단어를 나타내는 와일드카드와 단어의 문자를 모두 적용하는 방법을 보여줍니다.

      title_right: "구문 검색을 다른 검색과 결합하는 .NET API"
      content_right: |
        * 먼저 인덱스 폴더 및 문서 폴더의 경로를 지정해야 합니다.
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스를 호출하여 지정된 폴더에 인덱스 생성
        * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) 메서드를 호출하여 지정된 폴더에서 문서 인덱싱
        * 텍스트 형식의 구문 검색
        * 객체 형태의 구문 검색
        * 단어 패턴을 정의하고 문자열을 추가합니다.
        * [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery) 메소드를 호출하여 wordPattern1 생성 및 word3 생성
        * [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1) 메소드를 호출하여 wildcard2 생성
        * [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery) 메서드를 호출하여 하위 쿼리를 결합하여 새 검색어 생성
        * 검색 시작 및 검색 결과 표시
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

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