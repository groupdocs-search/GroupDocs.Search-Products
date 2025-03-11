
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:31
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tìm kiếm boolean XLSX qua Node.js"
head_description: "Sử dụng API GroupDocs.Search for Node.js via Java để thực hiện các tìm kiếm nâng cao trong nội dung tài liệu với các toán tử boolean như AND, OR và NOT, phù hợp cho các nhà phát triển JavaScript."

############################# Header ############################
title: "Thực hiện tìm kiếm logic boolean" 
description: "Với GroupDocs.Search for Node.js via Java, bạn có thể tạo các truy vấn tìm kiếm nâng cao bằng cách sử dụng các toán tử boolean (AND, OR, NOT) một cách liền mạch trong môi trường Node.js của bạn."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải Ngay"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) là một công cụ mạnh mẽ để tìm kiếm và lập chỉ mục văn bản trong các tài liệu. Nó hỗ trợ hơn 70 định dạng như PDF, Word, Excel, PowerPoint, hình ảnh và tệp ZIP, giúp xử lý lượng thông tin lớn một cách hiệu quả.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm kiếm trong các tài liệu XLSX sử dụng các toán tử boolean"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) cho phép bạn tìm kiếm nội dung trong các tệp XLSX một cách hiệu quả. Với logic boolean, bạn có thể tinh chỉnh các truy vấn tìm kiếm của mình trong các ứng dụng Node.js via Java để nâng cao độ chính xác.
      
      1. Thiết lập thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tệp XLSX để tìm kiếm.
      3. Chạy truy vấn tìm kiếm và lấy kết quả.
      4. Xử lý và phân tích kết quả tìm kiếm.
   
    code:
      platform: "nodejs-java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "nhấp để sao chép"
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

        // Đặt vị trí cho thư mục chỉ mục
        const index = new searchLib.Index("c:/MyIndex");

        // Xác định thư mục chứa các tài liệu để tìm kiếm
        index.add("c:/MyDocuments");

        // Thực hiện truy vấn tìm kiếm với logic nâng cao
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Công cụ mạnh mẽ cho việc tìm kiếm và lập chỉ mục tài liệu"
  description: "GroupDocs.Search for Node.js via Java đơn giản hóa việc tìm kiếm và lập chỉ mục văn bản cho hơn 70 loại tệp, giúp bạn tìm và quản lý thông tin nhanh chóng và chính xác."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản nâng cao"
      content: "Tìm văn bản nhanh chóng qua nhiều định dạng như PDF, tài liệu Word, thuyết trình và bảng tính. Sử dụng các tính năng như tìm kiếm chính xác, tìm kiếm wildcard và tìm kiếm mờ để đạt kết quả chính xác."

    # feature loop
    - title: "Lập chỉ mục dữ liệu hiệu quả"
      content: "Xây dựng và quản lý các chỉ mục để tăng tốc độ tìm kiếm trong các bộ sưu tập tài liệu lớn. Lập chỉ mục đảm bảo truy cập nhanh chóng và có cấu trúc vào dữ liệu của bạn."

    # feature loop
    - title: "Hỗ trợ đa ngôn ngữ"
      content: "Tìm kiếm trong các tài liệu viết bằng hơn 80 ngôn ngữ. Hỗ trợ hình thái và khả năng tương thích với bố cục bàn phím nâng cao kết quả tìm kiếm trong các ngôn ngữ khác nhau."

    # feature loop
    - title: "Cài đặt tìm kiếm linh hoạt"
      content: "Tùy chỉnh tìm kiếm của bạn bằng cách kích hoạt độ nhạy chữ hoa chữ thường, áp dụng bộ lọc ngày, hoặc bỏ qua các từ và dữ liệu cụ thể trong quá trình lập chỉ mục."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ví dụ về tìm kiếm boolean nâng cao"
      content: |
        Ví dụ này minh họa cách tạo các truy vấn dựa trên Boolean để tìm kiếm nội dung trong các tài liệu XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Định nghĩa thư mục cho chỉ mục tìm kiếm
          const index = new searchLib.Index("c:/MyIndex");
              
          // Cung cấp vị trí của các tài liệu để tìm kiếm
          index.add("c:/MyDocuments");

          // Xây dựng truy vấn sử dụng các toán tử boolean
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Lấy kết quả tìm kiếm
          const result = index.search(booleanQuery);
          
          // Xử lý và sử dụng kết quả tìm kiếm
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Sao chép"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.xlsx"
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
  description: "Thử nghiệm các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
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
    title: "Các khả năng chính của GroupDocs.Search"
    exclude: "boolean"
    description: "Khám phá các tính năng tìm kiếm nâng cao, hiệu quả và tùy chỉnh."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm các định dạng tài liệu phổ biến"
    exclude: "XLSX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp, cung cấp các quy tắc tìm kiếm linh hoạt và lập chỉ mục hiệu quả để tiết kiệm thời gian và công sức."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Bản trình bày PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---