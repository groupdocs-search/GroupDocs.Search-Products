
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: vi
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tìm kiếm trong tài liệu PDF bằng Node.js"
head_description: "GroupDocs.Search for Node.js via Java bổ sung khả năng tìm kiếm văn bản nhanh chóng và chính xác cho các ứng dụng JavaScript, hỗ trợ nhiều định dạng tài liệu."

############################# Header ############################
title: "Tìm văn bản trong tài liệu kinh doanh" 
description: "GroupDocs.Search for Node.js via Java cung cấp chức năng tìm kiếm mạnh mẽ và linh hoạt cho tài liệu. Tích hợp tìm kiếm văn bản vào các ứng dụng Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) là một thư viện tìm kiếm và lập chỉ mục mạnh mẽ giúp truy xuất văn bản nhanh chóng trong tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, Word, Excel và PowerPoint, đảm bảo tìm kiếm chính xác và hiệu quả.

############################# Steps ############################
steps:
    enable: true
    title: "Cách thực hiện tìm kiếm trong tài liệu PDF"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) giúp việc tìm kiếm văn bản trong các tài liệu PDF trở nên hiệu quả cho các ứng dụng Node.js via Java.
      
      1. Tạo một thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tài liệu.
      3. Thiết lập tùy chọn tìm kiếm để chỉ bao gồm các tệp PDF.
      4. Chạy tìm kiếm và truy xuất các kết quả.
   
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

        // Định nghĩa thư mục để lưu trữ chỉ mục tìm kiếm
        const index = new searchLib.Index("c:/MyIndex");

        // Chỉ định thư mục chứa tài liệu có thể tìm kiếm
        index.add("c:/MyDocuments");

        // Giới hạn tìm kiếm cho các định dạng tệp cụ thể
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".pdf");

        // Truy xuất và xử lý kết quả tìm kiếm
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Nâng cao khả năng tìm kiếm"
  description: "GroupDocs.Search for Node.js via Java nâng cao hiệu quả tìm kiếm tài liệu bằng cách lập chỉ mục hơn 70 định dạng tệp. Tối ưu hóa việc truy xuất nội dung với các kỹ thuật tìm kiếm tiên tiến."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản toàn diện"
      content: "Trích xuất và định vị văn bản trong các định dạng tài liệu phổ biến, chẳng hạn như PDF, tệp Word, bảng tính và bài thuyết trình. Hỗ trợ tìm kiếm mờ, từ đồng âm và truy vấn ký tự đại diện."

    # feature loop
    - title: "Lập chỉ mục tối ưu cho hiệu suất"
      content: "Thúc đẩy tốc độ tìm kiếm bằng cách tạo các chỉ mục có thể tái sử dụng. Tăng cường tốc độ và hiệu quả khi làm việc với các bộ tài liệu lớn."

    # feature loop
    - title: "Hỗ trợ đa ngôn ngữ"
      content: "Tìm kiếm qua tài liệu trong hơn 80 ngôn ngữ. Nhận diện bố cục bàn phím và biến thể từ ngữ để đạt độ chính xác cao hơn."

    # feature loop
    - title: "Tùy chọn tìm kiếm có thể tùy chỉnh"
      content: "Tinh chỉnh kết quả tìm kiếm bằng cách sử dụng bộ lọc, biểu thức chính quy, độ nhạy chữ hoa và các cài đặt linh hoạt khác."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Lọc các tài liệu có thể tìm kiếm"
      content: |
        Tìm hiểu cách tinh chỉnh việc tìm kiếm tài liệu bằng cách sử dụng bộ lọc.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Cấu hình một chỉ mục để loại trừ các định dạng tệp không mong muốn
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Chỉ định thư mục chứa tài liệu
          index.add("c:/MyDocuments");

          // Xử lý kết quả tìm kiếm để sử dụng cho các mục đích khác
          const result = index.Search("Lorem", options);
          
          // Xử lý kết quả tìm kiếm để sử dụng cho các mục đích khác
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
            link: "/examples/search/formats/searchfilters.pdf"
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
    title: "Chức năng chính"
    exclude: "filters"
    description: "Thực hiện tìm kiếm văn bản nhanh chóng và chính xác trên các tài liệu."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm trong nhiều định dạng tài liệu"
    exclude: "PDF"
    description: "GroupDocs.Search hỗ trợ hơn 70 loại tệp, cho phép tìm kiếm văn bản hiệu quả trên nhiều tài liệu văn phòng và kinh doanh."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Bản trình bày PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---