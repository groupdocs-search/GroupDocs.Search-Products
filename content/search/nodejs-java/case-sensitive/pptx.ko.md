
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:33
draft: false
lang: ko
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PPTX에서 Node.js를 사용하여 대소문자를 구분하는 검색 수행하기"
head_description: "GroupDocs.Search for Node.js via Java API는 JavaScript 개발자가 다양한 문서 유형에서 대소문자를 구분하는 검색을 수행할 수 있도록 지원합니다."

############################# Header ############################
title: "대소문자 구분 검색" 
description: "GroupDocs.Search for Node.js via Java를 사용하면 Node.js 애플리케이션에서 대소문자를 구분하는 고급 검색 기능을 구현할 수 있습니다."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search란?"
    link: "/search/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)는 문서 내 텍스트 검색 및 인덱싱을 위한 강력한 라이브러리입니다. PDF, Word, Excel, PowerPoint, 이미지 및 ZIP 파일을 포함하여 70개 이상의 형식을 지원하여 대량의 데이터를 효율적으로 처리합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 파일에서 대소문자 구분 검색 수행하기 위한 단계"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)를 사용하면 PPTX 파일에서 대소문자 구분 검색을 수행하여 Node.js via Java 워크플로우를 향상시킬 수 있습니다.
      
      1. 검색 인덱스를 저장할 폴더를 설정합니다.
      2. PPTX 파일이 포함된 폴더를 선택합니다.
      3. 검색을 실행하고 결과를 받습니다.
      4. 결과를 처리하고 사용합니다.
   
    code:
      platform: "nodejs-java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "복사하려면 클릭"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // 인덱스 폴더의 경로를 지정합니다.
        const index = new searchLib.Index("c:/MyIndex");

        // 검색할 문서가 포함된 폴더를 설정합니다.
        index.add("c:/MyDocuments");

        // 설정에서 대소문자 구분 검색을 활성화합니다.
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // 검색을 실행합니다.
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 검색 및 인덱싱을 위한 주요 기능"
  description: "GroupDocs.Search for Node.js via Java을 사용하면 70개 이상의 파일 형식에서 텍스트를 쉽게 검색하고 인덱싱할 수 있습니다. 고급 검색 도구를 사용하여 정보를 손쉽게 액세스하고 정리하세요."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search의 핵심 기능"
  features:
    # feature loop
    - title: "포괄적인 텍스트 검색"
      content: "PDF, Word 파일, 스프레드시트 및 프레젠테이션과 같은 다양한 문서 유형에서 텍스트를 찾습니다. 정확한 결과를 위해 정확한 일치, 퍼지 검색 및 와일드카드와 같은 옵션을 사용하십시오."

    # feature loop
    - title: "효율적인 데이터 인덱싱"
      content: "검색 속도를 높이기 위해 인덱스를 생성하고 관리합니다. 인덱싱은 대규모 문서 컬렉션에서 데이터를 조직하고 빠르게 찾도록 도와줍니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 문서를 검색할 수 있으며 다양하고 다채로운 키보드 레이아웃 및 단어 변형을 지원하여 정확한 검색 결과를 보장합니다."

    # feature loop
    - title: "사용자 정의 가능한 검색 설정"
      content: "대소문자 구분, 날짜 필터 및 인덱싱 중 특정 용어나 데이터를 제외하는 등의 검색 설정을 조정하세요."
      
  code_samples_ext:
    # code sample ext loop
    - title: "예제: 대소문자 구분 검색 구현"
      content: |
        이 예제는 PPTX 문서에 대한 대소문자 구분 검색을 수행하는 방법을 보여줍니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 검색 인덱스를 위한 폴더를 정의합니다.
          const index = new searchLib.Index("c:/MyIndex");
              
          // 문서 폴더의 경로를 제공합니다.
          index.add("c:/MyDocuments");

          // 검색 쿼리를 설정합니다.
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // 대소문자 구분 검색 설정을 활성화합니다.
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // 문서에서 텍스트를 검색합니다.
          const result = index.search(wordQuery, options);
          
          // 결과를 처리하고 다룹니다.
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "복사"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "복사하려면 클릭"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.pptx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "문서화"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨습니까?"
  description: "GroupDocs.Search 기능을 무료로 시험해 보거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "NPM 다운로드"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "라이센스"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "주요 기능"
    exclude: "case-sensitive"
    description: "빠르고 정밀한 문서 검색을 위한 고급 기능을 탐색하세요."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "호환 가능한 문서 형식"
    exclude: "PPTX"
    description: "GroupDocs.Search는 70개 이상의 문서 형식을 지원합니다. 검색 옵션을 사용자 정의하고 인덱싱으로 시간을 절약하세요."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Microsoft Word Open XML 문서"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Adobe 휴대용 문서 형식"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "PowerPoint Open XML 프레젠테이션"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Microsoft Excel Open XML 스프레드시트"
  

---