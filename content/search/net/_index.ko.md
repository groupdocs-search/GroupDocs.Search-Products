---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: ko
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: ".NET PDF, Office 파일 및 기타에 대한 문서 검색 및 인덱싱 라이브러리"
head_description: "PDF, Word, Excel, 발표, 이메일 및 웹 형식과 같은 문서에서 텍스트 검색 및 인덱싱을 위한 강력한 .NET 솔루션."

############################# Header ############################
title: ".NET API로 고급 문서 검색 및 인덱싱"
description: ".NET 애플리케이션에 인기 문서 형식의 최첨단 텍스트 검색 기능을 추가하십시오."
words:
  for: "을 위한"

actions:
  main: "Nuget 무료 다운로드"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "라이센스"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "지금 시작하세요!"
  description: "모든 기능을 잠금 해제하려면 GroupDocs.Search의 기능을 무료로 탐색하거나 라이센스를 확보하십시오."

release:
  title: "버전 {0} 출시"
  notes: "새로운 기능 보기"
  downloads: "다운로드"

code:
  title: "디렉토리 파일의 텍스트 검색"
  more: "더 많은 예제"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // 문서의 인덱스 생성
    Index index = new Index("c:/MyIndex");

    // 효율적인 검색을 위해 인덱스에 문서 추가
    index.Add("c:/MyDocuments");
    
    // 예를 들어, 특정 단어 또는 구문 검색
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 개요"
  description: ".NET C# 라이브러리를 통해 강력한 텍스트 검색 및 인덱싱을 탐색하십시오."
  features:
    # feature loop
    - title: ".NET 인덱싱 및 검색 기능"
      content: "GroupDocs.Search for .NET를 사용하여 문서 데이터를 효율적으로 인덱싱, 저장 및 처리하여 매우 정확하고 빠른 검색 작업을 수행합니다."

    # feature loop
    - title: "검색 속도 향상을 위한 인덱스 결합"
      content: "GroupDocs.Search for .NET를 사용하여 여러 인덱스를 병합하여 성능을 최적화하십시오. 델타 인덱스의 영향을 줄이기 위해 여러 인덱스를 포괄적인 인덱스로 결합하여 더 원활한 검색을 할 수 있습니다."

    # feature loop
    - title: "다양한 키보드 레이아웃간 검색"
      content: "GroupDocs.Search for .NET의 지능형 인식을 통해 88개 언어와 164개의 키보드 레이아웃에서 검색 쿼리를 쉽게 처리하십시오."

    # feature loop
    - title: "형태론적 단어 검색"
      content: "GroupDocs.Search for .NET는 단수/복수 명사 및 다양한 동사 형태와 같은 단어 변형에 대한 검색을 지원하며, 다양한 언어에 맞게 사용자 정의할 수 있습니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Search for .NET는 주요 운영 체제와 패키지 관리자를 통해 원활하게 작동합니다."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    GroupDocs.Search for .NET를 사용하여 다양한 파일 형식을 처리하십시오. [지원되는 모든 형식 보기](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### 인기 사무용 형식
        * **휴대용:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **텍스트:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### 미디어 형식
        * **인기 이미지 형식:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **다중 페이지 이미지:** GIF, WEBP, TIFF
        * **오디오:** MP3, WAV
        * **비디오:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### 기타
        * **이메일:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **웹:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **기타:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for .NET의 주요 기능"
  description: "PDF, DOCX, XLSX, PPTX 등과 같은 인기 형식에서 고급 검색 기능으로 문서 관리를 간소화하십시오."

  items:
    # feature loop
    - icon: "document_info"
      title: "유연한 검색 매개변수"
      content: "기간 및 대소문자 구분과 같은 필터를 사용하여 검색을 세분화하십시오."

    # feature loop
    - icon: "detect"
      title: "스마트 맞춤법 검사"
      content: "맞춤법 수정, 와일드카드 및 무시할 특수 문자로 검색 구문을 처리하십시오."

    # feature loop
    - icon: "collect"
      title: "필터링된 검색 결과"
      content: "문서 유형이나 기준에 따라 검색 결과를 사용자 정의하고 필터링하십시오."

    # feature loop
    - icon: "get"
      title: "인덱스 가져오기 및 내보내기"
      content: "데이터를 가져오고 인덱싱 설정을 수정하며 인덱싱된 결과를 내보내십시오."

    # feature loop
    - icon: "remove"
      title: "관련 없는 데이터 제외"
      content: "특정 파일이나 단어를 건너뛰어 인덱싱을 최적화하십시오."

    # feature loop
    - icon: "style"
      title: "URL 추출"
      content: "HTML 형식의 텍스트를 파일로 변환하고 검색 결과에 대한 링크를 생성하십시오."

    # feature loop
    - icon: "detect"
      title: "고속 검색"
      content: "대용량 인덱스를 더 작은 부분으로 나누어 처리 속도를 높이십시오."

    # feature loop
    - icon: "manipulate"
      title: "데이터 스트림 처리"
      content: "데이터 스트림 및 구조에서 직접 문서를 인덱싱하십시오."

    # feature loop
    - icon: "compare"
      title: "맞춤법 오류 감지"
      content: "대체 단어를 제안하고 발생 횟수를 추적하여 정확성을 향상시키십시오."

    # feature loop
    - icon: "unreadable_characters"
      title: "아카이브 지원"
      content: "중첩된 ZIP 아카이브를 인덱싱하고 그 안의 파일 세부정보를 검색하십시오."

    # feature loop
    - icon: "hidden_print"
      title: "효율적인 인덱싱"
      content: "Compact indexing으로 디스크 공간을 절약하고 암호 보호 문서를 처리하십시오."

    # feature loop
    - icon: "style"
      title: "사용자 정의 동의어"
      content: "맞춤 검색 결과를 위해 동의어를 추가하고 관리하십시오."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "GroupDocs.Search for .NET의 강력한 기능을 실제 예제로 발견하십시오."
  items:
    # code sample loop
    - title: "모호 검색으로 생산성 향상"
      content: |
        고급 검색 알고리즘을 통해 유연하고 정확한 콘텐츠 제어를 위해 GroupDocs.Search for .NET를 활용하십시오. [자세히 알아보기](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="검색 결과 처리 방법">}}
        ```csharp {style=abap}
        // 인덱스 생성
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // 검색 옵션 설정
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // 단어 'water' 또는 구문 'Lorem ipsum'이 포함된 문서를 검색합니다.
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // 검색 결과 처리
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "정규 표현식을 사용한 고급 검색"
      content: |
        GroupDocs.Search for .NET는 정확한 검색을 위해 정규 표현식을 지원합니다. [고급 기술 알아보기](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="정규 표현식을 사용한 검색 방법">}}
        ```csharp {style=abap}   
        // 인덱스 생성
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // 문자 형태로 구문 검색

        // 처음에 나타나는 캐럿 문자는 이것이 정규 표현식 검색 쿼리임을 나타냅니다.
        string query = "^^(.)\\1{1,}";
        // 단어 시작 부분에 두 개 이상의 동일한 문자를 검색
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
