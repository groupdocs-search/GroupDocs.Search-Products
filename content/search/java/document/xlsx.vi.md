
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tìm kiếm văn bản trong tài liệu XLSX với GroupDocs.Search cho Java"
head_description: "GroupDocs.Search for Java hỗ trợ các lập trình viên Java tìm kiếm văn bản nhanh chóng trong nhiều định dạng tài liệu khác nhau."

############################# Header ############################
title: "Tìm kiếm văn bản tài liệu thông minh" 
description: "Với GroupDocs.Search for Java, bạn có thể tìm kiếm và trích xuất văn bản từ nhiều loại tài liệu trong ứng dụng Java của bạn một cách liền mạch."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Nhận bản dùng thử miễn phí"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search có chức năng gì?"
    link: "/search/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) là một thư viện tìm kiếm và lập chỉ mục tài liệu mạnh mẽ hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, Word, PowerPoint, Excel, hình ảnh và các tệp ZIP. Nó cho phép tìm kiếm nhanh chóng, chính xác và quy mô cho những bộ sưu tập tài liệu lớn.

############################# Steps ############################
steps:
    enable: true
    title: "Thực hiện tìm kiếm văn bản trong các tệp XLSX"
    content: |
      [GroupDocs.Search](/search/java/) giúp bạn tìm kiếm các tệp XLSX với logic và lập chỉ mục tinh vi, cải thiện sự chính xác trong các ứng dụng Java.
      
      1. Thiết lập một thư mục để lưu chỉ mục tìm kiếm.
      2. Chọn một thư mục chứa các tệp XLSX.
      3. Định nghĩa các tùy chọn tìm kiếm bổ sung.
      4. Thực hiện tìm kiếm và phân tích kết quả.
   
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
        // Đặt thư mục để lưu trữ chỉ mục tìm kiếm
        Index index = new Index("c:/MyIndex");

        // Xác định thư mục chứa các tài liệu có thể tìm kiếm
        index.add("c:/MyDocuments");

        // Kích hoạt tìm kiếm đồng âm để khớp các từ phát âm tương tự
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Thực thi một truy vấn tìm kiếm nâng cao
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khả năng tìm kiếm và lập chỉ mục nâng cao"
  description: "GroupDocs.Search for Java đơn giản hóa việc tìm kiếm văn bản và lập chỉ mục trên hơn 70 định dạng tài liệu, cung cấp các công cụ hiệu quả để quản lý và truy xuất thông tin một cách nhanh chóng."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Các Tính năng Chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản toàn diện"
      content: "Tìm văn bản trên nhiều định dạng tài liệu như PDF, tài liệu Word, bài thuyết trình PowerPoint và bảng tính. Sử dụng các kết quả chính xác, tìm kiếm không chính xác và toán tử đại diện cho các kết quả tìm kiếm tinh vi."

    # feature loop
    - title: "Tối ưu hóa lập chỉ mục cho dữ liệu lớn"
      content: "Tạo các chỉ mục có cấu trúc để tăng tốc độ tìm kiếm, giúp dễ dàng điều hướng qua các kho tài liệu rộng lớn một cách hiệu quả."

    # feature loop
    - title: "Hỗ trợ nhiều ngôn ngữ"
      content: "Thực hiện tìm kiếm bằng hơn 80 ngôn ngữ với hỗ trợ tích hợp cho các bố trí bàn phím khác nhau và sự biến thể hình thái từ, cải thiện độ chính xác."

    # feature loop
    - title: "Cài đặt tìm kiếm linh hoạt"
      content: "Tùy chỉnh tìm kiếm với các tùy chọn như độ nhạy chữ hoa chữ thường, lọc theo ngày và khả năng loại trừ các từ cụ thể để có kết quả chính xác."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Thực hiện các truy vấn tìm kiếm nâng cao"
      content: |
        Ví dụ này minh họa cách sử dụng các truy vấn tìm kiếm để tìm kiếm trong các tài liệu XLSX một cách hiệu quả.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Định nghĩa thư mục để lập chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Cung cấp đường dẫn tệp cho các tài liệu
          index.add("c:/MyDocuments");

          // Nhập mật khẩu cho các tài liệu được mã hóa
          index.getDictionaries().getDocumentPasswords().add("protected.xlsx", "123456");

          // Kích hoạt tìm kiếm không chính xác để phát hiện các từ tương tự
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Lấy kết quả tìm kiếm
          SearchResult result = index.Search("Loarem", options);
          
          // Xử lý và phân tích kết quả tìm kiếm
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    title: "Tổng quan về các tính năng chính"
    exclude: "document"
    description: "Khám phá các chức năng tìm kiếm văn bản hiệu suất cao được thiết kế cho hiệu quả và độ chính xác."
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
    title: "Tìm thông tin trên tài liệu XLSX với GroupDocs.Search"
    exclude: "XLSX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng, bao gồm các tệp văn phòng, cho phép tìm kiếm nhanh chóng với các tính năng lập chỉ mục nâng cao."
    items: 
        # format loop 1
        - name: "Tìm kiếm trong tài liệu DOCX"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm trong tài liệu PDF"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm trong tài liệu PPTX"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm trong tài liệu TXT"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm trong tài liệu XLSX"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---