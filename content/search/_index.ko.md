---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: ko

############################# Head ############################
head_title: "문서 텍스트 검색 및 인덱싱 | API 및 무료 웹 애플리케이션"
head_description: " 우리의 API 또는 무료 온라인 문서 검색 앱을 사용하여 PDF, MS Office, OpenDocument 및 기타 인기 파일 형식에서 효율적인 텍스트 검색과 데이터 인덱싱을 수행하십시오."

############################# Header ############################
title: "포괄적인 문서 검색 및 인덱싱 솔루션"
description:  |
  PDF, Microsoft Office, OpenOffice 및 많은 다른 문서 파일 형식에서 텍스트 검색 및 인덱싱을 수행하십시오.

  고급 전체 텍스트 검색 기능을 통해 대규모 문서 컬렉션에서 정보를 신속하게 찾아보십시오.

  정확도와 결과를 높이기 위해 동의어, 모호 검색 및 어간 추출과 같은 검색 기능을 사용자 정의하십시오.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "플랫폼 선택"
  title: "플랫폼 독립성"
  description: "GroupDocs.Search는 다음 운영 체제 및 프레임워크와 호환됩니다:"
  details_link_title: "자세히 알아보기"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> 기타 텍스트 편집기
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "GroupDocs.Search의 주요 기능"
  description: "GroupDocs.Search는 인기 있는 문서 형식에서 텍스트를 인덱싱하고 검색하기 위한 강력한 도구를 제공합니다. 고급 검색 기능으로 문서 관리를 간소화하고 향상시킵니다."

  items:
    # items loop
    - icon: "view"
      title: "고급 텍스트 검색"
      content: "인덱스된 문서에서 빠르고 정확한 텍스트 검색을 수행하십시오."

    # items loop
    - icon: "manipulate"
      title: "사용자 정의 가능한 검색 옵션"
      content: "정확한 결과를 얻기 위해 모호 검색, 동의어 및 어간 추출과 같은 기능을 활용하십시오."

    # items loop
    - icon: "merge"
      title: "다양한 형식 지원"
      content: "Microsoft Office, PDF, OpenOffice 및 기타 일반 형식에서 콘텐츠를 인덱스하고 검색하십시오."

    # items loop
    - icon: "additional"
      title: "효율적인 인덱싱"
      content: "대규모 문서 컬렉션에 대한 인덱스를 신속하게 생성하고 유지하십시오."

############################# Code samples ############################
code_samples:
  enable: true
  title: "인기 문서 형식에서 텍스트 검색"
  description: "GroupDocs.Search 코드 예제"
  items:
    # code sample loop
    - title: "텍스트 검색"
      content: |
       GroupDocs.Search는 문서에서 텍스트를 찾는 강력한 도구입니다. 특정 폴더에 저장된 여러 형식의 문서에서 검색할 수 있습니다. 검색 결과는 별도의 폴더에 저장되어 검색을 다시 수행하지 않고도 액세스 및 재사용할 수 있습니다.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Index 클래스의 인스턴스를 생성하고 인덱스를 저장할 폴더를 지정합니다.
            Index index = new Index("\\Index Folder");

            //검색이 수행될 문서의 경로를 지정합니다.
            index.Add("\\Documents Folder");

            //SearchOptions 객체의 인스턴스를 생성합니다.
            SearchOptions options = new SearchOptions();

            //원하는 텍스트에 대해 검색을 수행합니다.
            SearchResult result = index.Search("ipsum dolor", options);

            //검색 결과를 처리하고 관리합니다.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Index 클래스의 인스턴스를 생성하고 인덱스를 저장할 폴더를 지정합니다.
            Index index = new Index("\\Index Folder");

            //검색이 수행될 문서의 경로를 지정합니다.
            index.add("\\Documents Folder");

            //SearchOptions 객체의 인스턴스를 생성합니다.
            SearchOptions options = new SearchOptions();

            //원하는 텍스트에 대해 검색을 수행합니다.
            SearchResult result = index.search("ipsum dolor", options);

            //검색 결과를 처리하고 관리합니다.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Index 클래스의 인스턴스를 생성하고 인덱스를 저장할 폴더를 지정합니다.
            const index = new searchLib.Index('\\Index Folder');

            //검색이 수행될 문서의 경로를 지정합니다.
            index.add('\\Documents Folder');

            //SearchOptions 객체의 인스턴스를 생성합니다.
            const options = new searchLib.SearchOptions();

            //원하는 텍스트에 대해 검색을 수행합니다.
            const result = index.search('ipsum dolor', options);

            //검색 결과를 처리하고 관리합니다.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "70개 이상의 파일 형식 지원"
  description: "GroupDocs.Search는 거의 모든 널리 사용되는 파일 형식을 지원합니다."

