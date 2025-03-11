
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:36
draft: false
lang: vi
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tìm kiếm trong các tài liệu DOCX bằng Java"
head_description: "GroupDocs.Search for Java thêm chức năng tìm kiếm văn bản mạnh mẽ vào các ứng dụng Java, hỗ trợ nhiều định dạng tài liệu doanh nghiệp."

############################# Header ############################
title: "Tìm văn bản trong các tài liệu kinh doanh" 
description: "GroupDocs.Search for Java cho phép bạn tìm kiếm văn bản trong các tài liệu bằng các truy vấn linh hoạt và chính xác. Tích hợp chức năng tìm kiếm vào các ứng dụng Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) là một thư viện mạnh mẽ cho tìm kiếm văn bản nhanh và lập chỉ mục tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm các tiêu chuẩn trong ngành như PDF, Word, Excel và PowerPoint. Nâng cao ứng dụng của bạn với những khả năng tìm kiếm chính xác và tốc độ cao.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm kiếm trong các tài liệu DOCX"
    content: |
      [GroupDocs.Search](/search/java/) cho phép tìm kiếm văn bản nhanh và hiệu quả trong các tài liệu DOCX, hoàn hảo cho các ứng dụng Java.
      
      1. Chỉ định một thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tài liệu của bạn.
      3. Cấu hình các tùy chọn tìm kiếm để giới hạn kết quả ở các tài liệu DOCX.
      4. Chạy tìm kiếm và nhận được kết quả.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        copy_tip: "nhấp để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Thư mục để lưu trữ chỉ mục tìm kiếm tái sử dụng
        Index index = new Index("c:/MyIndex");

        // Thư mục chứa các tài liệu
        index.add("c:/MyDocuments");

        // Lọc tìm kiếm theo định dạng tài liệu
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".docx");

        // Lấy kết quả tìm kiếm
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khả năng tìm kiếm nâng cao"
  description: "GroupDocs.Search for Java cung cấp khả năng tìm kiếm văn bản nâng cao trong hơn 70 định dạng tệp. Việc lập chỉ mục giúp tăng tốc độ tìm kiếm và cải thiện hiệu quả quản lý tài liệu."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản mạnh mẽ"
      content: "Tìm văn bản trong các định dạng tài liệu phổ biến như PDF, tệp Word, bài thuyết trình và bảng tính. Hỗ trợ nhiều phương pháp tìm kiếm, bao gồm tìm kiếm mờ, âm đồng và ký tự đại diện."

    # feature loop
    - title: "Lập chỉ mục tối ưu cho hiệu suất tốt hơn"
      content: "Tạo và tái sử dụng chỉ mục tìm kiếm để nâng cao tốc độ và hiệu quả tìm kiếm, đặc biệt là trong các bộ sưu tập tài liệu lớn."

    # feature loop
    - title: "Hỗ trợ tìm kiếm đa ngôn ngữ"
      content: "Tìm kiếm trong các tài liệu viết bằng hơn 80 ngôn ngữ. Phát hiện các kiểu bàn phím khác nhau và các biến thể từ ngữ để cải thiện độ chính xác."

    # feature loop
    - title: "Tùy chọn tìm kiếm có thể tùy chỉnh"
      content: "Thu hẹp kết quả tìm kiếm với các bộ lọc, biểu thức chính quy và các cài đặt tìm kiếm nâng cao khác."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Lọc tài liệu trước khi tìm kiếm"
      content: |
        Tìm hiểu cách tinh chỉnh tìm kiếm bằng cách sử dụng bộ lọc.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Thiết lập một chỉ mục loại trừ một số định dạng tệp nhất định.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Chỉ định đường dẫn lưu trữ tài liệu.
          index.add("c:/MyDocuments");

          // Lấy kết quả tìm kiếm.
          SearchResult result = index.search("Lorem", options);
          
          // Xử lý và sử dụng các kết quả tìm kiếm.
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Sao chép"
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
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Thử nghiệm các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Các tính năng chính"
    exclude: "filters"
    description: "Thực hiện các tìm kiếm văn bản chính xác và hiệu quả."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm trong các tài liệu kinh doanh"
    exclude: "DOCX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp, giúp bạn dễ dàng tìm kiếm trong các tài liệu văn phòng được sử dụng rộng rãi."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Bản trình bày PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---