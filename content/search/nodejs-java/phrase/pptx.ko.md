
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: ko
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PPTX에서 구문 검색하기 - GroupDocs.Search for Node.js via Java"
head_description: "GroupDocs.Search for Node.js via Java은 JavaScript 애플리케이션에 효율적인 문서 검색을 위한 강력한 구문 검색 기능을 추가합니다."

############################# Header ############################
title: "문서에서 구문 찾기" 
description: "GroupDocs.Search for Node.js via Java을(를) 사용하여 특정 구문을 신속하게 찾으세요. 빠르고 정확한 검색 기능을 Node.js 애플리케이션에 통합하십시오."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "다운로드"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search의 기능"
    link: "/search/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)은 문서 내 텍스트를 색인화하고 검색하기 위한 고성능 라이브러리입니다. PDF, Word 문서, Excel 스프레드시트, 이미지, ZIP 아카이브를 포함하여 70개 이상의 파일 형식을 지원하여 정확하고 빠른 검색 결과를 보장합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 문서에서 구문 찾는 방법"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)을(를) 사용하면 PPTX 문서에서 구문 검색을 수행할 수 있습니다. Node.js via Java 애플리케이션에서 결과를 정제하기 위해 다양한 검색 옵션을 적용하십시오.
      
      1. 검색 색인 폴더를 설정하십시오.
      2. PPTX 파일이 포함된 폴더를 정의하십시오.
      3. 검색 매개변수를 구성하십시오.
      4. 검색 결과를 검색하고 처리하십시오.
   
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

        // 검색 색인을 저장할 경로 지정
        const index = new searchLib.Index("c:/MyIndex");

        // 문서를 포함한 폴더 설정
        index.add("c:/MyDocuments");

        // 검색 설정 구성
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // 검색 쿼리 실행
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js 문서 검색 엔진 발견하기"
  description: "GroupDocs.Search for Node.js via Java은 70개 이상의 파일 형식에서 구문 검색을 가능하게 하여 고급 검색 기능을 통해 데이터를 쉽게 찾고 정리할 수 있습니다."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "구문 검색"
      content: "PDF, Word 파일, 프레젠테이션, 스프레드시트와 같은 비즈니스 문서에서 정확한 구문을 찾습니다. 전체 구문이 알려지지 않은 경우 와일드카드 및 유연한 검색 옵션을 사용하십시오."

    # feature loop
    - title: "최적화된 데이터 색인화"
      content: "재사용 가능한 색인을 생성하여 검색 성능을 높입니다. 구조화된 색인화는 문서 검색 속도를 높이고 정확성을 개선합니다."

    # feature loop
    - title: "다국어 호환성"
      content: "80개 이상의 언어로 문서를 검색하며 다양한 키보드 레이아웃과 형태소 단어 변형을 지원하여 정확한 결과를 보장합니다."

    # feature loop
    - title: "고급 검색 옵션"
      content: "대소문자 구분, 퍼지 매칭, 동음이의어 탐지, 문서 필터링 등 다양한 강력한 기능으로 검색을 사용자 설정합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 검색 기술 사용하기"
      content: |
        PPTX에서 검색 쿼리를 구성하는 방법을 배우십시오.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 검색 색인 디렉터리 정의
          const index = new searchLib.Index("c:/MyIndex");
              
          // 대상 문서에 대한 경로 설정
          index.add("c:/MyDocuments");

          // 원하는 구문에 대한 쿼리 생성
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // 검색 결과 검색
          const result = index.search(query);
          
          // 결과 처리 및 사용
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
            link: "/examples/search/formats/searchphrase.pptx"
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
    title: "고급 검색 기능"
    exclude: "phrase"
    description: "더 빠르고 정확한 결과를 위해 강력한 검색 기능을 활용하십시오."
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
    title: "비즈니스 문서에서 구문 검색하기"
    exclude: "PPTX"
    description: "GroupDocs.Search은 70개 이상의 문서 형식에서 구문 검색을 지원합니다. 고급 옵션과 색인화를 사용하여 검색 프로세스를 간소화하십시오."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Microsoft Word Open XML 문서"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Adobe 휴대용 문서 형식"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "PowerPoint Open XML 프레젠테이션"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Microsoft Excel Open XML 스프레드시트"
  

---