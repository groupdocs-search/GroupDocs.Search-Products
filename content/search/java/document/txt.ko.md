
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: ko
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "GroupDocs.Search를 사용하여 TXT 문서에서 텍스트 찾기 - Java"
head_description: "GroupDocs.Search for Java는 Java 개발자가 다양한 문서 형식 내에서 신속하게 텍스트를 검색할 수 있도록 도와줍니다."

############################# Header ############################
title: "스마트 문서 텍스트 검색" 
description: "GroupDocs.Search for Java를 통해 Java 애플리케이션에서 여러 문서 형식의 텍스트를 원활하게 검색하고 추출할 수 있습니다."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 체험판 받기"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search는 무엇을 하나요?"
    link: "/search/java/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/)는 PDF, Word, PowerPoint, Excel, 이미지, ZIP 아카이브를 포함한 70개 이상의 파일 형식을 지원하는 강력한 문서 검색 및 인덱싱 라이브러리입니다. 대량의 문서 컬렉션에 대해 빠르고 정확하며 확장 가능한 검색 기능을 제공합니다.

############################# Steps ############################
steps:
    enable: true
    title: "TXT 파일에서 텍스트 검색 수행"
    content: |
      [GroupDocs.Search](/search/java/)는 정교한 논리와 인덱싱을 통해 TXT 파일을 검색할 수 있도록 하여 Java 애플리케이션에서 검색 정확도를 향상시킵니다.
      
      1. 검색 인덱스를 저장할 디렉토리 설정.
      2. TXT 파일이 포함된 폴더 선택.
      3. 추가 검색 옵션 정의.
      4. 검색을 실행하고 결과 분석.
   
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
        // 검색 인덱스를 저장할 디렉토리 설정
        Index index = new Index("c:/MyIndex");

        // 검색 가능한 문서가 포함된 폴더 지정
        index.add("c:/MyDocuments");

        // 유사한 발음의 단어를 일치시키는 동음이의어 검색 활성화
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // 고급 검색 쿼리 실행
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "향상된 검색 및 인덱싱 기능"
  description: "GroupDocs.Search for Java는 70개 이상의 문서 형식에서 텍스트 검색 및 인덱싱을 간소화하여 정보를 신속하게 관리하고 검색할 수 있는 효율적인 도구를 제공합니다."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search의 핵심 기능"
  features:
    # feature loop
    - title: "포괄적인 텍스트 검색"
      content: "PDF, Word 문서, PowerPoint 프레젠테이션 및 스프레드시트와 같은 여러 문서 형식에서 텍스트를 찾습니다. 정확한 일치, 퍼지 검색 및 와일드카드 연산자를 사용하여 세부적인 검색 결과를 얻으세요."

    # feature loop
    - title: "대규모 데이터에 대한 최적화된 인덱싱"
      content: "구조화된 인덱스를 생성하여 검색 속도를 높이고, 방대한 문서 저장소를 효율적으로 탐색할 수 있습니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어에서 검색을 수행하며, 다양한 키보드 레이아웃과 단어 형태 변화에 대한 지원으로 정확도를 높입니다."

    # feature loop
    - title: "유연한 검색 설정"
      content: "대소문자 구분, 날짜 기반 필터링, 특정 단어 제외와 같은 옵션으로 검색을 사용자화하여 정확한 결과를 제공합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 검색 쿼리 구현"
      content: |
        이 예제는 TXT 문서 내에서 효율적으로 검색 쿼리를 사용하는 방법을 보여줍니다.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // 검색 인덱스를 위한 디렉토리 정의
          Index index = new Index("c:/MyIndex");
              
          // 문서에 대한 파일 경로 제공
          index.add("c:/MyDocuments");

          // 암호화된 문서에 대한 암호 입력
          index.getDictionaries().getDocumentPasswords().add("protected.txt", "123456");

          // 유사한 단어를 감지하기 위한 퍼지 검색 활성화
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // 검색 결과 가져오기
          SearchResult result = index.Search("Loarem", options);
          
          // 검색 결과 처리 및 분석
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
            link: "/examples/search/formats/searchdocument.txt"
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
    exclude: "document"
    description: "효율성과 정확성을 위해 설계된 고성능 텍스트 검색 기능을 발견하세요."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "GroupDocs.Search를 사용하여 TXT 문서에서 정보 찾기"
    exclude: "TXT"
    description: "GroupDocs.Search는 70개 이상의 형식을 지원하며, 사무 파일을 포함하여 빠른 검색과 고급 인덱싱 기능을 제공합니다."
    items: 
        # format loop 1
        - name: "DOCX 문서에서 검색"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 문서에서 검색"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 문서에서 검색"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 문서에서 검색"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 문서에서 검색"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---