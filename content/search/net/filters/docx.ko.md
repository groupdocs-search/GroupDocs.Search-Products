
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: ko
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "DOCX 문서에서 검색하기 - .NET"
head_description: "GroupDocs.Search for .NET는 다양한 비즈니스 문서 형식에서 효율적인 텍스트 검색을 통해 C# 애플리케이션을 향상시킵니다."

############################# Header ############################
title: "비즈니스 문서에서 텍스트 검색하기" 
description: "GroupDocs.Search for .NET는 문서 내에서 강력하고 유연한 텍스트 검색을 가능하게 합니다. .NET 애플리케이션에 검색 기능을 통합하세요."
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
       [GroupDocs.Search for .NET](/search/net/)는 효율적인 텍스트 검색 및 문서 인덱싱을 위한 강력한 라이브러리입니다. PDF, Word, Excel, PowerPoint와 같은 업계 표준 문서 등 70개 이상의 파일 형식을 지원합니다. 빠르고 정확한 결과로 검색 성능을 향상시킵니다.

############################# Steps ############################
steps:
    enable: true
    title: "DOCX 데이터에서 검색하는 방법"
    content: |
      [GroupDocs.Search](/search/net/)는 DOCX 문서에서 효율적인 텍스트 검색을 가능하게 하여 .NET 애플리케이션에 적합합니다.
      
      1. 검색 인덱스를 저장할 폴더를 설정합니다.
      2. 파일이 포함된 폴더를 선택합니다.
      3. DOCX 문서만 처리하도록 검색 옵션을 구성합니다.
      4. 검색을 실행하고 결과를 가져옵니다.
   
    code:
      platform: "net"
      copy_title: "복사"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "복사하려면 클릭"
        copy_done: "복사됨"
      links:
        #  loop
        - title: "더 많은 예제"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "문서화"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // 재사용 가능한 검색 인덱스를 저장할 경로
        Index index = new Index("c:/MyIndex");

        // 문서가 포함된 폴더
        index.Add("c:/MyDocuments");

        // 특정 파일 형식 내에서만 검색
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".docx");

        // 검색 결과 가져오기
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 검색 기능"
  description: "GroupDocs.Search for .NET는 70개 이상의 파일 형식에서 정교한 텍스트 검색을 가능하게 합니다. 인덱싱은 검색 효율성을 높이고 문서 내용을 효과적으로 관리하도록 돕습니다."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "고급 텍스트 검색"
      content: "PDF, Word 파일, 프레젠테이션 및 스프레드시트와 같은 인기 있는 비즈니스 문서에서 관련 텍스트를 추출합니다. 퍼지 검색, 동음이의어 탐지 및 와일드카드와 같은 여러 검색 기술을 지원합니다."

    # feature loop
    - title: "더 빠른 검색을 위한 최적화된 인덱싱"
      content: "검색 속도를 향상시키기 위해 검색 인덱스를 작성하고 재사용할 수 있습니다. 대규모 문서 집합을 검색할 때 성능을 최적화합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 작성된 문서에서 검색을 수행합니다. 정확성을 개선하기 위해 다양한 키보드 레이아웃 및 단어 변형을 감지합니다."

    # feature loop
    - title: "유연한 검색 설정"
      content: "필터, 정규 표현식 및 대소문자 구분 설정과 같은 사용자 정의 옵션으로 검색 결과를 정제합니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "처리할 문서 필터링"
      content: |
        필터를 사용하여 문서 검색 범위를 좁히는 방법을 배웁니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 특정 파일 형식을 제외하는 인덱스를 설정합니다.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // 문서 디렉토리를 지정합니다.
          index.Add("c:/MyDocuments");

          // 검색 결과를 가져옵니다.
          SearchResult result = index.Search("Lorem");
          
          // 검색 출력을 처리하고 사용합니다.
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "복사"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "복사하려면 클릭"
          copy_done: "복사됨"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
        links:
          #  loop
          - title: "더 많은 예제"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "문서화"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "시작할 준비가 되셨습니까?"
  description: "GroupDocs.Search 기능을 무료로 시험해 보거나 라이센스를 요청하세요."
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
    title: "주요 기능"
    exclude: "filters"
    description: "정확하고 효율적인 데이터 검색을 수행합니다."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "비즈니스 문서에서 데이터 찾기"
    exclude: "DOCX"
    description: "GroupDocs.Search는 70개 이상의 파일 형식을 지원하며, 인기 있는 오피스 문서의 효율적인 처리 및 검색을 가능하게 합니다."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Microsoft Word Open XML 문서"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Adobe 휴대용 문서 형식"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "PowerPoint Open XML 프레젠테이션"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Microsoft Excel Open XML 스프레드시트"
  

---