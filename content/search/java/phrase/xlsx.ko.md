
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:52
draft: false
lang: ko
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "XLSX에서 구문 검색 수행하기 - GroupDocs.Search for Java"
head_description: "GroupDocs.Search for Java는 문서 콘텐츠에 대한 고급 구문 검색 기능으로 Java 애플리케이션을 향상시킵니다."

############################# Header ############################
title: "문서에서 구문 찾기" 
description: "GroupDocs.Search for Java를 사용하여 특정 구문을 신속하게 찾아보세요. Java 애플리케이션에 강력한 검색 기능을 추가하세요."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "다운로드"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search 기능"
    link: "/search/java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)는 문서 내 텍스트 색인화 및 검색을 위한 강력한 라이브러리입니다. PDF, Word 문서, Excel 스프레드시트, 이미지 및 ZIP 파일을 포함하여 70개 이상의 파일 형식을 지원하여 빠르고 정확한 검색 결과를 보장합니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX 문서에서 구문 찾는 방법"
    content: |
      [GroupDocs.Search](/search/java/)는 XLSX 문서에서 구문 검색을 간소화합니다. Java 애플리케이션에서 검색 결과를 개선하기 위해 다양한 옵션을 사용하세요.
      
      1. 검색 인덱스 디렉토리 생성.
      2. XLSX 파일이 있는 폴더 지정.
      3. 검색 매개변수 조정.
      4. 검색 결과를 검색하고 분석.
   
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
        // 검색 인덱스 경로 정의
        Index index = new Index("c:/MyIndex");

        // 문서가 있는 폴더 지정
        index.add("c:/MyDocuments");

        // 검색 기본 설정 설정
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // 검색 쿼리 실행
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Java 문서 검색 엔진 탐색"
  description: "GroupDocs.Search for Java는 70개 이상의 파일 형식에서 구문 검색을 지원합니다. 고급 검색 기능을 사용하여 데이터를 쉽게 찾고 정리할 수 있습니다."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "구문 검색"
      content: "PDF, Word 파일, 프레젠테이션 및 스프레드시트와 같은 비즈니스 문서에서 정확한 구문을 찾습니다. 정확한 구문이 알려지지 않은 경우 와일드카드 및 기타 옵션을 사용하세요."

    # feature loop
    - title: "최적화된 데이터 색인화"
      content: "검색 인덱스를 생성하고 재사용하여 문서 검색 속도를 높입니다. 색인화는 데이터를 효율적으로 정리하여 더 빠르고 정확한 검색을 가능하게 합니다."

    # feature loop
    - title: "다국어 호환성"
      content: "80개 이상의 언어로 문서를 검색하세요. 다양한 키보드 레이아웃과 형태소 분석을 지원하여 검색 정밀도를 향상시킵니다."

    # feature loop
    - title: "고급 검색 옵션"
      content: "대소문자 구분, 퍼지 검색, 동음이의어 일치, 문서 필터링 및 기타 강력한 기능으로 검색을 사용자 맞춤화하세요."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 검색 방법 활용하기"
      content: |
        XLSX에서 검색 쿼리 구성 방법을 배워보세요.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 검색 인덱스의 디렉토리 정의
          Index index = new Index("c:/MyIndex");
              
          // 대상 문서의 경로 설정
          index.add("c:/MyDocuments");

          // 특정 구문을 위한 검색 쿼리 생성
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // 검색 결과 가져오기
          SearchResult result = index.search(query);
          
          // 가져온 결과 처리 및 활용
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "고급 검색 기능"
    exclude: "phrase"
    description: "개선된 정확도와 성능을 위한 최첨단 검색 기능을 활용하세요."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "비즈니스 문서에서 구문 검색"
    exclude: "XLSX"
    description: "GroupDocs.Search는 70개 이상의 문서 형식에서 구문 검색을 가능하게 합니다. 효율적인 검색을 위해 고급 옵션 및 색인화 기능을 활용하세요."
    items: 
        # format loop 1
        - name: "DOCX 구문 검색"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 구문 검색"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 구문 검색"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 구문 검색"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 구문 검색"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---