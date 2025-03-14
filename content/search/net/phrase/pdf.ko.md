
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: ko
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "PDF에서 구문 검색하기 - GroupDocs.Search for .NET"
head_description: "GroupDocs.Search for .NET는 문서 콘텐츠에 대한 강력한 구문 검색 기능으로 C# 응용 프로그램을 강화합니다."

############################# Header ############################
title: "문서에서 구문 검색하기" 
description: "GroupDocs.Search for .NET를 사용하여 특정 구문을 신속하게 찾으십시오. 효율적인 검색 기능을 .NET 응용 프로그램에 통합하십시오."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "다운로드"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search의 기능"
    link: "/search/net/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/)는 문서에서 텍스트를 인덱싱하고 검색하는 강력한 라이브러리입니다. PDF, Word 문서, Excel 시트, 이미지 및 ZIP 파일을 포함한 70개 이상의 파일 형식을 지원하여 빠르고 정확한 검색 결과를 제공합니다.

############################# Steps ############################
steps:
    enable: true
    title: "PDF 문서에서 구문 검색하는 방법"
    content: |
      [GroupDocs.Search](/search/net/)는 PDF 문서에서의 검색을 단순화합니다. 다양한 옵션을 사용하여 .NET 응용 프로그램에서 검색 결과를 세분화하십시오.
      
      1. 검색 인덱스 폴더를 설정하십시오.
      2. PDF 파일이 포함된 폴더를 지정하십시오.
      3. 검색 설정을 구성하십시오.
      4. 검색 결과를 검색하고 처리하십시오.
   
    code:
      platform: "net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "검색 결과"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "클릭하여 복사"
        copy_done: "복사 완료"
      links:
        #  loop
        - title: "자세한 예시"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // 검색 인덱스를 저장할 경로
        Index index = new Index("c:/MyIndex");

        // 문서가 포함된 폴더
        index.Add("c:/MyDocuments");

        // 검색 옵션 구성
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // 검색 실행
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: ".NET 문서 검색 엔진 발견하기"
  description: "GroupDocs.Search for .NET는 70개 이상의 파일 형식에서 구문 검색을 가능하게 합니다. 고급 검색 기능으로 데이터를 효율적으로 찾고 관리하십시오."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "구문 검색"
      content: "PDF, Word 파일, 프레젠테이션 및 스프레드시트를 포함한 비즈니스 문서에서 정확한 구문을 검색하십시오. 정확한 구문을 모르는 경우 와일드카드 및 기타 옵션을 사용하십시오."

    # feature loop
    - title: "효율적인 데이터 인덱싱"
      content: "문서 검색 속도를 향상시키기 위해 검색 인덱스를 생성하고 재사용하십시오. 인덱싱은 데이터를 효율적으로 구조화하여 구문 검색 속도를 빠르게 합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 문서를 검색하십시오. 더 나은 검색 정확성을 위해 다양한 키보드 레이아웃 및 형태소 단어 형태를 지원합니다."

    # feature loop
    - title: "유연한 검색 옵션"
      content: "대소문자 구분, 퍼지 검색 및 동음이의어 검색, 문서 필터링 등과 같은 기능으로 검색을 사용자 정의하십시오."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 검색 기술 사용하기"
      content: |
        PDF에서 검색하기 위한 쿼리를 만드는 방법을 배우십시오.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 검색 인덱스를 위한 폴더를 지정하십시오.
          Index index = new Index("c:/MyIndex");
              
          // 검색용 문서 경로 설정
          index.Add("c:/MyDocuments");

          // 특정 구문을 위한 쿼리 생성
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // 검색 결과를 검색
          SearchResult result = index.Search(query);
          
          // 결과를 처리하고 활용하십시오.
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "복사"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "클릭하여 복사"
          copy_done: "복사 완료"
        top_links:
          #  loop
          - title: "결과 다운로드"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pdf"
        links:
          #  loop
          - title: "자세한 예시"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "문서화"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨습니까?"
  description: "GroupDocs.Search의 기능을 무료로 체험하거나 라이센스를 요청해 보십시오."
  items:
    #  loop
    - title: "Nuget 다운로드"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "라이센스"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "고급 기능"
    exclude: "phrase"
    description: "강력하고 효율적인 검색 기능을 활용하십시오."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "비즈니스 문서에서 구문 검색하기"
    exclude: "PDF"
    description: "GroupDocs.Search는 70개 이상의 문서 형식에서 검색을 지원합니다. 고급 옵션과 인덱싱을 사용하여 검색 프로세스를 간소화하십시오."
    items: 
        # format loop 1
        - name: "DOCX 구문 검색"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 구문 검색"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 구문 검색"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 구문 검색"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 구문 검색"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---