
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: vi
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tìm kiếm cụm từ trong PDF bằng .NET"
head_description: "GroupDocs.Search for .NET tăng cường các ứng dụng C# với khả năng tìm kiếm cụm từ mạnh mẽ cho nội dung tài liệu."

############################# Header ############################
title: "Tìm kiếm cụm từ trong tài liệu" 
description: "Tìm các cụm từ cụ thể một cách nhanh chóng với GroupDocs.Search for .NET. Tích hợp chức năng tìm kiếm hiệu quả vào các ứng dụng .NET của bạn."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Các tính năng của GroupDocs.Search"
    link: "/search/net/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) là một thư viện mạnh mẽ cho việc lập chỉ mục và tìm kiếm văn bản trong tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, tài liệu Word, bảng tính Excel, hình ảnh và tệp ZIP, cho phép kết quả tìm kiếm nhanh chóng và chính xác.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm kiếm cụm từ trong tài liệu PDF"
    content: |
      [GroupDocs.Search](/search/net/) đơn giản hóa việc tìm kiếm trong tài liệu PDF. Sử dụng các tùy chọn khác nhau để tinh chỉnh kết quả tìm kiếm trong các ứng dụng .NET.
      
      1. Cài đặt thư mục chỉ mục tìm kiếm.
      2. Xác định thư mục chứa các tệp PDF.
      3. Cấu hình các thiết lập tìm kiếm.
      4. Lấy và xử lý kết quả tìm kiếm.
   
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
        // Đường dẫn để lưu trữ chỉ mục tìm kiếm
        Index index = new Index("c:/MyIndex");

        // Thư mục chứa các tài liệu
        index.Add("c:/MyDocuments");

        // Cấu hình các tùy chọn tìm kiếm
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Thực hiện tìm kiếm
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khám phá công cụ tìm kiếm tài liệu .NET"
  description: "GroupDocs.Search for .NET cho phép tìm kiếm cụm từ trên 70+ định dạng tệp. Xác định và quản lý dữ liệu một cách hiệu quả với các khả năng tìm kiếm nâng cao."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm cụm từ"
      content: "Tìm kiếm các cụm từ chính xác trong tài liệu kinh doanh, bao gồm PDF, tệp Word, bài thuyết trình và bảng tính. Sử dụng ký tự đại diện và các tùy chọn khác nếu cụm từ chính xác không rõ ràng."

    # feature loop
    - title: "Lập chỉ mục dữ liệu hiệu quả"
      content: "Tạo và tái sử dụng các chỉ mục tìm kiếm để tăng tốc độ tìm kiếm tài liệu. Lập chỉ mục cấu trúc dữ liệu một cách hiệu quả, giúp tìm kiếm cụm từ nhanh hơn."

    # feature loop
    - title: "Hỗ trợ đa ngôn ngữ"
      content: "Tìm kiếm tài liệu bằng hơn 80 ngôn ngữ. Hỗ trợ các bố trí bàn phím khác nhau và các hình thức từ vựng hình thái cho độ chính xác trong tìm kiếm cao hơn."

    # feature loop
    - title: "Tùy chọn tìm kiếm linh hoạt"
      content: "Tùy chỉnh tìm kiếm với các tính năng như phân biệt chữ hoa chữ thường, tìm kiếm gần đúng và đồng âm, lọc tài liệu và nhiều hơn nữa."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử dụng kỹ thuật tìm kiếm nâng cao"
      content: |
        Tìm hiểu cách tạo các truy vấn để tìm kiếm trong PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Xác định thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Đặt đường dẫn đến các tài liệu để tìm kiếm
          index.Add("c:/MyDocuments");

          // Tạo một truy vấn cho một cụm từ cụ thể
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Lấy kết quả tìm kiếm
          SearchResult result = index.Search(query);
          
          // Xử lý và sử dụng kết quả
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Các tính năng nâng cao"
    exclude: "phrase"
    description: "Khám phá các chức năng tìm kiếm mạnh mẽ và hiệu quả."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm cụm từ trong tài liệu kinh doanh"
    exclude: "PDF"
    description: "GroupDocs.Search hỗ trợ tìm kiếm trong 70+ định dạng tài liệu. Sử dụng các tùy chọn tiên tiến và lập chỉ mục để tối ưu hóa quy trình tìm kiếm của bạn."
    items: 
        # format loop 1
        - name: "Tìm kiếm cụm từ trong DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm cụm từ trong PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm cụm từ trong PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm cụm từ trong TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm cụm từ trong XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---