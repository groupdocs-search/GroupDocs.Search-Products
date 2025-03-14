
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: ko
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "PPTX에서 Java의 대소문자를 구분하는 검색 수행"
head_description: "GroupDocs.Search for Java API는 Java 개발자가 여러 문서 유형에서 대소문자를 구분하는 검색을 실행할 수 있도록 돕습니다."

############################# Header ############################
title: "대소문자를 구분하는 문서 검색" 
description: "GroupDocs.Search for Java을(를) 사용하면 Java 프로젝트에서 정밀한 대소문자 구분 검색 기능을 구현할 수 있습니다."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료로 받기"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search에 대하여 알아보기"
    link: "/search/java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)은(는) 다양한 문서 간 텍스트 검색 및 인덱싱을 위한 다재다능한 도구입니다. PDF, Word 파일, PowerPoint 프레젠테이션, Excel 시트, 이미지, ZIP 파일 등 70개 이상의 형식을 지원하여 방대한 데이터를 효율적으로 처리할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "PPTX 파일에서 대소문자 구분 검색하기"
    content: |
      [GroupDocs.Search](/search/java/)을(를) 사용하여 PPTX 문서에서 대소문자 구분 검색을 수행하여 Java 프로젝트를 향상시킬 수 있습니다.
      
      1. 검색 인덱스를 저장할 폴더를 설정합니다.
      2. PPTX 파일이 포함된 폴더를 선택합니다.
      3. 대소문자 구분 검색을 실행하고 결과를 수집합니다.
      4. 검색 결과를 처리하고 사용합니다.
   
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
        // 인덱스 저장 위치를 정의합니다.
        Index index = new Index("c:/MyIndex");

        // 검색할 문서가 포함된 폴더를 지정합니다.
        index.add("c:/MyDocuments");

        // 검색 설정에서 대소문자 구분 모드를 활성화합니다.
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // 검색을 실행합니다.
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "강화된 검색 및 인덱싱 도구"
  description: "GroupDocs.Search for Java으로 70개 이상의 형식에 대한 문서 검색 및 인덱싱을 간소화하여 정보를 찾아주고 정리하기가 더 용이합니다."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "유연한 텍스트 검색"
      content: "PDF, Word 파일, 스프레드시트, 프레젠테이션 등 문서 내에서 검색합니다. 정확한 일치를 포함하여 퍼지 검색 및 와일드카드 지원과 같은 도구를 사용하여 결과를 세분화하십시오."

    # feature loop
    - title: "효율적인 인덱스 관리"
      content: "대량의 데이터 세트를 정리하고 인덱싱하여 큰 문서 컬렉션을 처리할 때 검색 속도와 성능을 향상시킵니다."

    # feature loop
    - title: "글로벌 언어 지원"
      content: "80개 이상의 언어로 검색을 수행하여 다양한 키보드 레이아웃과 언어적 변형에 대한 더 나은 정확성을 제공합니다."

    # feature loop
    - title: "맞춤형 검색 필터"
      content: "대소문자 구분, 날짜 범위 필터링 및 인덱싱 중 원하지 않는 단어 또는 데이터를 제외하는 옵션과 같은 검색 기준을 조정합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "예제: 대소문자 구분 검색 쿼리"
      content: |
        이 예제는 PPTX 문서를 위한 대소문자 구분 검색을 구현하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 검색 인덱스를 위한 디렉토리를 정의합니다.
          Index index = new Index("c:/MyIndex");
              
          // 문서 폴더의 위치를 지정합니다.
          index.add("c:/MyDocuments");

          // 검색 쿼리를 설정합니다.
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // 검색 옵션에서 대소문자 구분을 활성화합니다.
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // 문서 검색을 수행합니다.
          SearchResult result = index.search(wordQuery, options);
          
          // 검색된 결과를 처리합니다.
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
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    title: "주요 기능 개요"
    exclude: "case-sensitive"
    description: "GroupDocs.Search for Java에서 제공하는 강력하고 효과적인 검색 기능을 알아보세요."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "검색을 위한 지원 파일 형식"
    exclude: "PPTX"
    description: "GroupDocs.Search은(는) 70개 이상의 인기 문서 형식과 함께 작동하며, 맞춤형 검색 설정 및 효율적인 인덱싱을 제공합니다."
    items: 
        # format loop 1
        - name: "DOCX 대소문자 구분 검색"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 대소문자 구분 검색"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 대소문자 구분 검색"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 대소문자 구분 검색"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 대소문자 구분 검색"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---