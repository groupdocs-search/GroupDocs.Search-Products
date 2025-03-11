
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: vi
format: Docx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Tìm kiếm DOCX trong .NET sử dụng các toán tử boolean"
head_description: "API GroupDocs.Search for .NET cho phép các lập trình viên C# tìm kiếm nội dung tài liệu bằng các toán tử boolean như AND, OR và NOT."

############################# Header ############################
title: "Tìm kiếm văn bản theo logic boolean" 
description: "GroupDocs.Search for .NET giúp tạo các truy vấn tìm kiếm nâng cao bằng cách sử dụng các toán tử boolean (AND, OR, NOT) trong ứng dụng .NET của bạn."
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
       [GroupDocs.Search for .NET](/search/net/) là một thư viện toàn diện cho việc tìm kiếm và lập chỉ mục văn bản trong các tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, chẳng hạn như PDF, Word, PowerPoint, Excel, hình ảnh và tệp ZIP, giúp xử lý hiệu quả lượng thông tin lớn.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm kiếm nội dung tài liệu DOCX sử dụng logic boolean"
    content: |
      [GroupDocs.Search](/search/net/) giúp việc tìm kiếm nội dung tài liệu DOCX trở nên đơn giản. Nó cung cấp các điều kiện tìm kiếm logic boolean để làm rõ kết quả trong các ứng dụng .NET.
      
      1. Chỉ định thư mục để lưu trữ chỉ mục tìm kiếm.
      2. Chọn thư mục chứa các tệp DOCX.
      3. Thực hiện tìm kiếm và nhận kết quả.
      4. Xử lý kết quả.
   
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

        // Chỉ định thư mục chứa tài liệu để tìm kiếm
        index.Add("c:/MyDocuments");

        // Thực hiện tìm kiếm sử dụng truy vấn phức tạp
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khám phá các tính năng nâng cao cho tìm kiếm và lập chỉ mục tài liệu"
  description: "Thư viện GroupDocs.Search for .NET đơn giản hóa việc tìm kiếm và lập chỉ mục văn bản cho hơn 70 định dạng tệp. Tìm kiếm và quản lý thông tin một cách dễ dàng với các công cụ tìm kiếm nâng cao."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Các tính năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm văn bản mạnh mẽ"
      content: "Tìm kiếm văn bản trong nhiều loại tệp khác nhau, bao gồm PDF, tài liệu Word, bài thuyết trình PowerPoint và bảng tính. Sử dụng các tính năng như khớp chính xác, tìm kiếm mờ và ký tự đại diện để tinh chỉnh kết quả."

    # feature loop
    - title: "Lập chỉ mục tập dữ liệu lớn"
      content: "Tạo và duy trì các chỉ mục để tìm kiếm nhanh hơn. Lập chỉ mục cấu trúc và tổ chức dữ liệu, giúp dễ dàng tìm kiếm các bộ sưu tập tài liệu rộng lớn."

    # feature loop
    - title: "Hỗ trợ nhiều ngôn ngữ"
      content: "Tìm kiếm tài liệu bằng hơn 80 ngôn ngữ, với hỗ trợ các kiểu bàn phím khác nhau và các hình thức từ ngữ hình thái để nâng cao độ chính xác trong tìm kiếm."

    # feature loop
    - title: "Tùy chọn tìm kiếm có thể tùy chỉnh"
      content: "Điều chỉnh cài đặt tìm kiếm với các tính năng như nhạy cảm với chữ hoa, bộ lọc theo khoảng thời gian, và khả năng loại trừ các từ hoặc dữ liệu cụ thể trong quá trình lập chỉ mục."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử dụng các truy vấn tìm kiếm boolean nâng cao"
      content: |
        Ví dụ này minh họa cách áp dụng các truy vấn boolean để tìm kiếm các tài liệu DOCX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Đặt thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Chỉ định đường dẫn đến các tài liệu cần tìm kiếm
          index.Add("c:/MyDocuments");

          // Tạo một truy vấn tìm kiếm sử dụng logic boolean
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Lấy các kết quả tìm kiếm
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.docx"
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
    exclude: "boolean"
    description: "Khám phá các chức năng tìm kiếm nâng cao và hiệu quả."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm trên các định dạng tài liệu phổ biến"
    exclude: "DOCX"
    description: "GroupDocs.Search hỗ trợ hơn 70 định dạng tệp. Tùy chỉnh quy tắc tìm kiếm và tận dụng lập chỉ mục để tiết kiệm thời gian và công sức."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Định dạng tài liệu di động Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Bản trình bày PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---