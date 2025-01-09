---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: ko
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Java PDF, Office 파일 및 웹 콘텐츠에 대한 문서 검색 및 인덱싱 솔루션"
head_description: "Java 애플리케이션을 위한 강력한 텍스트 검색 및 인덱싱. PDF, Word, Excel, 발표, 이메일 및 웹 형식에서 데이터를 쉽게 검색하고 구성하십시오."

############################# Header ############################
title: "Java API로 효율적인 문서 검색 및 인덱싱"
description: "Java 애플리케이션을 모든 인기 문서 형식에서 강력한 텍스트 검색 기능으로 응원하십시오."
words:
  for: "을 위한"

actions:
  main: "Maven 무료 다운로드"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "라이센스"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "지금 시작하세요!"
  description: "모든 기능을 잠금 해제하려면 GroupDocs.Search의 기능을 무료로 탐색하거나 라이센스를 확보하십시오."

release:
  title: "버전 {0} 출시"
  notes: "새로운 기능 보기"
  downloads: "다운로드"

code:
  title: "Java를 사용하여 파일에서 텍스트 찾기"
  more: "더 많은 예제"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // 문서의 인덱스 생성
    Index index = new Index("c:/MyIndex");

    // 효율적인 검색을 위해 인덱스에 문서 추가
    index.add("c:/MyDocuments");
    
    // 예를 들어, 특정 단어 또는 구문 검색
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 개요"
  description: "Java Java 라이브러리의 강력한 텍스트 검색 기능을 발견하십시오."
  features:
    # feature loop
    - title: "Java에서의 인덱싱 및 검색 작업"
      content: "GroupDocs.Search for Java를 사용하여 데이터를 효율적으로 수집, 저장 및 분석하여 더 빠르고 더 정확한 검색을 위한 상세 인덱스를 생성할 수 있습니다."

    # feature loop
    - title: "인덱스를 병합하여 검색 최적화"
      content: "GroupDocs.Search for Java로 여러 인덱스를 쉽게 결합하여 검색을 간소화하십시오. 작은 델타 인덱스의 영향을 줄이기 위해 이를 단일 고성능 인덱스로 통합하십시오."

    # feature loop
    - title: "다국어 키보드 레이아웃 지원"
      content: "GroupDocs.Search for Java로 다양한 언어와 키보드 레이아웃을 통해 검색하십시오. 88개 언어 및 164개의 키보드 구성으로 비교할 수 없는 다재다능성을 갖추고 있습니다."

    # feature loop
    - title: "형태론적 검색 기능"
      content: "GroupDocs.Search for Java를 사용하여 단수/복수 명사 및 동사 변형과 같은 다양한 단어 형태를 찾으십시오. 검색 옵션은 영어 및 기타 언어에 맞게 사용자 정의할 수 있습니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Search for Java는 주요 운영 체제 및 패키지 관리자가 호환됩니다."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "지원되는 파일 형식"
  description: |
    포괄적인 형식 범위를 사용할 수 있습니다. [전체 목록 보기](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "GroupDocs.Search for Java의 기능"
  description: "PDF, DOCX, XLSX, PPTX 등과 같은 형식을 지원하는 고급 검색 기능으로 문서 콘텐츠를 효과적으로 관리하십시오."

  items:
    # feature loop
    - icon: "document_info"
      title: "사용자 정의 가능한 검색 매개변수"
      content: "기간 범위 및 대소문자 구분 필터를 사용하여 검색을 세분화하십시오."

    # feature loop
    - icon: "detect"
      title: "향상된 맞춤법 검사"
      content: "효율적으로 검색하기 위해 맞춤법 검사, 와일드카드 및 특수 문자를 무시하십시오."

    # feature loop
    - icon: "collect"
      title: "필터링된 검색 결과"
      content: "특정 문서 유형 또는 기준에 기반하여 검색 결과를 필터링하십시오."

    # feature loop
    - icon: "get"
      title: "인덱스 데이터 가져오기 및 내보내기"
      content: "인덱싱을 위한 데이터를 쉽게 가져오고, 결과를 파일로 내보내십시오."

    # feature loop
    - icon: "remove"
      title: "불필요한 파일 건너뛰기"
      content: "특정 파일이나 단어를 제외하여 인덱싱을 최적화합니다."

    # feature loop
    - icon: "style"
      title: "HTML 및 URL 처리"
      content: "HTML 내용을 파일로 추출하고 검색 결과를 통해 내비게이션하는 URL을 생성하십시오."

    # feature loop
    - icon: "detect"
      title: "대형 인덱스에서 고속 검색"
      content: "크고 관리하기 쉬운 청사진을 나누어 놓을 수 있는 방법을 사용할 수 있습니다."

    # feature loop
    - icon: "manipulate"
      title: "스트림 기반 인덱싱"
      content: "스트림 또는 데이터 구조에서 직접 데이터를 인덱싱하십시오."

    # feature loop
    - icon: "compare"
      title: "잘못된 쿼리 처리"
      content: "잘못된 철자 및 대체 단어를 제안하여 더 나은 검색 정확성을 기초하십시오."

    # feature loop
    - icon: "unreadable_characters"
      title: "포괄적인 아카이브 지원"
      content: "모든 ZIP 파일 내에서 중첩 아카이브를 인덱싱하고 파일의 세부사항을 검색하십시오."

    # feature loop
    - icon: "hidden_print"
      title: "공간 절약형 인덱싱"
      content: "디스크 공간을 절약할 수 있는 컴팩트한 인덱싱으로 사용하고 암호 보호된 문서를 처리하십시오."

    # feature loop
    - icon: "style"
      title: "사용자 지정 동의어 지원"
      content: "동의어 사전을 확대하여 맞춰진 옵션으로 검색 정확도를 향상시키십시오."

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "코드 예제를 통해 GroupDocs.Search for Java의 기능을 살펴보십시오."
  items:
    # code sample loop
    - title: "모호 일치를 통해 검색 정확성 향상"
      content: |
        고급 모호 검색 기능으로 콘텐츠를 관리하기 위해 GroupDocs.Search for Java의 유연함을 활용하십시오. [더 알아보기](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="검색 결과 처리 방법">}}
        ```java {style=abap}
        // 인덱스 생성
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // 검색 옵션 설정
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 단어 'water' 또는 구문 'Lorem ipsum'이 포함된 문서를 검색합니다.
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // 검색 결과 처리
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "정규 표현식으로 결과 세분화"
      content: |
        GroupDocs.Search for Java에서 정규 표현식을 사용하여 정밀하고 상세한 검색을 수행하십시오. [고급 기술 탐색](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="정규 표현식을 사용한 검색 방법">}}
        ```java {style=abap}   
        // 인덱스 생성
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // 문자 형태로 구문 검색

        // 처음에 나타나는 캐럿 문자는 이것이 정규 표현식 검색 쿼리임을 나타냅니다.
        String query = "^^(.)\\1{1,}";
        // 단어 시작 부분에 두 개 이상의 동일한 문자를 검색
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
