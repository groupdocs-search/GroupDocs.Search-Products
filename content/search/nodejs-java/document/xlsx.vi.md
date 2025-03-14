
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tìm kiếm văn bản trong XLSX với GroupDocs.Search trên Node.js"
head_description: "Sử dụng GroupDocs.Search for Node.js via Java với JavaScript để tìm kiếm văn bản một cách hiệu quả trong nhiều định dạng tài liệu khác nhau."

############################# Header ############################
title: "Giải pháp tìm kiếm tài liệu thông minh" 
description: "Xác định vị trí văn bản trong các định dạng tài liệu khác nhau bằng cách sử dụng GroupDocs.Search for Node.js via Java. Tạo các truy vấn tìm kiếm nâng cao trong các ứng dụng Node.js của bạn."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Thử nghiệm miễn phí"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Giới thiệu về GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) là một thư viện hiệu suất cao cho tìm kiếm toàn văn và lập chỉ mục tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, Word, PowerPoint, Excel, hình ảnh và các lưu trữ ZIP, đảm bảo kết quả nhanh chóng và chính xác.

############################# Steps ############################
steps:
    enable: true
    title: "Thực hiện tìm kiếm trong các tệp XLSX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) cho phép bạn thực hiện tìm kiếm trong các tệp XLSX, tinh chỉnh kết quả trong các ứng dụng Node.js via Java.
      
      1. Xác định một thư mục lưu trữ cho chỉ mục tìm kiếm.
      2. Chọn một thư mục chứa các tệp XLSX.
      3. Thiết lập thêm các tham số tìm kiếm.
      4. Chạy tìm kiếm và phân tích kết quả.
   
    code:
      platform: "nodejs-java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Kết quả tìm kiếm"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Xác định thư mục cho việc lưu trữ chỉ mục tìm kiếm
        const index = new searchLib.Index("c:/MyIndex");

        // Chọn thư mục chứa tài liệu để tìm kiếm
        index.add("c:/MyDocuments");

        // Bật tìm kiếm đồng âm cho các từ có âm giống nhau
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Thực hiện một truy vấn tìm kiếm phức tạp
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khả năng tìm kiếm và lập chỉ mục nâng cao"
  description: "GroupDocs.Search for Node.js via Java cung cấp các công cụ tìm kiếm văn bản và lập chỉ mục mạnh mẽ trên hơn 70 định dạng tài liệu, giúp bạn dễ dàng tìm kiếm và tổ chức thông tin."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Lợi ích chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản toàn diện"
      content: "Xác định vị trí văn bản trong nhiều loại tài liệu, bao gồm PDF, tài liệu Word, bài thuyết trình PowerPoint và bảng tính. Sử dụng các truy vấn chính xác, tìm kiếm mờ và ký tự đại diện để có kết quả tinh chỉnh."

    # feature loop
    - title: "Lập chỉ mục hiệu quả cho dữ liệu lớn"
      content: "Tăng tốc độ tìm kiếm bằng cách tạo các chỉ mục có cấu trúc, giúp dễ dàng truy xuất thông tin từ các tập tài liệu lớn."

    # feature loop
    - title: "Hỗ trợ hơn 80 ngôn ngữ"
      content: "Tìm kiếm trong các tài liệu bằng các ngôn ngữ khác nhau, với khả năng nhận dạng tự động các dạng từ và bố cục bàn phím khác nhau."

    # feature loop
    - title: "Cài đặt tìm kiếm tùy chỉnh"
      content: "Điều chỉnh các tùy chọn tìm kiếm như phân biệt chữ hoa chữ thường, bộ lọc ngày tháng và loại trừ từ để có được kết quả chính xác."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử dụng tìm kiếm cho các tài liệu XLSX"
      content: |
        Ví dụ này cho thấy cách sử dụng các truy vấn tìm kiếm trong các tài liệu XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Thiết lập thư mục cho việc lập chỉ mục tìm kiếm
          const index = new searchLib.Index("c:/MyIndex");
              
          // Cung cấp đường dẫn đến tệp để lưu trữ tài liệu
          index.add("c:/MyDocuments");

          // Nhập mật khẩu cho các tệp bảo vệ
          index.getDictionaries().getDocumentPasswords().add("protected.xlsx", '123456');

          // Bật tìm kiếm mờ để phát hiện từ tương tự
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Trích xuất kết quả tìm kiếm
          const result = index.search("Loarem", options);
          
          // Xử lý và xem xét các kết quả
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Sao chép"
        install:
          command: "npm i @groupdocs/groupdocs.search"
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
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Hãy thử các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Khám phá các tính năng chính"
    exclude: "document"
    description: "Khám phá những tính năng tìm kiếm tốc độ cao được thiết kế để nâng cao hiệu suất và độ chính xác."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm trong nhiều loại tài liệu"
    exclude: "XLSX"
    description: "GroupDocs.Search hoạt động với hơn 70 định dạng tệp, bao gồm tài liệu văn phòng, đảm bảo kết quả tìm kiếm nhanh chóng và chính xác với hỗ trợ lập chỉ mục."
    items: 
        # format loop 1
        - name: "Tìm kiếm trong tài liệu DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm trong tài liệu PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm trong tài liệu PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm trong tài liệu TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm trong tài liệu XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---