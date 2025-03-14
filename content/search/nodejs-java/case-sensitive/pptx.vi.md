
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: vi
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Thực hiện tìm kiếm phân biệt chữ hoa chữ thường trong PPTX với Node.js"
head_description: "API GroupDocs.Search for Node.js via Java cho phép các nhà phát triển JavaScript thực hiện tìm kiếm phân biệt chữ hoa chữ thường trên các loại tài liệu khác nhau."

############################# Header ############################
title: "Tìm kiếm phân biệt chữ hoa chữ thường" 
description: "GroupDocs.Search for Node.js via Java cho phép bạn triển khai chức năng tìm kiếm phân biệt chữ hoa chữ thường nâng cao trong các ứng dụng Node.js của bạn."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) là một thư viện mạnh mẽ để tìm kiếm và lập chỉ mục văn bản trong các tài liệu. Nó hỗ trợ hơn 70 định dạng, bao gồm PDF, Word, Excel, PowerPoint, hình ảnh và tệp ZIP, cho phép xử lý hiệu quả một lượng lớn dữ liệu.

############################# Steps ############################
steps:
    enable: true
    title: "Các bước để thực hiện tìm kiếm phân biệt chữ hoa chữ thường trong các tệp PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) giúp bạn thực hiện tìm kiếm phân biệt chữ hoa chữ thường trong các tệp PPTX, nâng cao quy trình làm việc Node.js via Java của bạn.
      
      1. Thiết lập một thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tệp PPTX.
      3. Chạy tìm kiếm và nhận kết quả.
      4. Xử lý và sử dụng kết quả.
   
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

        // Xác định đường dẫn cho thư mục chỉ mục
        const index = new searchLib.Index("c:/MyIndex");

        // Đặt thư mục chứa các tài liệu cần tìm
        index.add("c:/MyDocuments");

        // Kích hoạt tìm kiếm phân biệt chữ hoa chữ thường trong cài đặt
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Thực hiện tìm kiếm
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tính năng chính cho Tìm kiếm và Lập chỉ mục Tài liệu"
  description: "Với GroupDocs.Search for Node.js via Java, bạn có thể tìm kiếm và lập chỉ mục văn bản trong hơn 70 định dạng tệp. Truy cập và tổ chức thông tin một cách hiệu quả bằng các công cụ tìm kiếm nâng cao."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Các Tính năng Chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm Văn bản Toàn diện"
      content: "Tìm kiếm văn bản trong nhiều loại tài liệu như PDF, tệp Word, bảng tính và bài thuyết trình. Sử dụng các tùy chọn như tìm kiếm chính xác, tìm kiếm mờ và ký tự đại diện để có kết quả chính xác."

    # feature loop
    - title: "Lập chỉ mục Dữ liệu Hiệu quả"
      content: "Tạo và quản lý các chỉ mục để tăng tốc độ tìm kiếm. Lập chỉ mục giúp bạn tổ chức và nhanh chóng xác định dữ liệu trong các bộ sưu tập tài liệu lớn."

    # feature loop
    - title: "Hỗ trợ Nhiều Ngôn ngữ"
      content: "Tìm kiếm các tài liệu bằng hơn 80 ngôn ngữ với hỗ trợ cho các bố cục bàn phím và biến thể từ vựng đa dạng, đảm bảo kết quả tìm kiếm chính xác."

    # feature loop
    - title: "Cài đặt Tìm kiếm Tùy chỉnh"
      content: "Điều chỉnh cài đặt tìm kiếm, bao gồm phân biệt chữ hoa chữ thường, bộ lọc theo ngày, và loại trừ các thuật ngữ hoặc dữ liệu nhất định trong quá trình lập chỉ mục."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ví dụ: Triển khai Tìm kiếm Phân biệt Chữ hoa Chữ thường"
      content: |
        Ví dụ này trình bày cách thực hiện tìm kiếm phân biệt chữ hoa chữ thường cho các tài liệu PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Định nghĩa thư mục cho chỉ mục tìm kiếm
          const index = new searchLib.Index("c:/MyIndex");
              
          // Cung cấp đường dẫn đến thư mục tài liệu
          index.add("c:/MyDocuments");

          // Thiết lập một truy vấn tìm kiếm
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Kích hoạt cài đặt tìm kiếm phân biệt chữ hoa chữ thường
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Tìm kiếm văn bản trong các tài liệu
          const result = index.search(wordQuery, options);
          
          // Xử lý và xử lý kết quả
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
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    title: "Chức năng Chính"
    exclude: "case-sensitive"
    description: "Khám phá các tính năng nâng cao cho việc tìm kiếm tài liệu nhanh chóng và chính xác."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Định dạng Tài liệu Tương thích"
    exclude: "PPTX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tài liệu. Tùy chỉnh các tùy chọn tìm kiếm của bạn và tiết kiệm thời gian với việc lập chỉ mục."
    items: 
        # format loop 1
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường trong XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---