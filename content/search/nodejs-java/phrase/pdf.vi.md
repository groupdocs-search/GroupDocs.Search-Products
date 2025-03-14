
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:54
draft: false
lang: vi
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Tìm kiếm cụm từ trong PDF sử dụng Node.js"
head_description: "GroupDocs.Search for Node.js via Java thêm chức năng tìm kiếm cụm từ mạnh mẽ cho các ứng dụng JavaScript nhằm nâng cao hiệu quả tìm kiếm tài liệu."

############################# Header ############################
title: "Tìm cụm từ trong tài liệu" 
description: "Nhanh chóng xác định các cụm từ cụ thể với GroupDocs.Search for Node.js via Java. Tích hợp khả năng tìm kiếm nhanh và chính xác vào các ứng dụng Node.js của bạn."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Tính năng của GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) là một thư viện hiệu suất cao cho việc lập chỉ mục và tìm kiếm văn bản trong các tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, tài liệu Word, bảng tính Excel, hình ảnh và tệp ZIP, đảm bảo kết quả tìm kiếm chính xác và nhanh chóng.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm cụm từ trong tài liệu PDF"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) giúp việc tìm kiếm cụm từ trong tài liệu PDF trở nên hiệu quả. Áp dụng các tùy chọn tìm kiếm khác nhau để tinh chỉnh kết quả trong các ứng dụng Node.js via Java.
      
      1. Thiết lập thư mục chỉ mục tìm kiếm.
      2. Định nghĩa thư mục chứa các tệp PDF.
      3. Cấu hình các tham số tìm kiếm.
      4. Lấy và xử lý kết quả tìm kiếm.
   
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

        // Chỉ định đường dẫn để lưu chỉ mục tìm kiếm
        const index = new searchLib.Index("c:/MyIndex");

        // Đặt thư mục chứa các tài liệu
        index.add("c:/MyDocuments");

        // Cấu hình cài đặt tìm kiếm
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Chạy truy vấn tìm kiếm
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khám phá công cụ tìm kiếm tài liệu Node.js"
  description: "GroupDocs.Search for Node.js via Java cho phép tìm kiếm cụm từ trên hơn 70 định dạng tệp, giúp bạn dễ dàng tìm và tổ chức dữ liệu với các tính năng tìm kiếm nâng cao."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Các khả năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm cụm từ"
      content: "Tìm các cụm từ chính xác trong các tài liệu kinh doanh như PDF, tệp Word, bài thuyết trình và bảng tính. Sử dụng ký tự đại diện và các tùy chọn tìm kiếm linh hoạt khi cụm từ đầy đủ không được biết."

    # feature loop
    - title: "Tối ưu hóa lập chỉ mục dữ liệu"
      content: "Tăng cường hiệu suất tìm kiếm bằng cách tạo lập chỉ mục có thể tái sử dụng. Lập chỉ mục có cấu trúc giúp tăng tốc độ tìm kiếm tài liệu và cải thiện độ chính xác."

    # feature loop
    - title: "Tương thích đa ngôn ngữ"
      content: "Tìm kiếm tài liệu bằng hơn 80 ngôn ngữ với hỗ trợ cho các bố cục bàn phím khác nhau và các biến thể từ hình thái, đảm bảo kết quả chính xác."

    # feature loop
    - title: "Tùy chọn tìm kiếm nâng cao"
      content: "Tùy chỉnh tìm kiếm với độ nhạy cảm với chữ cái, kết hợp mơ hồ, phát hiện đồng âm, lọc tài liệu, và nhiều tính năng mạnh mẽ khác."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử dụng các kỹ thuật tìm kiếm nâng cao"
      content: |
        Tìm hiểu cách xây dựng truy vấn để tìm kiếm trong PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Định nghĩa thư mục chỉ mục tìm kiếm
          const index = new searchLib.Index("c:/MyIndex");
              
          // Đặt đường dẫn đến các tài liệu mục tiêu
          index.add("c:/MyDocuments");

          // Tạo truy vấn cho cụm từ mong muốn
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Lấy kết quả tìm kiếm
          const result = index.search(query);
          
          // Xử lý và sử dụng kết quả
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Khả năng tìm kiếm nâng cao"
    exclude: "phrase"
    description: "Tận dụng các tính năng tìm kiếm mạnh mẽ để có kết quả nhanh hơn và chính xác hơn."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm cụm từ trong tài liệu kinh doanh"
    exclude: "PDF"
    description: "GroupDocs.Search hỗ trợ tìm kiếm cụm từ trong hơn 70 định dạng tài liệu. Sử dụng các tùy chọn nâng cao và lập chỉ mục để tối ưu hóa quy trình tìm kiếm."
    items: 
        # format loop 1
        - name: "Tìm kiếm cụm từ trong DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm cụm từ trong PDF"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm cụm từ trong PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm cụm từ trong TXT"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm cụm từ trong XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---