
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: ko
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "DOCX에서 .NET를 사용하는 대소문자 구분 검색"
head_description: "GroupDocs.Search for .NET API는 C# 개발자가 다양한 문서에서 대소문자 구분 검색을 수행할 수 있게 합니다."

############################# Header ############################
title: "대소문자 구분 검색" 
description: "GroupDocs.Search for .NET를 사용하면 .NET 애플리케이션 내에서 고급 대소문자 구분 검색 쿼리를 쉽게 생성할 수 있습니다."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "무료 다운로드"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search란?"
    link: "/search/net/"
    link_title: "자세히 알아보기"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/)는 문서 내 텍스트 검색 및 인덱싱을 위한 강력한 라이브러리입니다. PDF, Word, PowerPoint, Excel, 이미지 및 ZIP 파일 등 70개 이상의 파일 형식을 지원하여 대량의 데이터를 효율적으로 처리합니다.

############################# Steps ############################
steps:
    enable: true
    title: "DOCX 문서에서 대소문자 구분 검색 수행 방법"
    content: |
      [GroupDocs.Search](/search/net/)는 DOCX 문서에서 대소문자 구분 검색을 단순화합니다. .NET 애플리케이션에서 결과를 세분화하는 데 사용하세요.
      
      1. 검색 인덱스를 저장할 폴더를 정의합니다.
      2. DOCX 파일이 있는 폴더를 선택합니다.
      3. 검색을 실행하고 결과를 검색합니다.
      4. 결과를 처리합니다.
   
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
        // 인덱스 폴더의 경로를 설정합니다.
        Index index = new Index("c:/MyIndex");

        // 검색할 문서가 포함된 폴더를 지정합니다.
        index.Add("c:/MyDocuments");

        // 옵션에서 대소문자 구분 검색을 활성화합니다.
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // 검색을 실행합니다.
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 검색 및 인덱싱을 위한 고급 기능"
  description: "GroupDocs.Search for .NET 라이브러리는 70개 이상의 파일 형식에서 텍스트 검색 및 인덱싱을 단순화합니다. 강력한 검색 도구를 사용하여 정보를 쉽게 찾고 관리할 수 있습니다."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "고급 텍스트 검색"
      content: "PDF, Word 문서, 스프레드시트, 프레젠테이션 등 다양한 파일 형식에서 텍스트를 검색합니다. 정확한 결과를 위해 정확한 일치, 퍼지 검색 및 와일드카드와 같은 옵션을 사용할 수 있습니다."

    # feature loop
    - title: "대규모 데이터 세트 인덱싱"
      content: "빠른 검색을 위해 인덱스를 구축하고 유지 관리합니다. 조직된 인덱싱은 방대한 문서 컬렉션 검색을 간소화합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 된 문서에서 검색하며, 서로 다른 키보드 레이아웃과 단어 형태를 지원하여 보다 정확한 결과를 제공합니다."

    # feature loop
    - title: "사용자 정의 검색 옵션"
      content: "대소문자 구분, 날짜 범위 필터 및 인덱싱 시 특정 단어 또는 데이터를 제외할 수 있는 기능으로 검색 설정을 사용자 정의합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "대소문자 구분 검색 쿼리 사용"
      content: |
        이 예제는 DOCX 문서 검색을 위한 대소문자 구분 쿼리 사용 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 검색 인덱스를 위한 폴더를 설정합니다.
          Index index = new Index("c:/MyIndex");
              
          // 검색할 문서의 경로를 지정합니다.
          index.Add("c:/MyDocuments");

          // 검색 쿼리를 생성합니다.
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // 대소문자 구분 검색 옵션을 활성화합니다.
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // 문서에서 텍스트를 검색합니다.
          SearchResult result = index.Search(wordQuery, options);
          
          // 검색 결과를 처리합니다.
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
            link: "/examples/search/formats/searchcase-sensitive.docx"
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
    title: "주요 기능 알아보기"
    exclude: "case-sensitive"
    description: "고급 및 효율적인 검색 기능을 탐색하세요."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "인기 문서 형식 검색"
    exclude: "DOCX"
    description: "GroupDocs.Search는 70개 이상의 파일 형스를 지원합니다. 검색 규칙을 사용자 정의하고 인덱싱을 사용하여 시간과 노력을 절약하세요."
    items: 
        # format loop 1
        - name: "DOCX 대소문자 구분 검색"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 대소문자 구분 검색"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 대소문자 구분 검색"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 대소문자 구분 검색"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 대소문자 구분 검색"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---