---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
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
head_title: "Node.js 문서, PDF, Office 및 웹을 위한 텍스트 검색 및 인덱싱 라이브러리"
head_description: "Node.js 애플리케이션을 위한 고급 텍스트 검색 솔루션으로 문서에서 데이터를 검색하고 인덱싱 및 수집합니다: PDF, Word, Excel, 발표, 이메일 및 웹 파일 형식."

############################# Header ############################
title: "Node.js API를 사용하여 문서 검색 및 인덱싱"
description: "Node.js 애플리케이션을 향상시켜 모든 인기 문서 형식에서 텍스트 검색을 구현합니다."
words:
  for: "을 위한"

actions:
  main: "NPM 무료 다운로드"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "라이센스"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "지금 시작하세요!"
  description: "모든 기능을 잠금 해제하려면 GroupDocs.Search의 기능을 무료로 탐색하거나 라이센스를 확보하십시오."

release:
  title: "버전 {0} 출시"
  notes: "새로운 기능 보기"
  downloads: "다운로드"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "JavaScript로 폴더에서 텍스트 검색 수행"
  more: "더 많은 예제"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // 문서의 인덱스 생성
    const index = new searchLib.Index('c:/MyIndex');

    // 효율적인 검색을 위해 인덱스에 문서 추가
    index.add('c:/MyDocuments');
    
    // 예를 들어, 특정 단어 또는 구문 검색
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 개요"
  description: "Node.js JavaScript 라이브러리로 텍스트 검색"
  features:
    # feature loop
    - title: "Node.js 인덱싱 및 검색 작업"
      content: "GroupDocs.Search for Node.js via Java에서 인덱싱은 데이터를 정확하고 효율적으로 수집, 저장 및 파싱하여 검색 운영을 수행합니다. 이 인덱스는 검색 수행에 자주 사용됩니다."

    # feature loop
    - title: "검색 효율성을 높이기 위해 여러 인덱스 병합"
      content: "GroupDocs.Search for Node.js via Java API는 여러 인덱스를 병합하여 하나로 만들 수 있습니다. 빈번한 수정으로 인해 여러 델타 인덱스가 생성될 수 있으며 이는 검색 성능을 저하시킬 수 있습니다. 우리의 솔루션은 이러한 델타 인덱스를 일반 인덱스로 병합하여 검색 효율성을 크게 향상시키는 동시에 델타 인덱스는 변경하지 않습니다. 다양한 기능을 구성하여 이 프로세스를 세부 조정할 수 있습니다."

    # feature loop
    - title: "다른 키보드 레이아웃에서 검색 쿼리 인식"
      content: "GroupDocs.Search for Node.js via Java는 키보드 레이아웃과 일치하지 않는 검색 쿼리를 인식합니다. 현재 88개 언어 및 164개의 키보드 레이아웃이 지원됩니다."

    # feature loop
    - title: "형태론적 단어 형태 검색"
      content: "GroupDocs.Search for Node.js via Java를 사용해서 다양한 단어 형태를 검색할 수 있습니다. 복수 및 단수 명사 또는 다양하게 변형된 동사를 사용해 검색할 수 있습니다. 영어 및 비영어 언어는 특정 단어 형태에 맞게 사용자 정의할 수 있습니다."

############################# Platforms ############################
platforms:
  enable: true
  title: "플랫폼 독립성"
  description: "GroupDocs.Search for Node.js via Java는 모든 인기 운영 체제 및 패키지 관리자를 지원합니다."
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
    GroupDocs.Search for Node.js via Java를 통해 다양한 파일 형식을 처리할 수 있습니다. [전체 목록 탐색](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
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
  title: "GroupDocs.Search for Node.js via Java 기능"
  description: "PDF, DOCX, XLSX, PPTX 및 기타 파일 형식에서 인기 있는 파일 형식을 지원하는 고급 검색 엔진을 통해 비즈니스 문서 콘텐츠를 제어하십시오."

  items:
    # feature loop
    - icon: "document_info"
      title: "유연한 매개변수"
      content: "검색 매개변수로 기간 및 대소문자 구분 사용"

    # feature loop
    - icon: "detect"
      title: "맞춤법 검사 검색"
      content: "특수 문자를 건너뛰고 검색 구문에 맞춤법 검사와 와일드카드를 사용하세요."

    # feature loop
    - icon: "collect"
      title: "결과 필터링"
      content: "검색 결과에서 문서 필터링을 설정합니다."

    # feature loop
    - icon: "get"
      title: "가져오기 및 내보내기"
      content: "인덱싱 중 문자 수정을 위해 가져오기 수행하거나 목록을 사용하고 파일로 내보내기"

    # feature loop
    - icon: "remove"
      title: "불필요한 데이터 건너뛰기"
      content: "특정 파일에 대한 인덱싱을 선택적으로 건너뛰고 특정 단어는 더 빠르게 인덱스할 수 있습니다."

    # feature loop
    - icon: "style"
      title: "URL 처리"
      content: "HTML 형식의 텍스트를 파일로 추출하고 검색 결과에서 HTML 내비게이션 URL을 생성합니다."

    # feature loop
    - icon: "detect"
      title: "신속한 검색"
      content: "더 빠른 대형 인덱스를 위해 검색을 더 작은 청크로 나눕니다."

    # feature loop
    - icon: "manipulate"
      title: "스트림 처리"
      content: "스트림 및 데이터 구조에서 문서 인덱싱"

    # feature loop
    - icon: "compare"
      title: "맞춤법 처리"
      content: "잘못된 철자의 경우 발생 횟수를 정확하게 제시하여 대체 단어 제안을 제공합니다."

    # feature loop
    - icon: "unreadable_characters"
      title: "아카이브 지원"
      content: "ZIP 아카이브 내의 압축 아카이브 인덱싱 및 아카이브 내 인덱스된 파일 목록 검색"

    # feature loop
    - icon: "hidden_print"
      title: "공간 절약형 인덱싱"
      content: "Compact indexing 및 암호 보호된 문서 인덱싱"

    # feature loop
    - icon: "style"
      title: "사용자 정의 동의어"
      content: "기본 동의어 사전에 영어 동의어 추가"

############################# Code samples ############################
code_samples:
  enable: true
  title: "코드 샘플"
  description: "GroupDocs.Search for Node.js via Java 기능을 예제를 통해 탐색하세요."
  items:
    # code sample loop
    - title: "생산성 향상을 위한 '모호' 검색 사용"
      content: |
        정교한 검색 알고리즘을 통해 문서 내용 제어를 향상시키는 GroupDocs.Search for Node.js via Java의 유연함을 즐기세요. [더 알아보기](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="검색 결과 처리 방법">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // 인덱스 생성
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // 검색 옵션 설정
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 단어 'water' 또는 구문 'Lorem ipsum'이 포함된 문서를 검색합니다.
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // 검색 결과 처리
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "고급 검색 시나리오에 대한 정규 표현식 사용 가능"
      content: |
        GroupDocs.Search for Node.js via Java는 검색 결과를 좁히기 위해 정규 표현식을 사용할 수 있습니다. [고급 검색 기술 알아보기](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="정규 표현식을 사용한 검색 방법">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // 인덱스 생성
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // 문자 형태로 구문 검색

        // 처음에 나타나는 캐럿 문자는 이것이 정규 표현식 검색 쿼리임을 나타냅니다.
        const query = '^^(.)\\1{1,}';
        // 단어 시작 부분에 두 개 이상의 동일한 문자를 검색
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
