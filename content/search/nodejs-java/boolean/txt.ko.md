
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: ko
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "TXT 문서에 대한 불리언 검색 Node.js"
head_description: "GroupDocs.Search for Node.js via Java API를 사용하여 AND, OR, NOT과 같은 불리언 연산자를 사용해 문서 내용에서 고급 검색을 수행하세요. 이는 JavaScript 개발자를 위해 맞춤 제작되었습니다."

############################# Header ############################
title: "불리언 논리 검색 수행" 
description: "GroupDocs.Search for Node.js via Java을 사용하면 Node.js 환경 내에서 불리언 연산자(AND, OR, NOT)를 사용하여 고급 검색 쿼리를 쉽게 생성할 수 있습니다."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "지금 다운로드"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search란?"
    link: "/search/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)는 문서 내 텍스트 검색 및 인덱싱을 위한 강력한 도구입니다. PDF, Word, Excel, PowerPoint, 이미지, ZIP 파일 등 70개 이상의 포맷을 지원하여 대량의 정보를 효율적으로 처리할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "TXT 문서에서 불리언 연산자를 사용하여 검색하는 방법"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)는 TXT 파일의 내용을 효과적으로 검색할 수 있게 해줍니다. 불리언 논리를 통해 Node.js via Java 애플리케이션 내에서 검색 쿼리를 세밀하게 조정하여 정확성을 향상시킬 수 있습니다.
      
      1. 검색 인덱스를 저장할 폴더를 설정합니다.
      2. TXT 파일이 포함된 폴더를 선택합니다.
      3. 검색 쿼리를 실행하고 결과를 가져옵니다.
      4. 검색 결과를 처리하고 분석합니다.
   
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

        // 인덱스 폴더의 위치 설정
        const index = new searchLib.Index("c:/MyIndex");

        // 검색할 문서가 있는 폴더 지정
        index.add("c:/MyDocuments");

        // 고급 논리와 함께 검색 쿼리 실행
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 검색 및 인덱싱을 위한 강력한 도구"
  description: "GroupDocs.Search for Node.js via Java은 70개 이상의 파일 유형에 대한 텍스트 검색 및 인덱싱을 간소화하여 정보를 더 빠르고 정확하게 찾고 관리하는 데 도움을 줍니다."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "향상된 텍스트 검색"
      content: "PDF, Word 문서, 프레젠테이션, 스프레드시트 등 다양한 포맷에서 텍스트를 신속하게 찾습니다. 정확한 결과를 위해 정확한 일치, 와일드카드 검색 및 퍼지 검색과 같은 기능을 활용할 수 있습니다."

    # feature loop
    - title: "효율적인 데이터 인덱싱"
      content: "대량의 문서 컬렉션에서 검색 속도를 높이기 위해 인덱스를 구축하고 관리하세요. 인덱싱은 데이터에 대한 빠르고 구조화된 액세스를 보장합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 작성된 문서에서 검색할 수 있습니다. 형태론적 지원 및 키보드 레이아웃 호환성이 다양한 언어에서 검색 결과를 향상시킵니다."

    # feature loop
    - title: "유연한 검색 설정"
      content: "대소문자 구분을 활성화하거나 날짜 필터를 적용하거나 인덱싱 중 특정 단어 및 데이터를 건너뛰는 등의 방법으로 검색을 사용자 정의할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 불리언 검색의 예"
      content: |
        이 예제는 TXT 문서에서 내용을 검색하기 위한 불리언 기반 쿼리를 생성하는 방법을 보여줍니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 검색 인덱스를 위한 폴더 정의
          const index = new searchLib.Index("c:/MyIndex");
              
          // 검색할 문서의 위치 제공
          index.add("c:/MyDocuments");

          // 불리언 연산자를 사용하여 쿼리 구축
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // 검색 결과 가져오기
          const result = index.search(booleanQuery);
          
          // 검색 결과 처리 및 사용
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "GroupDocs.Search의 주요 기능"
    exclude: "boolean"
    description: "고급, 효율적이며 사용자 정의 가능한 검색 기능을 활용하세요."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "인기 문서 포맷 검색"
    exclude: "TXT"
    description: "GroupDocs.Search는 70개 이상의 파일 포맷을 지원하며, 유연한 검색 규칙과 효율적인 인덱싱을 통해 시간과 노력을 절약합니다."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Microsoft Word Open XML 문서"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Adobe 휴대용 문서 형식"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "PowerPoint Open XML 프레젠테이션"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Microsoft Excel Open XML 스프레드시트"
  

---