
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: ko
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "XLSX 문서 내 검색, .NET에서 불리언 연산자 사용"
head_description: "GroupDocs.Search for .NET API는 C# 개발자들이 AND, OR 및 NOT과 같은 불리언 연산자를 사용하여 문서 콘텐츠를 검색할 수 있도록 합니다."

############################# Header ############################
title: "불리언 논리 텍스트 검색" 
description: "GroupDocs.Search for .NET는 .NET 애플리케이션 내에서 불리언 연산자(AND, OR, NOT)를 사용하여 고급 검색 쿼리를 구성하는 것을 간편하게 만듭니다."
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
       [GroupDocs.Search for .NET](/search/net/)는 문서 내 텍스트 검색 및 인덱싱을 위한 종합 라이브러리입니다. PDF, Word, PowerPoint, Excel, 이미지, ZIP 파일 등 70개 이상의 파일 형식을 지원하여 대량의 정보를 효율적으로 처리할 수 있습니다.

############################# Steps ############################
steps:
    enable: true
    title: "불리언 논리를 사용하여 XLSX 문서 콘텐츠 검색하기"
    content: |
      [GroupDocs.Search](/search/net/)는 XLSX 문서 콘텐츠 검색을 간단하게 해줍니다. .NET 애플리케이션 내에서 결과를 세분화하기 위해 불리언 논리 검색 조건을 제공합니다.
      
      1. 검색 인덱스를 저장할 폴더를 지정합니다.
      2. XLSX 파일이 포함된 폴더를 선택합니다.
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
        // 인덱스 폴더의 경로 설정
        Index index = new Index("c:/MyIndex");

        // 검색할 문서가 포함된 폴더 지정
        index.Add("c:/MyDocuments");

        // 복잡한 쿼리를 사용하여 검색 실행
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "문서 검색 및 인덱싱을 위한 고급 기능 탐색"
  description: "GroupDocs.Search for .NET 라이브러리는 70개 이상의 파일 형식에 대한 텍스트 검색 및 인덱싱을 간소화합니다. 고급 검색 도구를 사용하여 정보를 신속하게 찾고 관리할 수 있습니다."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search의 주요 기능"
  features:
    # feature loop
    - title: "강력한 텍스트 검색"
      content: "PDF, Word 문서, PowerPoint 프레젠테이션 및 스프레드시트 등 다양한 파일 유형에서 텍스트를 검색합니다. 정확한 일치, 유사 검색 및 와일드카드 사용과 같은 기능을 활용하여 결과를 세분화할 수 있습니다."

    # feature loop
    - title: "대규모 데이터 세트 인덱싱"
      content: "더 빠른 검색을 위한 인덱스를 생성하고 유지관리합니다. 인덱싱은 데이터를 조직하고 구조화하여 방대한 문서 컬렉션을 더 쉽게 검색할 수 있게 합니다."

    # feature loop
    - title: "다국어 지원"
      content: "80개 이상의 언어로 문서를 검색할 수 있으며, 다양한 키보드 레이아웃 및 형태소 단어 형태를 지원하여 검색 정확도를 높입니다."

    # feature loop
    - title: "사용자 지정 가능한 검색 옵션"
      content: "대소문자 구분, 날짜 범위 필터와 같은 기능과 인덱싱 중 특정 단어나 데이터를 제외하는 기능으로 검색 설정을 조정할 수 있습니다."
      
  code_samples_ext:
    # code sample ext loop
    - title: "고급 불리언 검색 쿼리 사용하기"
      content: |
        이 예제는 XLSX 문서 검색을 위한 불리언 쿼리를 적용하는 방법을 보여줍니다.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 검색 인덱스를 위한 폴더 설정
          Index index = new Index("c:/MyIndex");
              
          // 검색할 문서의 경로 지정
          index.Add("c:/MyDocuments");

          // 불리언 논리를 적용하여 검색 쿼리 생성
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // 검색 결과를 가져옵니다.
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.xlsx"
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
    title: "주요 기능 발견하기"
    exclude: "boolean"
    description: "고급 및 효율적인 검색 기능을 탐색합니다."
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
    title: "인기 문서 형식 내에서 검색"
    exclude: "XLSX"
    description: "GroupDocs.Search는 70개 이상의 파일 형식을 지원합니다. 검색 규칙을 사용자 지정하고 인덱싱을 통해 시간과 노력을 절약하세요."
    items: 
        # format loop 1
        - name: "DOCX 조건부 검색"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "마이크로소프트 워드 오픈 XML 문서"
          
        # format loop 2
        - name: "PDF 조건부 검색"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "어도비 휴대용 문서 형식"
          
        # format loop 3
        - name: "PPTX 조건부 검색"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "파워포인트 오픈 XML 프레젠테이션"

        # format loop 4
        - name: "TXT 조건부 검색"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "텍스트 문서"
          
        # format loop 5
        - name: "XLSX 조건부 검색"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "마이크로소프트 엑셀 오픈 XML 스프레드시트"
  

---