############################# Metrics ###############################
metrics:
  enable: true
  title: "우리 제품 통계"
  description: "우리의 성과, 도달 범위 및 성장률을 보여주는 주요 지표를 발견하십시오."

  items:
    # items loop
    - number: "70+"
      title: "지원되는 형식"
      content: "70개 이상의 인기 문서 형식과의 호환성을 제공합니다."

    # items loop
    - number: "500k"
      title: "NuGet 다운로드"
      content: "GroupDocs.Search for .NET는 NuGet에서 500,000회 이상 다운로드되었습니다."

    # items loop
    - number: "12k"
      title: "Maven 다운로드"
      content: "Java 개발자가 Maven에서 GroupDocs.Search를 12,000회 이상 다운로드했습니다."

    # items loop
    - number: "150+"
      title: "만족한 고객"
      content: "전 세계의 개발자 및 주요 기업이 혁신적인 솔루션을 위해 우리 제품에 의존합니다."


############################# Customers ###############################
customers:
  enable: true
  title: "우리의 행복한 고객들"
  description: "GroupDocs 라이브러리는 전 세계의 주요 브랜드와 조직으로부터 신뢰받고 있습니다."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "지금 시작하세요!"
  description: "선택한 플랫폼에서 GroupDocs.Search을 무료로 체험하십시오."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "자주 묻는 질문"
  description: "GroupDocs.Search에 대한 일반적인 질문에 대한 답을 찾으십시오."

  items:
    # items loop
    - question: "GroupDocs.Search는 문서 검색을 위해 외부 도구가 필요합니까?"
      answer: "아니요, GroupDocs.Search는 독립형 솔루션으로 작동하며, 검색을 수행하기 위해 Adobe Acrobat이나 Microsoft Office와 같은 추가 도구나 소프트웨어가 필요하지 않습니다."

    # items loop
    - question: "GroupDocs.Search를 구매하기 전에 테스트할 수 있습니까?"
      answer: "예, 가능합니다! GroupDocs.Search는 무료 평가판을 제공합니다. 이 기능을 탐색할 수 있지만, 평가판 버전은 워터마크 또는 기능 제한과 같은 제한 사항이 포함될 수 있습니다. 모든 기능을 잠금 해제하려면 무료 30일 임시 라이센스를 요청할 수 있습니다. [임시 라이센스](https://purchase.groupdocs.com/temporary-license/) 페이지에서 자세히 알아보십시오."

    # items loop
    - question: "어떤 라이센스 옵션이 있습니까?"
      answer: "GroupDocs.Search에 대해 여러 라이센스 모델을 제공하며, 이는 다양한 요구에 맞춰 조정됩니다. 팀 크기, 사용 시나리오 또는 클라이언트 배포를 위한 SDK/API가 필요한지에 따라 라이센스를 선택하십시오. 유연한 사용을 원하시면 실제 사용량에 따라 비용을 지불하는 계량 라이센스를 고려하십시오. [가격 책정](https://purchase.groupdocs.com/pricing/search/net/) 페이지에서 옵션에 대해 자세히 알아보십시오."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search 웹 앱"
  description: "우리의 무료 웹 애플리케이션을 사용하여 GroupDocs.Search을 탐색하십시오. 브라우저에서 직접 70개 이상의 인기 파일 형식에서 텍스트 검색 및 인덱싱을 수행하십시오—완전히 무료입니다."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "PDF, Excel, Word, PowerPoint 및 기타 파일 형식에서 웹 브라우저로 직접 검색하십시오."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "소프트웨어 설치 없이 DOCX를 업로드하여 고급 텍스트 검색을 수행하십시오."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "다양한 형식에서 PDF 인덱싱 및 검색 기능을 무료로 테스트하십시오."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---