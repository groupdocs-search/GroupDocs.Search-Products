
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Thực hiện tìm kiếm nhạy cảm với chữ hoa trong XLSX với Java"
head_description: "API GroupDocs.Search for Java giúp các lập trình viên Java thực hiện tìm kiếm nhạy cảm với chữ hoa trên nhiều loại tài liệu."

############################# Header ############################
title: "Tìm Kiếm Tài Liệu Nhạy Cảm Với Chữ Hoa" 
description: "GroupDocs.Search for Java cho phép bạn triển khai chức năng tìm kiếm chính xác nhạy cảm với chữ hoa trong các dự án Java của bạn."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nhận Miễn Phí"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tìm Hiểu Về GroupDocs.Search"
    link: "/search/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) là một công cụ đa năng cho việc tìm kiếm và lập chỉ mục văn bản trên nhiều tài liệu khác nhau. Nó hỗ trợ hơn 70 định dạng như PDF, tệp Word, bài thuyết trình PowerPoint, bảng tính Excel, hình ảnh và file ZIP, giúp bạn hiệu quả xử lý các tập dữ liệu lớn.

############################# Steps ############################
steps:
    enable: true
    title: "Hướng Dẫn Tìm Kiếm Nhạy Cảm Với Chữ Hoa Trong Tệp XLSX"
    content: |
      Sử dụng [GroupDocs.Search](/search/java/), bạn có thể thực hiện tìm kiếm nhạy cảm với chữ hoa trong các tài liệu XLSX, nâng cao các dự án Java của bạn.
      
      1. Đặt thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tệp XLSX.
      3. Chạy tìm kiếm nhạy cảm với chữ hoa và thu thập kết quả.
      4. Xử lý và sử dụng các kết quả tìm kiếm.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Kết quả tìm kiếm"
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
        copy_tip: "nhấn để sao chép"
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
        // Định nghĩa vị trí lưu trữ chỉ mục
        Index index = new Index("c:/MyIndex");

        // Trỏ đến thư mục chứa tài liệu để tìm kiếm
        index.add("c:/MyDocuments");

        // Kích hoạt chế độ nhạy cảm với chữ hoa trong cài đặt tìm kiếm
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Thực hiện tìm kiếm
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Công Cụ Tìm Kiếm và Lập Chỉ Mục Nâng Cao"
  description: "Với GroupDocs.Search for Java, bạn có thể hợp lý hóa việc tìm kiếm và lập chỉ mục tài liệu cho hơn 70 định dạng, giúp việc tìm kiếm và tổ chức thông tin trở nên dễ dàng hơn."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Các điểm nổi bật của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm Kiếm Văn Bản Linh Hoạt"
      content: "Tìm kiếm qua các tài liệu như PDF, tệp Word, bảng tính và bài thuyết trình một cách hiệu quả. Sử dụng các công cụ như tìm kiếm chính xác, tìm kiếm mờ và hỗ trợ ký tự đại diện để làm rõ kết quả."

    # feature loop
    - title: "Quản Lý Chỉ Mục Hiệu Quả"
      content: "Tổ chức và lập chỉ mục các tập dữ liệu lớn để cải thiện tốc độ tìm kiếm và hiệu suất khi xử lý các bộ sưu tập tài liệu lớn."

    # feature loop
    - title: "Hỗ Trợ Ngôn Ngữ Toàn Cầu"
      content: "Thực hiện tìm kiếm trên hơn 80 ngôn ngữ, phục vụ cho các bố cục bàn phím khác nhau và các biến thể ngôn ngữ để đạt được độ chính xác tốt hơn."

    # feature loop
    - title: "Bộ Lọc Tìm Kiếm Tùy Chỉnh"
      content: "Điều chỉnh tiêu chí tìm kiếm với các tùy chọn như nhạy cảm với chữ hoa, lọc theo khoảng thời gian và loại trừ các từ hoặc dữ liệu không mong muốn trong quá trình lập chỉ mục."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ví Dụ: Tìm Kiếm Nhạy Cảm Với Chữ Hoa"
      content: |
        Ví dụ này minh họa cách thực hiện tìm kiếm nhạy cảm với chữ hoa cho các tài liệu XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Định nghĩa thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Chỉ định vị trí của thư mục tài liệu
          index.add("c:/MyDocuments");

          // Thiết lập một truy vấn tìm kiếm
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Kích hoạt tính năng nhạy cảm với chữ hoa trong tùy chọn tìm kiếm
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Thực hiện tìm kiếm tài liệu
          SearchResult result = index.search(wordQuery, options);
          
          // Xử lý các kết quả đã thu thập
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
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
  description: "Hãy thử các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
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
    title: "Tổng Quan Các Tính Năng Chính"
    exclude: "case-sensitive"
    description: "Khám phá khả năng tìm kiếm mạnh mẽ và hiệu quả mà GroupDocs.Search for Java cung cấp."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Định Dạng Tệp Được Hỗ Trợ Cho Tìm Kiếm"
    exclude: "XLSX"
    description: "GroupDocs.Search hoạt động với hơn 70 định dạng tài liệu phổ biến, cung cấp các cài đặt tìm kiếm tùy chỉnh và lập chỉ mục hiệu quả."
    items: 
        # format loop 1
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---