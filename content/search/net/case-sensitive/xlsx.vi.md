
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tìm kiếm phân biệt chữ hoa trong XLSX sử dụng .NET"
head_description: "API GroupDocs.Search for .NET cho phép các nhà phát triển C# thực hiện các tìm kiếm phân biệt chữ hoa trong nhiều tài liệu."

############################# Header ############################
title: "Tìm kiếm phân biệt chữ hoa" 
description: "GroupDocs.Search for .NET giúp tạo các truy vấn tìm kiếm phân biệt chữ hoa phức tạp trong ứng dụng .NET của bạn."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải Xuống Miễn Phí"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) là một thư viện mạnh mẽ cho việc tìm kiếm và lập chỉ mục văn bản trong các tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, Word, PowerPoint, Excel, hình ảnh và tệp ZIP, đảm bảo xử lý hiệu quả các khối lượng dữ liệu lớn.

############################# Steps ############################
steps:
    enable: true
    title: "Cách Thực Hiện Tìm Kiếm Phân Biệt Chữ Hoa trong Tài Liệu XLSX"
    content: |
      [GroupDocs.Search](/search/net/) đơn giản hóa tìm kiếm phân biệt chữ hoa trong các tài liệu XLSX. Sử dụng để tinh chỉnh kết quả trong các ứng dụng .NET.
      
      1. Xác định thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa tệp XLSX.
      3. Chạy tìm kiếm và lấy kết quả.
      4. Xử lý các kết quả.
   
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
        // Đặt đường dẫn đến thư mục chỉ mục
        Index index = new Index("c:/MyIndex");

        // Chỉ định thư mục chứa các tài liệu cần tìm
        index.Add("c:/MyDocuments");

        // Bật tìm kiếm phân biệt chữ hoa trong tùy chọn
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Chạy tìm kiếm
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Tính Năng Nâng Cao cho Tìm Kiếm và Lập Chỉ Mục Tài Liệu"
  description: "Thư viện GroupDocs.Search for .NET đơn giản hóa việc tìm kiếm văn bản và lập chỉ mục trên hơn 70 định dạng tệp. Tìm và quản lý thông tin một cách hiệu quả với các công cụ tìm kiếm mạnh mẽ."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Các Tính Năng Chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm Kiếm Văn Bản Nâng Cao"
      content: "Tìm kiếm văn bản trong nhiều định dạng tệp khác nhau, bao gồm PDF, tài liệu Word, bảng tính và bài thuyết trình. Sử dụng các tùy chọn như tìm kiếm chính xác, tìm kiếm không chính xác và ký tự đại diện để có kết quả chính xác."

    # feature loop
    - title: "Lập Chỉ Mục Tập Dữ Liệu Lớn"
      content: "Xây dựng và duy trì các chỉ mục để tìm kiếm nhanh hơn. Lập chỉ mục có tổ chức giúp tìm kiếm các bộ sưu tập tài liệu lớn một cách dễ dàng."

    # feature loop
    - title: "Hỗ Trợ Đa Ngôn Ngữ"
      content: "Tìm kiếm trong các tài liệu bằng hơn 80 ngôn ngữ, với hỗ trợ cho các bố trí bàn phím và hình thức từ khác nhau để có kết quả chính xác hơn."

    # feature loop
    - title: "Tùy Chỉnh Tùy Chọn Tìm Kiếm"
      content: "Tùy chỉnh cài đặt tìm kiếm với phân biệt chữ hoa, bộ lọc khoảng thời gian và khả năng loại trừ các từ hoặc dữ liệu cụ thể trong quá trình lập chỉ mục."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử Dụng Các Truy Vấn Tìm Kiếm Phân Biệt Chữ Hoa"
      content: |
        Ví dụ này cho thấy cách sử dụng các truy vấn phân biệt chữ hoa để tìm kiếm trong các tài liệu XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Đặt thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Xác định đường dẫn đến các tài liệu cần tìm
          index.Add("c:/MyDocuments");

          // Tạo một truy vấn tìm kiếm
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Bật các tùy chọn tìm kiếm phân biệt chữ hoa
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Tìm kiếm văn bản trong các tài liệu
          SearchResult result = index.Search(wordQuery, options);
          
          // Xử lý các kết quả tìm kiếm
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "Khám Phá Các Tính Năng Chính"
    exclude: "case-sensitive"
    description: "Khám phá các chức năng tìm kiếm tiên tiến và hiệu quả."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm Kiếm Các Định Dạng Tài Liệu Phổ Biến"
    exclude: "XLSX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp. Tùy chỉnh quy tắc tìm kiếm và sử dụng lập chỉ mục để tiết kiệm thời gian và công sức."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Bản trình bày PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---