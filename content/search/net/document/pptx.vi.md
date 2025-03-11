
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: vi
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tìm kiếm tài liệu PPTX trong .NET với GroupDocs.Search"
head_description: "Sử dụng GroupDocs.Search for .NET để thực hiện các tìm kiếm văn bản hiệu quả trong nhiều định dạng tài liệu khác nhau với C#."

############################# Header ############################
title: "Tìm kiếm văn bản tài liệu nâng cao" 
description: "GroupDocs.Search for .NET đơn giản hóa việc tìm kiếm văn bản trong các định dạng tài liệu phổ biến, cho phép bạn tạo các truy vấn tìm kiếm mạnh mẽ trong các ứng dụng .NET của bạn."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về miễn phí"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) là một thư viện mạnh mẽ được thiết kế cho việc tìm kiếm và lập chỉ mục toàn văn trong các tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, Word, PowerPoint, Excel, hình ảnh và tệp ZIP, đảm bảo kết quả tìm kiếm nhanh chóng và chính xác.

############################# Steps ############################
steps:
    enable: true
    title: "Cách thực hiện tìm kiếm văn bản trong tài liệu PPTX"
    content: |
      [GroupDocs.Search](/search/net/) cho phép thực hiện các thao tác tìm kiếm nội dung nâng cao trong các tài liệu PPTX, cho kết quả tìm kiếm tinh chỉnh trong các ứng dụng .NET.
      
      1. Thiết lập thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tệp PPTX.
      3. Cấu hình các tùy chọn tìm kiếm bổ sung.
      4. Chạy tìm kiếm và xem xét các kết quả.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "nhấp để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Định nghĩa đường dẫn cho chỉ mục tìm kiếm
        Index index = new Index("c:/MyIndex");

        // Chọn thư mục chứa các tài liệu cần tìm kiếm
        index.Add("c:/MyDocuments");

        // Kích hoạt tìm kiếm đồng âm để tìm các từ phát âm giống nhau
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Thực hiện một truy vấn tìm kiếm phức tạp
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Các tính năng tìm kiếm và lập chỉ mục nâng cao"
  description: "GroupDocs.Search for .NET nâng cao việc tìm kiếm văn bản và lập chỉ mục trên hơn 70 định dạng tệp, cung cấp các công cụ hiệu quả để xác định và quản lý thông tin."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản mạnh mẽ"
      content: "Tìm kiếm văn bản trên nhiều loại tài liệu khác nhau, bao gồm PDF, tài liệu Word, bài thuyết trình PowerPoint và bảng tính. Sử dụng các tính năng như khớp chính xác, tìm kiếm mờ, và ký tự đại diện để tinh chỉnh kết quả của bạn."

    # feature loop
    - title: "Lập chỉ mục nhanh cho các tập dữ liệu lớn"
      content: "Tạo và quản lý các chỉ mục tìm kiếm để truy xuất thông tin nhanh chóng. Việc lập chỉ mục tối ưu hóa tìm kiếm trên các bộ sưu tập tài liệu rộng lớn."

    # feature loop
    - title: "Hỗ trợ đa ngôn ngữ"
      content: "Thực hiện tìm kiếm bằng hơn 80 ngôn ngữ, với hỗ trợ cho các bố cục bàn phím khác nhau và các biến thể từ để cải thiện độ chính xác."

    # feature loop
    - title: "Cài đặt tìm kiếm tùy chỉnh"
      content: "Tinh chỉnh các tham số tìm kiếm với các tùy chọn như phân biệt chữ hoa chữ thường, bộ lọc khoảng thời gian, và loại trừ từ để có kết quả tốt hơn."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Thực hiện các truy vấn tìm kiếm nâng cao"
      content: |
        Ví dụ này minh họa cách áp dụng các truy vấn tìm kiếm cho các tài liệu PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Định nghĩa thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Chỉ định đường dẫn đến các tệp tài liệu
          index.Add("c:/MyDocuments");

          // Cung cấp mật khẩu cho các tài liệu được bảo vệ
          index.Dictionaries.DocumentPasswords.Add("protected.pptx", "123456");

          // Kích hoạt tìm kiếm mờ để tìm các từ tương tự
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Lấy kết quả tìm kiếm
          SearchResult result = index.Search("Loarem", options);
          
          // Xử lý kết quả tìm kiếm
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Sao chép"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "nhấp để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pptx"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Thử nghiệm các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Khám phá các tính năng chính"
    exclude: "document"
    description: "Tận dụng các chức năng tìm kiếm nâng cao và hiệu suất cao."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm trên các tài liệu doanh nghiệp của bạn"
    exclude: "PPTX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp, bao gồm các tài liệu văn phòng, cho phép tìm kiếm nhanh chóng và hiệu quả với khả năng lập chỉ mục."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Bản trình bày PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---