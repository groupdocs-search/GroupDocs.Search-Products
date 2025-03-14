
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: ko
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "XLSX 문서를 .NET에서 GroupDocs.Search으로 검색하기"
head_description: "GroupDocs.Search for .NET을(를) 사용하여 다양한 문서 형식에서 텍스트 검색을 효율적으로 수행할 수 있습니다. C#와 함께 사용하세요."

############################# Header ############################
title: "고급 문서 텍스트 검색" 
description: "GroupDocs.Search for .NET은(는) 널리 사용되는 문서 형식에서 텍스트 검색을 간소화하여, .NET 애플리케이션에서 강력한 검색 쿼리를 생성할 수 있게 해줍니다."
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
       [GroupDocs.Search for .NET](/search/net/)은(는) 문서에서 전체 텍스트 검색 및 인덱싱을 위해 설계된 강력한 라이브러리입니다. PDF, Word, PowerPoint, Excel, 이미지 및 ZIP 파일을 포함한 70개 이상의 파일 형식을 지원하여 빠르고 정확한 검색 결과를 보장합니다.

############################# Steps ############################
steps:
    enable: true
    title: "XLSX 문서에서 텍스트 검색 수행 방법"
    content: |
      [GroupDocs.Search](/search/net/)은(는) XLSX 문서에서 고급 콘텐츠 검색 작업을 가능하게 하여, .NET 애플리케이션에서 세분화된 검색 결과를 제공합니다.
      
      1. 검색 인덱스를 저장할 폴더를 설정합니다.
      2. XLSX 파일이 포함된 폴더를 선택합니다.
      3. 추가 검색 옵션을 구성합니다.
      4. 검색을 실행하고 결과를 검토합니다.
   
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
        // 검색 인덱스의 경로를 정의합니다.
        Index index = new Index("c:/MyIndex");

        // 검색할 문서가 포함된 폴더를 선택합니다.
        index.Add("c:/MyDocuments");

        // 동음이의어 검색을 활성화하여 비슷한 발음을 찾습니다.
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // 복잡한 검색 쿼리를 실행합니다.
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "고급 검색 및 인덱싱 기능"
  description: "GroupDocs.Search for .NET은(는) 70개 이상의 파일 형식에서 텍스트 검색 및 인덱싱을 강화하여 정보 검색 및 관리를 위한 효율적인 도구를 제공합니다."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "강력한 텍스트 검색"
      content: "PDF, Word 문서, PowerPoint 프레젠테이션 및 스프레드시트를 포함한 여러 문서 유형에서 텍스트를 검색합니다. 정확한 일치, 유사 검색 및 와일드카드와 같은 기능을 사용하여 결과를 세분화하세요."

    # feature loop
    - title: "대량 데이터 세트를 위한 빠른 인덱싱"
      content: "정보의 신속한 검색을 위해 검색 인덱스를 생성 및 관리합니다. 인덱싱은 방대한 문서 컬렉션을 쉽게 검색할 수 있도록 최적화합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 검색을 수행하며, 다양한 키보드 레이아웃과 단어 변형을 지원하여 정확도를 높입니다."

    # feature loop
    - title: "사용자 정의 가능한 검색 설정"
      content: "대소문자 구분, 날짜 범위 필터 및 단어 제외와 같은 옵션으로 검색 매개변수를 세밀하게 조정하여 더 나은 결과를 얻습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 검색 쿼리 실행하기"
      content: |
        이 예제는 XLSX 문서에 대한 검색 쿼리를 적용하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 검색 인덱스를 위한 폴더를 정의합니다.
          Index index = new Index("c:/MyIndex");
              
          // 문서 파일의 경로를 지정합니다.
          index.Add("c:/MyDocuments");

          // 보호된 문서에 대한 비밀번호를 제공합니다.
          index.Dictionaries.DocumentPasswords.Add("protected.xlsx", "123456");

          // 유사 검색을 활성화하여 유사한 단어를 찾습니다.
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // 검색 결과를 검색합니다.
          SearchResult result = index.Search("Loarem", options);
          
          // 검색 출력을 처리합니다.
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    title: "주요 기능 탐색하기"
    exclude: "document"
    description: "고급 및 고성능 검색 기능을 활용하세요."
    items: 
          
        # operation loop 1
        - name: "조건부 검색"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "부울 조건을 사용하여 문서에서 정보 찾기"

        # operation loop 2
        - name: "대소문자 구분 검색"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "대소문자 구분을 고려하여 검색 정확도를 향상"

        # operation loop 3
        - name: "문서 색인화"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "문서를 한 번 색인화하고 여러 검색에 재사용"

        # operation loop 4
        - name: "검색 필터"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "처리 중인 데이터를 좁혀주기 위해 필터 사용"

        # operation loop 5
        - name: "정확한 구문"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "특정 문장이나 구문 검색"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "비즈니스 문서에서 검색하기"
    exclude: "XLSX"
    description: "GroupDocs.Search은(는) 70개 이상의 파일 형식을 지원하며, 오피스 문서를 포함하여 인덱싱 기능을 갖춘 빠르고 효율적인 검색을 가능하게 합니다."
    items: 
        # format loop 1
        - name: "DOCX 문서에서 검색"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 문서에서 검색"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 문서에서 검색"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 문서에서 검색"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 문서에서 검색"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---