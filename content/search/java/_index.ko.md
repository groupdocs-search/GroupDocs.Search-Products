---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

head_title: "문서, PDF, Office 및 웹용 Java 텍스트 검색 및 인덱싱 API"
head_description: "PDF, Word, Excel, 프레젠테이션, 이메일 및 웹 파일 형식과 같은 문서에서 데이터를 검색, 색인화 및 검색하는 Java 애플리케이션용 고급 텍스트 검색 API."

title: "Java API를 통한 문서 검색 및 색인 생성"
description: "모든 인기 있는 문서 형식에서 텍스트 검색 조작을 수행하는 Java 애플리케이션 빌드."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for Java"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-java.png"
        product: "GroupDocs.Search"
        platform: "Java"

    middle:
        button:
            - link: "#overview"
              text: "개요"

            - link: "#features"
              text: "특징"

            - link: "#support"
              text: "지원하다"

            - link: "https://products.groupdocs.app/search"
              text: "라이브 데모"

            - link: "https://purchase.groupdocs.com/pricing/search/java"
              text: "가격"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/java/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Search for Java를 사용하면 최종 사용자가 이전과는 다른 방식으로 검색 작업을 수행할 수 있도록 하는 비즈니스 응용 프로그램을 생성할 수 있습니다. Java API를 사용하면 기본에서 고급 수준의 텍스트 검색 기능을 작동할 수 있습니다. 여러 인덱스를 만들고 병합합니다. 단순, 부울, 정규식(Regex), 퍼지 및 기타 유형의 쿼리를 사용하여 인덱스를 빠르고 스마트하게 검색합니다. GroupDocs.Search for Java는 널리 사용되는 모든 파일 형식을 지원하므로 파일, 문서, 이메일 및 아카이브에서 필요한 정보를 가져올 수 있습니다.
    tabs:
      enable: true     
      
      tab_one:
        description: |
          다음은 GroupDocs.Search for Java의 개요입니다.

        left:
          enable: true
          icon: "fas fa-search"
          title: "인덱싱"
          content: |
            * 생성 및 관리
            * 여러 인덱스 병합
            * 멀티 스레딩 비동기 인덱싱
            * 컴팩트 인덱싱
            * 아카이브 파일 인덱싱
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "고급 검색 및 검색어"
          content: |
            * 퍼지 검색
            * 동의어 검색
            * 이메일 검색
            * 동음이의어 용어 처리
            * 보호된 파일 검색
            * 단순한
            * 와일드카드
            * 정규식(Regex)
            * 패싯 및 부울
            * 대소문자 구분
      
      tab_two:
        description: |
          GroupDocs.Search for Java는 Microsoft Office, 이미지, 다이어그램 및 기타 여러 가지를 포함하여 널리 사용되는 모든 [문서 파일 형식](https://docs.groupdocs.com/search/java/supported-document-formats/)을 지원합니다.

        left:
          enable: true
          table:
            - title: "마이크로소프트 오피스 형식"
              content: |
                * **단어**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **엑셀**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **파워포인트**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **프로젝트**: MPP
                * **다이어그램**: VSD, VSS
                * **Microsoft 컴파일 HTML**: CHM
                * **원노트**: 하나

        right:
          enable: true
          table:
            - title: "OpenDocument 및 기타 형식"
              content: |
                * **Portable Document Format**: PDF
                * **OpenDocument**: ODT, OTT, ODS, OTS, ODP
                * **이메일**: PST, OST, MSG, EML, EMLX
                * **웹 파일 형식**: XML, HTM, HTML, XHTML, MHT, MHTML
                * **오디오**: MP3, WAV
                * **동영상**: AVI, MOV, QT, FLV, ASF
                * **텍스트**: TXT
                * **서식 있는 텍스트 형식**: RTF
                * **마크다운 문서 파일**: MD
                * **이미지**: BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **기타**: 토렌트, ZIP, DCM, DJVU, EPUB, FB2

      tab_three:
        description: |
          Java용 GroupDocs.Search는 다음 운영 체제, 프레임워크 및 패키지 ‎관리자:‎를 지원합니다.
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "운영체제"
              content: |
                * 마이크로소프트 윈도우 데스크탑
                * 마이크로소프트 윈도우 서버
                * 리눅스
                * 맥 OS

            - icon: "fas fa-code"
              title: "지원되는 프레임워크"
              content: |
                * 자바 7(1.7) 이상

        right:
          enable: true
          table:
            - icon: "fas fa-cogs"
              title: "개발 환경"
              content: |
                * 넷빈
                * IntelliJ 아이디어
                * 이클립스
            - icon: "fas fa-tools"
              title: "빌드 자동화 도구"
              content: |
                * 메이븐

features:
    enable: true
    title: "GroupDocs.Java 기능 검색"

    feature:
      - icon: "fas fa-copy"
        content: "비동기 멀티스레딩을 사용하여 디스크 또는 메모리에 인덱스 구축"

      - icon: "fas fa-eye"
        content: "인덱스 생성 및 업데이트 진행 상황 보기"

      - icon: "fas fa-bolt"
        content: "특정 파일에 대한 인덱싱을 선택적으로 건너뛰고 특정 단어를 건너뛰어 더 빠르게 인덱싱"
      
      - icon: "fas fa-file-powerpoint"
        content: "가져오기를 수행하거나 목록을 사용하여 인덱싱 및 파일로 내보내기 중 문자 수정"

      - icon: "fas fa-code"
        content: "오류 인덱싱 및 모순 설정에 대한 경고 사용자의 경우 인덱스 다시 로드"

      - icon: "fas fa-cloud"
        content: "최근 처리된 파일에 대한 색인 상태 알림"

      - icon: "fas fa-remove-format"
        content: "다른 ZIP 아카이브 내에서 압축된 아카이브 색인 생성 및 아카이브에서 색인화된 파일 목록 가져오기"

      - icon: "fas fa-comment-slash"
        content: "컴팩트 인덱싱 및 비밀번호 보안 문서 인덱싱으로 공간 절약‎"

      - icon: "fas fa-location-arrow"
        content: "인덱스 또는 소스 파일에서 문서 텍스트 추출"

      - icon: "fas fa-border-all"
        content: "HTML 형식의 텍스트를 파일로 추출하고 HTML에서 검색 결과를 탐색하기 위한 URL 생성"

      - icon: "fas fa-wrench"
        content: "인덱싱하는 동안 각 문서에 임의의 추가 필드 추가"

      - icon: "fas fa-columns"
        content: "퍼지 검색에 대한 유사성 수준 구성 및 최상의 결과 표시"

      - icon: "fas fa-file-word"
        content: "Fuzzy Search를 통한 스마트한 오타 관리"

      - icon: "fas fa-envelope"
        content: "패싯 및 부울 검색을 동시에 사용"

      - icon: "fas fa-print"
        content: "동의어 검색 구성 및 수행 및 동음이의어 용어를 현명하게 처리"

      - icon: "fas fa-file-archive"
        content: "날짜 범위 및 대소문자 구분을 검색 매개변수로 사용"

      - icon: "fas fa-lock"
        content: "Aspose.Email API를 통해 이메일 메시지를 검색하고 찾아보기 위한 색인 만들기"

      - icon: "fas fa-file-code"
        content: "맞춤법 검사 및 와일드 카드와 함께 검색 구문 사용 및 쿼리에서 특수 문자 건너뛰기"
      
      - icon: "fas fa-fill-drip"
        content: "여러 쿼리를 결합하여 단일 개체 트리 만들기"

      - icon: "fas fa-file-excel"
        content: "거대한 인덱스를 빠르게 검색하기 위해 검색을 더 작은 청크로 분할"

      - icon: "fas fa-heading"
        content: "스트림 및 데이터 구조에서 문서 색인 생성"

      - icon: "fas fa-project-diagram"
        content: "검색 결과에서 문서 필터링 설정"

      - icon: "fas fa-cube"
        content: "기본 동의어 사전에 영어 동의어 추가"

      - icon: "fab fa-uncharted"
        content: "철자가 틀린 경우 대체 단어 제안을 제공하기 위해 찾은 각 단어의 정확한 발생 횟수 활성화"

      - icon: "fab fa-uncharted"
        content: "다시 인덱싱하지 않고 인덱싱된 문서에 텍스트 속성 추가"

      - icon: "fab fa-uncharted"
        content: "문자를 기반으로 인덱싱 및 검색 작업 수행"

      - icon: "fab fa-uncharted"
        content: "비텍스트 문서 형식의 인덱스 메타데이터"

    more_feature:
      - title: "인덱싱 및 검색 작업"
        content: |
          인덱싱은 GroupDocs.Search for Java에서 데이터를 수집하고 정확하고 효율적인 검색 작업을 위해 데이터를 저장 및 구문 분석하는 데 사용됩니다. Java용 GroupDocs.Search는 검색을 수행하기 위해 이러한 색인을 자주 사용합니다.

          * **Create Index**: Index 폴더를 생성하고 해당 폴더에 문서를 추가/인덱싱합니다.
          * **인덱스 로드**: 기존 인덱스를 로드합니다.
          * **색인에 문서 추가**: 기존 색인에 문서를 비동기식으로 추가합니다.
          * **인덱스 업데이트**: 문서가 수정, 추가 또는 삭제될 때마다 기존 인덱스를 업데이트합니다. 이렇게 하면 검색 결과가 최신 상태로 유지됩니다.
          
          ```java
          / Creating index
          Index index = new Index("c:\\MyIndex");
          // 인덱스에 문서 추가
          index.addToIndex("c:\\MyDocuments");
          // 'principal', 'principle', 'principles', 'principally'가 있는 문서에서 '영향' 또는 '효과' 단어 검색
          SearchResults results = index.search("?ffect & princip?(2~4)");
          ```
      - title: "여러 인덱스를 병합하여 검색 효율성 향상"
        content: "GroupDocs.Search for Java API는 여러 인덱스를 공통 인덱스로 병합하는 기능을 제공합니다. 자주 수정되는 인덱스의 경우 여러 개의 델타 인덱스가 생성됩니다. 그러나 이 접근 방식은 검색 성능을 저하시킵니다. GroupDocs.Search for Java는 다양한 델타 인덱스를 병합하여 하나의 공통 인덱스를 생성하여 이러한 병목 현상을 극복합니다. 이 공통 병합 인덱스에는 병합된 델타 인덱스의 모든 정보가 포함됩니다. 이 접근 방식은 델타 인덱스를 변경하지 않은 상태로 유지하면서 검색 효율성을 크게 향상시킵니다. 이 프로세스를 추가로 조정하기 위해 다양한 기능을 구성할 수 있습니다.."

      - title: "다양한 키보드 레이아웃의 검색어 인식"
        content: "GroupDocs.Search for Java는 키보드 레이아웃과 일치하지 않는 검색어를 인식합니다. 현재 GroupDocs.Search for Java는 88개 언어와 164개 키보드 레이아웃을 성공적으로 인식할 수 있습니다.‎"

      - title: "형태소 단어 형식을 사용하여 검색"
        content: "GroupDocs.Search for Java를 사용하면 다양한 단어 형식을 자유롭게 검색할 수 있습니다. 특정 명사의 단수형과 복수형을 검색할 수 있습니다. 또는 동사의 모든 형태를 검색하도록 선택할 수 있습니다. 어근, 3인칭 단수, 단순과거 등 다양한 형태로 검색이 가능합니다. 영어가 아닌 언어의 경우 사용자 지정 단어 형식을 구성할 수 있습니다.."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Search는 다른 인기 있는 개발 환경을 위한 문서 보기 API를 제공합니다."

    solution:
        - img_alt: "GroupDocs.Search for .NET"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-net.png"
          product: "GroupDocs.Search"
          platform: ".NET"
          link: "/search/net/"

back_to_top:
  enable: true
---
