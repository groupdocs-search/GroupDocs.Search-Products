
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: vi
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tìm kiếm trong tài liệu XLSX sử dụng .NET"
head_description: "GroupDocs.Search for .NET nâng cao các ứng dụng C# với khả năng tìm kiếm văn bản hiệu quả qua nhiều định dạng tài liệu kinh doanh khác nhau."

############################# Header ############################
title: "Tìm kiếm văn bản trong tài liệu kinh doanh" 
description: "GroupDocs.Search for .NET cho phép tìm kiếm văn bản mạnh mẽ và linh hoạt trong tài liệu của bạn. Tích hợp chức năng tìm kiếm vào các ứng dụng .NET một cách dễ dàng."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải xuống miễn phí"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search là gì?"
    link: "/search/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) là một thư viện mạnh mẽ cho việc tìm kiếm văn bản hiệu quả và lập chỉ mục tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm các tài liệu tiêu chuẩn ngành như PDF, Word, Excel, và PowerPoint. Cải thiện hiệu suất tìm kiếm với kết quả nhanh chóng và chính xác.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm kiếm trong dữ liệu XLSX"
    content: |
      [GroupDocs.Search](/search/net/) cho phép tìm kiếm văn bản hiệu quả trong tài liệu XLSX, lý tưởng cho các ứng dụng .NET.
      
      1. Thiết lập thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tệp của bạn.
      3. Cấu hình các tùy chọn tìm kiếm để chỉ xử lý các tài liệu XLSX.
      4. Thực hiện tìm kiếm và lấy kết quả.
   
    code:
      platform: "net"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Kết quả tìm kiếm"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "nhấn để sao chép"
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
        // Đường dẫn lưu trữ chỉ mục tìm kiếm tái sử dụng
        Index index = new Index("c:/MyIndex");

        // Thư mục chứa tài liệu
        index.Add("c:/MyDocuments");

        // Tìm kiếm chỉ trong các định dạng tệp cụ thể
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".xlsx");

        // Lấy kết quả tìm kiếm
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Các tính năng tìm kiếm nâng cao"
  description: "GroupDocs.Search for .NET cho phép tìm kiếm văn bản tinh vi qua hơn 70 định dạng tệp. Việc lập chỉ mục cải thiện hiệu quả tìm kiếm và giúp quản lý nội dung tài liệu một cách hiệu quả."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản nâng cao"
      content: "Trích xuất văn bản liên quan từ tài liệu kinh doanh phổ biến, bao gồm PDF, tệp Word, bài thuyết trình và bảng tính. Hỗ trợ nhiều kỹ thuật tìm kiếm như tìm kiếm mờ, phát hiện đồng âm và ký tự đại diện."

    # feature loop
    - title: "Lập chỉ mục tối ưu cho tìm kiếm nhanh hơn"
      content: "Xây dựng và tái sử dụng các chỉ mục tìm kiếm để tăng tốc độ tìm kiếm. Lập chỉ mục tối ưu hóa hiệu suất khi tìm kiếm qua các bộ sưu tập tài liệu lớn."

    # feature loop
    - title: "Hỗ trợ nhiều ngôn ngữ"
      content: "Thực hiện tìm kiếm trong các tài liệu viết bằng hơn 80 ngôn ngữ. Phát hiện các kiểu bàn phím khác nhau và biến thể từ ngữ để cải thiện độ chính xác."

    # feature loop
    - title: "Cài đặt tìm kiếm linh hoạt"
      content: "Tinh chỉnh kết quả tìm kiếm với các tùy chọn tùy chỉnh, bao gồm bộ lọc, biểu thức chính quy và cài đặt nhạy cảm với chữ hoa chữ thường."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Lọc tài liệu cần được xử lý"
      content: |
        Tìm hiểu cách thu hẹp tìm kiếm tài liệu bằng cách sử dụng bộ lọc
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Thiết lập một chỉ mục mà không bao gồm một số định dạng tệp nhất định
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Chỉ định thư mục tài liệu
          index.Add("c:/MyDocuments");

          // Lấy kết quả tìm kiếm
          SearchResult result = index.Search("Lorem");
          
          // Xử lý và sử dụng kết quả tìm kiếm
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Sao chép"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/search/formats/searchfilters.xlsx"
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
  description: "Hãy thử các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
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
    title: "Các tính năng chính"
    exclude: "filters"
    description: "Thực hiện tìm kiếm dữ liệu chính xác và hiệu quả."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm dữ liệu trong tài liệu kinh doanh của bạn"
    exclude: "XLSX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp, cho phép xử lý và tìm kiếm hiệu quả các tài liệu văn phòng phổ biến."
    items: 
        # format loop 1
        - name: "Bộ lọc tìm kiếm cho DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Bộ lọc tìm kiếm cho PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Bộ lọc tìm kiếm cho PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Bộ lọc tìm kiếm cho TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Bộ lọc tìm kiếm cho XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---