
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: ko
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "TXT 문서에서 검색하기 - Node.js"
head_description: "GroupDocs.Search for Node.js via Java은 JavaScript 응용 프로그램에 빠르고 정확한 텍스트 검색 기능을 추가하여 다양한 문서 형식을 지원합니다."

############################# Header ############################
title: "업무 문서에서 텍스트 찾기" 
description: "GroupDocs.Search for Node.js via Java은 문서에 강력하고 유연한 검색 기능을 제공합니다. Node.js 응용 프로그램에 텍스트 검색을 통합하세요."
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
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)은 문서에서 빠른 텍스트 검색을 가능하게 하는 강력한 검색 및 인덱싱 라이브러리입니다. PDFs, Word, Excel, PowerPoint를 포함한 70개 이상의 파일 형식을 지원하여 정확하고 효율적인 검색을 보장합니다.

############################# Steps ############################
steps:
    enable: true
    title: "TXT 문서에서 검색 수행하는 방법"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)은 Node.js via Java 응용 프로그램에 대해 TXT 문서에서 텍스트 검색을 간단하고 효율적으로 수행합니다.
      
      1. 검색 인덱스를 저장할 디렉토리를 생성합니다.
      2. 문서가 포함된 폴더를 선택합니다.
      3. TXT 파일만 포함되도록 검색 옵션을 설정합니다.
      4. 검색을 실행하고 결과를 검색합니다.
   
    code:
      platform: "nodejs-java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "검색 결과"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "클릭하여 복사"
        copy_done: "복사 완료"
      links:
        #  loop
        - title: "자세한 예시"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // 검색 인덱스를 저장할 디렉토리 정의
        const index = new searchLib.Index("c:/MyIndex");

        // 검색 가능한 문서가 포함된 폴더 지정
        index.add("c:/MyDocuments");

        // 특정 파일 형식으로 검색 제한
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".txt");

        // 검색 결과 검색 및 처리
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 검색 기능"
  description: "GroupDocs.Search for Node.js via Java은 70개 이상의 파일 형식을 인덱싱하여 문서 검색 효율성을 향상시킵니다. 고급 검색 기술로 콘텐츠 검색을 최적화하세요."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "종합적인 텍스트 검색"
      content: "PDF, Word 파일, 스프레드시트, 프레젠테이션 등 인기 있는 문서 형식에서 텍스트를 추출하고 찾습니다. 퍼지 검색, 동음이의어 및 와일드카드 쿼리를 지원합니다."

    # feature loop
    - title: "성능을 위한 최적화된 인덱싱"
      content: "재사용 가능한 인덱스를 생성하여 검색 속도를 가속화합니다. 대규모 문서 컬렉션 작업 시 속도와 효율성을 향상시킵니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 문서를 검색합니다. 더 나은 정확성을 위해 키보드 레이아웃과 단어 변형을 인식합니다."

    # feature loop
    - title: "사용자 정의 가능한 검색 옵션"
      content: "필터, 정규 표현식, 대소문자 구분 및 기타 유연한 설정으로 검색 결과를 미세 조정합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "검색 가능한 문서 필터링"
      content: |
        필터를 사용하여 문서 검색을 세부적으로 조정하는 방법을 배웁니다.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 원하지 않는 파일 형식을 제외하도록 인덱스를 구성합니다.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // 문서가 포함된 디렉토리를 지정합니다.
          index.add("c:/MyDocuments");

          // 추가 사용을 위해 검색 출력을 처리합니다.
          const result = index.Search("Lorem", options);
          
          // 추가 사용을 위해 검색 출력을 처리합니다.
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "복사"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "클릭하여 복사"
          copy_done: "복사 완료"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/search/formats/searchfilters.txt"
        links:
          #  loop
          - title: "자세한 예시"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "문서화"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨습니까?"
  description: "GroupDocs.Search의 기능을 무료로 체험하거나 라이센스를 요청해 보십시오."
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
    exclude: "filters"
    description: "문서에서 빠르고 정확한 텍스트 검색을 수행합니다."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "다양한 문서 형식에서 검색하기"
    exclude: "TXT"
    description: "GroupDocs.Search은 70개 이상의 파일 형식을 지원하여 다양한 오피스 및 비즈니스 문서에서 효율적인 텍스트 검색을 가능하게 합니다."
    items: 
        # format loop 1
        - name: "DOCX 검색 필터"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 검색 필터"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 검색 필터"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 검색 필터"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 검색 필터"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---