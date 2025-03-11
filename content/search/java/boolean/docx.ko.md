
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: ko
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "DOCX에서 Java를 이용한 불리언 검색"
head_description: "GroupDocs.Search for Java를 사용하면 개발자는 AND, OR, NOT과 같은 불리언 연산자를 이용하여 문서 검색을 수행할 수 있습니다."

############################# Header ############################
title: "불리언 텍스트 검색" 
description: "GroupDocs.Search for Java를 사용하여 Java 프로젝트에서 복잡한 불리언(AND, OR, NOT) 검색 쿼리를 작성하세요."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 소개"
    link: "/search/java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)은 문서에서 텍스트 검색과 데이터 색인을 위해 설계된 다목적 라이브러리입니다. PDF, Word, Excel, PowerPoint 이미지 및 ZIP 아카이브를 포함한 70개 이상의 파일 형식을 지원하여 대량의 데이터 컬렉션에서 효율적인 검색을 수행할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "DOCX 문서에서 불리언 검색을 수행하는 방법"
    content: |
      [GroupDocs.Search](/search/java/)은 DOCX 문서 내에서 텍스트 검색을 수행할 수 있도록 지원합니다. 불리언 조건을 지원하여 Java 애플리케이션에서 검색 정확성을 높일 수 있습니다.
      
      1. 검색 색인을 저장할 폴더를 지정합니다.
      2. DOCX 문서가 포함된 폴더를 선택합니다.
      3. 검색 쿼리를 실행하고 결과를 검색합니다.
      4. 획득한 결과를 처리합니다.
   
    code:
      platform: "java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "복사하려면 클릭"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // 색인 폴더의 경로 설정
        Index index = new Index("c:/MyIndex");

        // 검색을 위해 문서가 포함된 폴더 경로 제공
        index.add("c:/MyDocuments");

        // 복잡한 쿼리로 검색 실행
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 검색 및 색인을 위한 강력한 도구"
  description: "GroupDocs.Search for Java은 70개 이상의 형식에 대한 텍스트 검색 및 데이터 색인을 간소화합니다. 고급 도구를 통해 내용을 쉽게 찾고 관리할 수 있습니다."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "포괄적인 텍스트 검색"
      content: "PDF, Word 문서, 프레젠테이션, 스프레드시트 등 다양한 형식에서 검색합니다. 결과를 정제하기 위해 정확한 일치, 퍼지 검색 및 와일드카드 쿼리와 같은 옵션을 사용할 수 있습니다."

    # feature loop
    - title: "효율적인 데이터 색인화"
      content: "더 빠른 문서 검색을 위해 색인을 구축하고 유지합니다. 이 기능은 데이터를 효율적으로 조직하여 대량의 문서 컬렉션 처리를 용이하게 합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 작성된 문서에서 검색합니다. 형태학적 단어 형식과 다양한 키보드 레이아웃을 활용하여 정확성을 향상시킵니다."

    # feature loop
    - title: "유연한 검색 맞춤 설정"
      content: "결과를 정제하기 위해 대소문자 구분, 날짜 범위 필터 및 제외 사항과 같은 기능으로 검색 설정을 조정합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "복잡한 불리언 검색 쿼리 사용"
      content: |
        이 예제에서는 DOCX 파일에서 불리언 검색을 수행하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 검색 색인을 위한 폴더 설정
          Index index = new Index("c:/MyIndex");
              
          // 검색할 문서의 경로 제공
          index.add("c:/MyDocuments");

          // 불리언 논리를 사용하여 쿼리 구성
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // 검색 결과 검색
          SearchResult result = index.search(booleanQuery);
          
          // 검색된 결과 처리
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "복사"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "복사하려면 클릭"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "문서화"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨습니까?"
  description: "GroupDocs.Search 기능을 무료로 시험해 보거나 라이센스를 요청하세요."
  items:
    #  loop
    - title: "Maven 다운로드"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "라이센스"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "한눈에 보는 주요 기능"
    exclude: "boolean"
    description: "강력하고 효율적인 검색 기능을 활용하세요."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "인기 문서 형식 검색"
    exclude: "DOCX"
    description: "GroupDocs.Search는 70개 이상의 파일 형식을 지원하여 검색 규칙을 맞춤 설정하고 성능을 최적화하는 데 색인을 사용할 수 있습니다."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word Open XML 문서"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobe 휴대용 문서 형식"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPoint Open XML 프레젠테이션"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft Excel Open XML 스프레드시트"
  

---