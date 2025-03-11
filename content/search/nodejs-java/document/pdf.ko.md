
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: ko
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Node.js에서 PDF의 텍스트 검색하기 - GroupDocs.Search"
head_description: "JavaScript와 함께 GroupDocs.Search for Node.js via Java를 사용하여 다양한 문서 형식에서 텍스트를 효율적으로 검색하세요."

############################# Header ############################
title: "스마트 문서 검색 솔루션" 
description: "GroupDocs.Search for Node.js via Java를 사용하여 다양한 문서 형식에서 텍스트를 찾으세요. Node.js 애플리케이션 내에서 고급 검색 쿼리를 작성할 수 있습니다."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험하기"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 소개"
    link: "/search/nodejs-java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)은 고성능 풀 텍스트 검색 및 문서 인덱싱을 위한 라이브러리입니다. PDF, Word, PowerPoint, Excel, 이미지 및 ZIP 아카이브를 포함한 70개 이상의 파일 형식을 지원하여 빠르고 정확한 결과를 보장합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PDF 파일에서 검색 수행"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)를 통해 PDF 파일에서 검색을 수행하여 Node.js via Java 애플리케이션 내에서 결과를 정제할 수 있습니다.
      
      1. 검색 인덱스를 위한 저장 폴더 정의.
      2. PDF 파일이 있는 폴더 선택.
      3. 추가 검색 매개변수 설정.
      4. 검색을 실행하고 결과 분석.
   
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

        // 검색 인덱스 저장을 위한 디렉토리 지정
        const index = new searchLib.Index("c:/MyIndex");

        // 검색할 문서가 포함된 폴더 선택
        index.add("c:/MyDocuments");

        // 유사하게 들리는 단어에 대한 동음 이의어 검색 활성화
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // 복잡한 검색 쿼리 실행
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 검색 및 인덱싱 기능"
  description: "GroupDocs.Search for Node.js via Java은 70개 이상의 문서 형식에서 강력한 텍스트 검색 및 인덱싱 도구를 제공하여 정보를 쉽게 찾고 정리할 수 있게 합니다."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 이점"
  features:
    # feature loop
    - title: "종합 텍스트 검색"
      content: "PDF, Word 문서, PowerPoint 프레젠테이션 및 스프레드시트를 포함한 다양한 문서 유형에서 텍스트를 찾습니다. 정밀한 결과를 위해 정확한 일치, 퍼지 검색 및 와일드카드를 사용하세요."

    # feature loop
    - title: "대량 데이터에 대한 효율적인 인덱싱"
      content: "구조화된 인덱스를 생성하여 검색을 가속화하며 대량의 문서 컬렉션에서 정보를 더 쉽게 검색할 수 있게 합니다."

    # feature loop
    - title: "80개 이상의 언어 지원"
      content: "다양한 언어의 문서에서 검색하며, 다양한 단어 형태와 키보드 레이아웃을 자동으로 인식합니다."

    # feature loop
    - title: "사용자 정의 검색 설정"
      content: "정확한 결과를 얻기 위해 대소문자 구분, 날짜 필터 및 단어 제외와 같은 검색 옵션을 조정하세요."
      
  code_samples_ext:
    # code sample ext loop
    - title: "PDF 문서에서 검색 사용하기"
      content: |
        이 예시는 PDF 문서 내에서 검색 쿼리를 사용하는 방법을 보여줍니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 검색 인덱스를 위한 디렉토리 설정
          const index = new searchLib.Index("c:/MyIndex");
              
          // 문서 저장을 위한 파일 경로 제공
          index.add("c:/MyDocuments");

          // 보호된 파일의 비밀번호 입력
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", '123456');

          // 유사 단어 탐지를 위한 퍼지 검색 활성화
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // 검색 결과 추출
          const result = index.search("Loarem", options);
          
          // 결과 처리 및 검토
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "주요 기능 탐색"
    exclude: "document"
    description: "효율성과 정확성을 향상시키기 위해 설계된 고속 검색 기능을 발견하세요."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 문서에서 검색하기"
    exclude: "PDF"
    description: "GroupDocs.Search은 사무 문서를 포함한 70개 이상의 파일 형식과 함께 작동하여 인덱싱 지원으로 빠르고 정확한 검색을 보장합니다."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Microsoft Word Open XML 문서"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Adobe 휴대용 문서 형식"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "PowerPoint Open XML 프레젠테이션"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Microsoft Excel Open XML 스프레드시트"
  

---