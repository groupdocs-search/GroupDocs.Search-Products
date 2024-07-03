---
############################# Static ############################
layout: "landing"
date: 2024-07-03T19:47:25
draft: false

lang: ko
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js 문서, PDF, Office 및 웹용 텍스트 검색 및 색인 라이브러리"
head_description: "PDF, Word, Excel, 프리젠테이션, 이메일 및 웹 파일 형식과 같은 문서에서 데이터를 검색, 색인화 및 수집하는 Node.js 애플리케이션용 고급 텍스트 검색 솔루션입니다."

############################# Header ############################
title: "Node.js API를 사용하여 문서 검색 및 색인 생성"
description: "모든 인기 있는 문서 형식에서 텍스트 검색을 구현하여 Node.js 애플리케이션을 향상시킵니다."
words:
  for: "~을 위한"

actions:
  main: "무료 NPM 다운로드"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "라이선스"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "시작할 준비가 되셨나요?"
  description: "GroupDocs.Search 기능을 무료로 사용해 보거나 라이선스를 요청하세요"

release:
  title: "버전 {0} 출시됨"
  notes: "새로운 소식 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "JavaScript으로 폴더에서 검색"
  more: "더 많은 예시"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // 색인 생성 중
    var index = new Index("c:\\MyIndex");

    // 색인에 문서 추가
    index.addToIndex("c:\\MyDocuments");
    
    // 다음과 같은 다양한 단어를 검색합니다.
    // 'affect', 'effect', 'principles', 'principally'
    var results = index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 개요"
  description: "텍스트 검색을 위한 Node.js JavaScript 라이브러리"
  features:
    # feature loop
    - title: "Node.js 색인 생성 및 검색 작업"
      content: "GroupDocs.Search for Node.js via Java의 색인 생성은 정확하고 효율적인 검색 작업을 위해 데이터를 수집, 저장 및 구문 분석합니다. 이러한 인덱스는 검색을 수행하는 데 자주 사용됩니다."

    # feature loop
    - title: "여러 인덱스를 병합하여 검색 효율성 향상"
      content: "GroupDocs.Search for Node.js via Java API를 사용하면 여러 색인을 하나로 병합할 수 있습니다. 자주 수정하면 여러 델타 인덱스가 생성되어 검색 성능이 저하될 수 있습니다. 우리의 솔루션은 이러한 델타 인덱스를 병합된 델타 인덱스의 모든 정보를 포함하는 공통 인덱스로 병합하여 델타 인덱스를 변경하지 않고 유지하면서 검색 효율성을 크게 향상시킵니다. 이 프로세스를 미세 조정하기 위해 다양한 기능을 구성할 수 있습니다."

    # feature loop
    - title: "다양한 키보드 레이아웃의 검색어 인식"
      content: "GroupDocs.Search for Node.js via Java은 키보드 레이아웃과 일치하지 않는 검색어를 인식합니다. 현재 88개 언어와 164개 키보드 레이아웃이 지원됩니다."

    # feature loop
    - title: "형태론적 단어 형식을 사용하여 검색"
      content: "GroupDocs.Search for Node.js via Java을(를) 사용하면 단수 및 복수 명사, 모든 형태의 동사 등 다양한 단어 형태를 검색할 수 있습니다. 영어와 영어가 아닌 언어는 특정 단어 형식에 맞게 사용자 정의할 수 있습니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Search for Node.js via Java은 널리 사용되는 모든 운영 체제 및 패키지 관리자를 지원합니다."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    GroupDocs.Search for Node.js via Java을(를) 사용하면 다양한 파일 형식을 처리할 수 있습니다. [전체 목록 살펴보기](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### 인기 있는 Office 형식
        * **가지고 다닐 수 있는:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **텍스트:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### 미디어 형식
        * **인기 있는 이미지 형식:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **다중 페이지 이미지:** GIF, WEBP, TIFF
        * **오디오:** MP3, WAV
        * **동영상:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### 다른
        * **이메일:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **편물:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **기타:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java 기능"
  description: "PDF, DOCX, XLSX, PPTX 등 널리 사용되는 파일 형식을 지원하는 고급 검색 엔진을 사용하여 비즈니스 문서 콘텐츠를 제어하세요."

  items:
    # feature loop
    - icon: "document_info"
      title: "유연한 매개변수"
      content: "날짜 범위 및 대소문자 구분을 검색 매개변수로 사용"

    # feature loop
    - icon: "detect"
      title: "맞춤법 검사 검색"
      content: "맞춤법 검사 및 와일드카드와 함께 검색 문구 사용 및 쿼리에서 특수 문자 건너뛰기"

    # feature loop
    - icon: "collect"
      title: "결과 필터링"
      content: "검색 결과에서 문서 필터링 설정"

    # feature loop
    - icon: "get"
      title: "수입 수출"
      content: "인덱싱 및 파일로 내보내기 중에 문자 수정을 위해 가져오기 또는 목록 사용 수행"

    # feature loop
    - icon: "remove"
      title: "불필요한 데이터 건너뛰기"
      content: "특정 파일에 대한 인덱싱을 선택적으로 건너뛰고 특정 단어를 건너뛰어 더 빠르게 인덱싱합니다."

    # feature loop
    - icon: "style"
      title: "URL 처리"
      content: "HTML 형식의 텍스트를 파일로 추출하고 URL을 생성하여 HTML에서 검색 결과 탐색"

    # feature loop
    - icon: "detect"
      title: "신속한 검색"
      content: "큰 인덱스를 빠르게 검색하기 위해 검색을 더 작은 청크로 나누기"

    # feature loop
    - icon: "manipulate"
      title: "스트림 처리"
      content: "스트림 및 데이터 구조의 문서 색인"

    # feature loop
    - icon: "compare"
      title: "철자 오류 처리"
      content: "철자가 틀린 경우 대체 단어 제안을 제공하기 위해 발견된 각 단어에 대해 정확한 발생 횟수를 활성화합니다."

    # feature loop
    - icon: "unreadable_characters"
      title: "아카이브 지원"
      content: "다른 ZIP 아카이브 내의 압축된 아카이브 색인화 및 아카이브에서 색인화된 파일 목록 검색"

    # feature loop
    - icon: "hidden_print"
      title: "디스크 공간 절약"
      content: "컴팩트 색인 및 색인 비밀번호 보안 문서로 공간 절약"

    # feature loop
    - icon: "style"
      title: "사용자 정의 동의어"
      content: "기본 동의어 사전에 영어 동의어 추가"

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "예시를 통해 GroupDocs.Search for Node.js via Java 기능 살펴보기"
  items:
    # code sample loop
    - title: "퍼지 검색을 사용하여 생산성 향상"
      content: |
        정교한 검색 알고리즘을 통해 문서 콘텐츠 제어를 강화하는 유연한 GroupDocs.Search for Node.js via Java 기능을 즐겨보세요. [자세히 알아보기](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="검색결과 처리 방법">}}
        ```javascript {style=abap}
        // 색인 만들기
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");

        // 검색 옵션 설정
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 'water'라는 단어 또는 'Lorem ipsum'이라는 문구가 포함된 문서를 검색합니다.
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // 프로세스 검색 결과
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "고급 검색 시나리오에 정규식을 사용할 수 있습니다."
      content: |
        GroupDocs.Search for Node.js via Java에서는 검색 결과 범위를 좁히기 위해 정규 표현식을 사용할 수 있습니다. [고급 검색 기술을 살펴보세요](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="정규식을 사용하여 검색하는 방법">}}
        ```javascript {style=abap}   
        // 색인 만들기
        var index = new Index("C:\\IndexFolder");
        index.add("C:\\DocumentFolder");
 
        // 텍스트 형태로 문구 검색

        // 시작 부분의 첫 번째 캐럿 문자는 이것이 정규식 검색 쿼리임을 나타냅니다.
        var query = "^^(.)\\1{1,}";
        // 단어 시작 부분에서 두 개 이상의 동일한 문자를 검색합니다.
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
