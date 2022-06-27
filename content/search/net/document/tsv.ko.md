---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ko/search/net/document/tsv/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "문서 생성 및 추가 .NET 애플리케이션 내에서 검색 및 인덱싱"
head_description: "GroupDocs.Search .NET API를 사용하면 .NET 앱 내에서 PDF DOC, DOCX, RTF, XLSX, CSV, PPTX 및 이메일 메시지와 같은 지원 형식을 검색하는 인스턴트 문서를 추가할 수 있습니다."

############################# Header ############################
title: "C# .NET API를 통해 TSV에 인스턴트 문서 검색을 추가하는 방법 "
description: "GroupDocs.Search .NET API를 사용하면 개발자가 앱에 강력한 문서 검색 및 인덱싱 기능을 추가할 수 있습니다. PDF DOC, DOCX, RTF, XLSX, CSV, PPT, PPTX, MSG, EML 등과 같은 문서를 지원합니다. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NET API를 사용하여 문서 검색 및 인덱싱을 만들고 추가하는 방법은 무엇입니까?"
    content: |
       이 페이지는 사용자가 적은 노력과 비용으로 자신의 응용 프로그램에 문서 검색 및 인덱싱 기능을 추가하는 방법을 배우는 데 도움이 됩니다. 인덱싱은 관련 검색 결과를 생성할 수 있도록 데이터를 구성하고 구조화하는 검색 엔진에서 사용하는 프로세스입니다. 목표는 사용자의 쿼리와 관련된 정보를 빠르고 정확하게 찾아 표시하는 것입니다. GroupDocs.Search for .NET은 소프트웨어 개발자가 자체 응용 프로그램 내에서 퍼지 및 동의어 알고리즘을 기반으로 고급 검색 및 인덱싱 작업을 수행할 수 있도록 하는 강력한 고성능 문서 검색 API입니다. 사용자 컴퓨터에 타사 도구나 외부 소프트웨어를 설치할 필요가 없습니다. PDF, HTML, Outlook 이메일, Microsoft Office Word, Excel 워크시트, PowerPoint 프레젠테이션, Outlook MSG, PST 등과 같이 가장 일반적으로 사용되는 문서 형식에 대한 지원이 포함되어 있습니다. 단순 단어, 부울, 정규식 검색, 대소문자 구분 검색, 유연한 퍼지, 동의어, 동음이의어, 와일드카드, 청크별 검색, 객체 유형 검색, 데이터 범위 설정 등과 같은 여러 유형의 검색을 지원합니다.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET API를 통해 TSV 문서에 대한 검색 색인 생성"
      content_left: |
       GroupDocs.Search .NET API는 새 색인을 생성하거나 자체 앱 내에서 기존 검색 색인을 열기 위한 완벽한 지원을 제공합니다. 아래 C# 코드 예제는 몇 줄의 코드를 사용하여 새 인덱스를 만들고 기존 인덱스를 여는 방법을 보여줍니다.

      title_right: "새 검색 색인을 만들거나 기존 검색 색인을 여는 방법"
      content_right: |
         * 먼저 인덱스 폴더의 경로를 지정해야 합니다.
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) 클래스의 인스턴스 생성
         * 위는 메모리나 디스크에 인덱스를 생성하고 기존 인덱스를 열 수도 있습니다.
       
      gisthash: "9651c19a9436afee860b7f39197f8399"
      gistfile: "create_or_open_new_search_index.cs"

    - title_left: "검색 색인에 동기적으로 TSV 문서를 추가하는 방법"
      content_left: |
       GroupDocs.Search .NET을 사용하면 소프트웨어 개발자가 자체 .NET 앱 내에서 동기적으로 문서 인덱싱을 수행할 수 있습니다. 아래 C# .NET 코드 예제는 쉽게 동기적으로 인덱싱을 수행하는 방법을 보여줍니다. 

      title_right: "C#을 통한 동기식 문서 인덱싱"
      content_right: |
        * 먼저 인덱스 폴더의 경로를 지정해야 합니다.
        * 검색할 문서가 있는 폴더의 경로 지정
        * [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) 클래스의 인스턴스 생성
        * 위는 메모리나 디스크에 인덱스를 생성하거나 기존 인덱스를 엽니다.
        * 지정된 폴더에서 동기식 인덱싱 문서
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_synchronously_to_indexing.cs"
      
    - title_left: ".NET을 통해 비동기식으로 문서 인덱싱 수행"
      content_left: |
        GroupDocs.Search .NET을 사용하면 컴퓨터 프로그래머가 자신의 .NET 앱 내에서 비동기 문서 인덱싱을 수행할 수 있습니다. 다음 .NET 코드 예제는 몇 줄의 코드로 비동기식으로 문서 인덱싱을 수행하는 방법을 보여줍니다.

      title_right: "C#을 통한 비동기식 TSV 문서 인덱싱"
      content_right: |
        * 먼저 인덱스 폴더의 경로를 지정해야 합니다.
        * 검색할 문서가 있는 폴더의 경로 지정
        * [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) 클래스의 인스턴스 생성
        * 이벤트 신청
        * 작업 완료를 나타내는 코드 작성 필요
        * 비동기 인덱싱을 위한 플래그 설정
        * 지정된 폴더에서 문서를 비동기식으로 인덱싱
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_asynchronously_to_indexing.cs"

    - title_left: "TSV Docs .NET에서 검색 결과를 사용하고 강조 표시하는 방법"
      content_left: |
       GroupDocs.Search .NET API를 사용하면 프로그래머가 검색 결과를 해석하고 찾은 문서의 간단한 목록이나 찾은 단어와 구로 결과를 표시할 수 있습니다. 문서의 텍스트를 쉽게 강조 표시할 수도 있습니다. 다음 .NET 코드 예제는 몇 줄의 코드로 찾은 문서를 나열하고 검색 결과를 강조 표시하는 방법을 보여줍니다.

      title_right: "C#을 통해 TSV 파일에서 검색 결과 강조 표시 "
      content_right: |
        * 색인에서 검색 수행
        * 검색 성공 후 결과 출력
        * 문서를 반복하고 찾은 문서 표시
        * 텍스트의 강조 표시
        * 강조 표시된 검색 결과로 출력 HTML 형식 문서 생성
     
      gisthash: "a5d1ad6eedd2acf12a33b541e763cdb4"
      gistfile: "how_to_list_search_result.cs"

    - title_left: "시스템 요구 사항"
      content_left: |
       GroupDocs.Search for .NET은 모든 주요 플랫폼 및 운영 체제에서 지원됩니다. 전체 시스템 요구 사항 가이드를 보려면 아래 코드를 실행하기 전에 [시스템 요구 사항](https://docs.groupdocs.com/search/net/system-requirements/)을 방문하십시오. 다음 전제 조건이 컴퓨터에 설치되어 있는지 확인하십시오. 체계:
         * 운영 체제: 마이크로소프트 윈도우, 리눅스, 맥OS
         * 개발 환경: Visual Studio, Xamarin, MonoDevelop 등
         * 프레임워크: .NET Framework, .NET Standard, .NET Core, Mono
         * 최신 버전의 GroupDocs.Search for .NET API를 [NuGet](https://www.nuget.org/packages/GroupDocs.search/)에서 가져옵니다.
        
      title_right: "GroupDocs.Assembly를 사용하는 이유"
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