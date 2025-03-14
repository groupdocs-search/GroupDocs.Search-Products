
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: ko
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "PDF 문서에서 검색하기 - GroupDocs.Search for Java"
head_description: "GroupDocs.Search for Java는 다양한 비즈니스 문서 형식을 지원하는 Java 애플리케이션에 강력한 텍스트 검색 기능을 추가합니다."

############################# Header ############################
title: "비즈니스 문서에서 텍스트 찾기" 
description: "GroupDocs.Search for Java를 사용하면 유연하고 정밀한 쿼리로 문서에서 텍스트를 검색할 수 있습니다. Java 애플리케이션에 검색 기능을 손쉽게 통합할 수 있습니다."
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
    title: "GroupDocs.Search란 무엇인가요?"
    link: "/search/java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)는 빠른 텍스트 검색 및 문서 색인을 위한 강력한 라이브러리입니다. PDF, Word, Excel 및 PowerPoint와 같은 산업 표준을 포함해 70개 이상의 파일 형식을 지원합니다. 높은 속도와 정확성을 갖춘 검색 기능으로 애플리케이션의 기능을 향상시킬 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "PDF 문서에서 검색하는 방법"
    content: |
      [GroupDocs.Search](/search/java/)는 PDF 문서에서 빠르고 효율적인 텍스트 검색을 가능하게 하며, Java 애플리케이션에 적합합니다.
      
      1. 검색 인덱스를 저장할 폴더를 지정합니다.
      2. 문서가 포함된 폴더를 선택합니다.
      3. PDF 문서로 결과를 제한하기 위해 검색 옵션을 구성합니다.
      4. 검색을 실행하고 결과를 가져옵니다.
   
    code:
      platform: "java"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "검색 결과"
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
        copy_tip: "클릭하여 복사"
        copy_done: "복사 완료"
      links:
        #  loop
        - title: "자세한 예시"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // 재사용 가능한 검색 인덱스를 저장할 디렉토리
        Index index = new Index("c:/MyIndex");

        // 문서를 포함하는 폴더
        index.add("c:/MyDocuments");

        // 문서 형식별로 검색 결과 필터링
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // 검색 결과 가져오기
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "향상된 검색 기능"
  description: "GroupDocs.Search for Java는 70개 이상의 파일 형식에서 고급 텍스트 검색을 제공합니다. 색인은 검색 속도를 높이고 문서 관리 효율성을 개선합니다."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "강력한 텍스트 검색"
      content: "PDF, Word 파일, 프레젠테이션 및 스프레드시트와 같은 인기 문서 형식에서 텍스트를 찾을 수 있습니다. 퍼지 검색, 동음이의어 및 와일드카드를 포함한 여러 검색 방법을 지원합니다."

    # feature loop
    - title: "향상된 성능을 위한 최적화된 색인 생성"
      content: "검색 속도와 효율성을 높이기 위해 검색 색인을 생성 및 재사용할 수 있으며, 특히 대량의 문서 컬렉션에서 효과적입니다."

    # feature loop
    - title: "다국어 검색 지원"
      content: "80개 이상의 언어로 작성된 문서 내에서 검색이 가능합니다. 다양한 키보드 레이아웃과 단어 변형을 감지하여 정확성을 향상시킵니다."

    # feature loop
    - title: "사용자 정의 가능한 검색 옵션"
      content: "필터, 정규 표현식 및 기타 고급 검색 설정으로 검색 결과를 세분화할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "검색하기 전에 문서 필터링하기"
      content: |
        필터를 사용하여 검색을 세분화하는 방법을 배웁니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 특정 파일 형식을 제외한 색인 설정
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // 문서 저장 경로 지정
          index.add("c:/MyDocuments");

          // 검색 결과 가져오기
          SearchResult result = index.search("Lorem", options);
          
          // 검색 결과 처리 및 활용
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
          copy_tip: "클릭하여 복사"
          copy_done: "복사 완료"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pdf"
        links:
          #  loop
          - title: "자세한 예시"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "문서화"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨습니까?"
  description: "GroupDocs.Search의 기능을 무료로 체험하거나 라이센스를 요청해 보십시오."
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
    title: "주요 기능"
    exclude: "filters"
    description: "정밀하고 효율적인 텍스트 검색을 수행합니다."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "비즈니스 문서에서 검색하기"
    exclude: "PDF"
    description: "GroupDocs.Search는 70개 이상의 파일 형식을 지원하여 널리 사용되는 오피스 문서에서 검색하기가 용이합니다."
    items: 
        # format loop 1
        - name: "DOCX 검색 필터"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 검색 필터"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 검색 필터"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 검색 필터"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 검색 필터"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---