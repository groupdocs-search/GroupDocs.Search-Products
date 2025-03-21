
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tìm kiếm Boolean trong XLSX với Java"
head_description: "Với GroupDocs.Search for Java, các nhà phát triển có thể thực hiện tìm kiếm tài liệu bằng cách sử dụng các toán tử Boolean như AND, OR, và NOT."

############################# Header ############################
title: "Tìm kiếm văn bản Boolean" 
description: "Sử dụng GroupDocs.Search for Java để tạo các truy vấn tìm kiếm Boolean nâng cao (AND, OR, NOT) trong các dự án Java của bạn."
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
    title: "Giới thiệu về GroupDocs.Search"
    link: "/search/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) là một thư viện đa năng được thiết kế cho việc tìm kiếm văn bản và chỉ mục dữ liệu trong tài liệu. Nó hỗ trợ hơn 70 loại tệp, bao gồm PDF, Word, Excel, PowerPoint, hình ảnh và các tệp ZIP, cho phép tìm kiếm hiệu quả trong những tập dữ liệu lớn.

############################# Steps ############################
steps:
    enable: true
    title: "Cách thực hiện tìm kiếm boolean trong tài liệu XLSX"
    content: |
      [GroupDocs.Search](/search/java/) cho phép tìm kiếm văn bản trong các tài liệu XLSX. Với hỗ trợ cho các điều kiện boolean, bạn có thể cải thiện độ chính xác tìm kiếm trong các ứng dụng Java.
      
      1. Chỉ định thư mục để lưu chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tài liệu XLSX.
      3. Thực hiện truy vấn tìm kiếm và lấy kết quả.
      4. Xử lý các kết quả thu được.
   
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
        // Đặt đường dẫn cho thư mục chỉ mục
        Index index = new Index("c:/MyIndex");

        // Cung cấp đường dẫn thư mục chứa các tài liệu cho tìm kiếm
        index.add("c:/MyDocuments");

        // Thực hiện tìm kiếm với truy vấn phức tạp
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Công cụ mạnh mẽ để tìm kiếm và lập chỉ mục tài liệu"
  description: "GroupDocs.Search for Java đơn giản hóa việc tìm kiếm văn bản và lập chỉ mục dữ liệu cho hơn 70 định dạng. Nó cung cấp các công cụ tiên tiến cho phép bạn tìm và quản lý nội dung một cách hiệu quả."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản toàn diện"
      content: "Tìm kiếm qua nhiều định dạng như PDF, tài liệu Word, bản trình bày, bảng tính và nhiều hơn nữa. Sử dụng các tùy chọn như khớp chính xác, tìm kiếm gần đúng và truy vấn ký tự đại diện để cải thiện kết quả."

    # feature loop
    - title: "Lập chỉ mục dữ liệu hiệu quả"
      content: "Xây dựng và duy trì các chỉ mục để tìm kiếm tài liệu nhanh chóng hơn. Tính năng này tổ chức dữ liệu một cách hiệu quả, giúp dễ dàng xử lý các bộ sưu tập tài liệu lớn."

    # feature loop
    - title: "Hỗ trợ đa ngôn ngữ"
      content: "Tìm kiếm trong các tài liệu được viết bằng hơn 80 ngôn ngữ. Tăng cường độ chính xác bằng cách sử dụng các hình thức từ vựng hình thái và các dạng bàn phím khác nhau."

    # feature loop
    - title: "Tùy chỉnh tìm kiếm linh hoạt"
      content: "Điều chỉnh cài đặt tìm kiếm với các tính năng như phân biệt chữ hoa chữ thường, bộ lọc khoảng thời gian và loại trừ để cải thiện kết quả của bạn."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử dụng các truy vấn tìm kiếm boolean phức tạp"
      content: |
        Ví dụ này minh họa cách thực hiện các tìm kiếm Boolean trong các tệp XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Đặt thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Cung cấp đường dẫn đến các tài liệu cần tìm kiếm
          index.add("c:/MyDocuments");

          // Xây dựng truy vấn bằng cách sử dụng logic Boolean
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Lấy kết quả tìm kiếm
          SearchResult result = index.search(booleanQuery);
          
          // Xử lý các kết quả đã thu được
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
            link: "/examples/search/formats/searchboolean.xlsx"
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
    title: "Các tính năng chính trong tầm tay"
    exclude: "boolean"
    description: "Khám phá các khả năng tìm kiếm mạnh mẽ và hiệu quả"
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
    title: "Tìm kiếm các định dạng tài liệu phổ biến"
    exclude: "XLSX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp, cho phép bạn tùy chỉnh quy tắc tìm kiếm và sử dụng lập chỉ mục để tối ưu hóa hiệu suất."
    items: 
        # format loop 1
        - name: "Tìm kiếm DOCX theo điều kiện"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm PDF theo điều kiện"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm PPTX theo điều kiện"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm TXT theo điều kiện"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm XLSX theo điều kiện"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---