---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: vi
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Thư viện Tìm kiếm và Lập chỉ mục tài liệu .NET cho PDF, Tệp Office và hơn thế nữa"
head_description: "Giải pháp mạnh mẽ .NET cho tìm kiếm văn bản và lập chỉ mục trong các tài liệu như PDF, Word, Excel, thuyết trình, email và các định dạng web."

############################# Header ############################
title: "Tìm kiếm và Lập chỉ mục tài liệu nâng cao với API .NET"
description: "Tăng cường ứng dụng .NET với khả năng tìm kiếm văn bản tiên tiến trên các định dạng tài liệu phổ biến."
words:
  for: "cho"

actions:
  main: "Tải Nuget miễn phí"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Bắt đầu Hành Trình của Bạn Ngày Hôm Nay!"
  description: "Khám phá các khả năng của GroupDocs.Search miễn phí hoặc bảo đảm một giấy phép để mở khóa toàn bộ tiềm năng của nó."

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"

code:
  title: "Tìm kiếm văn bản trong các tệp thư mục"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Tạo một chỉ mục cho tài liệu của bạn
    Index index = new Index("c:/MyIndex");

    // Thêm tài liệu vào chỉ mục để tìm kiếm hiệu quả
    index.Add("c:/MyDocuments");
    
    // Tìm kiếm từ hoặc cụm từ cụ thể, chẳng hạn như
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Search"
  description: "Khám phá thư viện .NET C# cho tìm kiếm văn bản và lập chỉ mục mạnh mẽ."
  features:
    # feature loop
    - title: "Tính năng Lập chỉ mục và Tìm kiếm của .NET"
      content: "Lập chỉ mục, lưu trữ và xử lý dữ liệu tài liệu hiệu quả với GroupDocs.Search for .NET cho các hoạt động tìm kiếm chính xác và nhanh chóng."

    # feature loop
    - title: "Kết hợp các chỉ mục để nâng cao tốc độ tìm kiếm"
      content: "GroupDocs.Search for .NET cho phép bạn hợp nhất nhiều chỉ mục để tối ưu hóa hiệu suất. Giảm ảnh hưởng của các chỉ mục delta bằng cách kết hợp chúng thành một chỉ mục tổng quát để tìm kiếm mượt mà hơn."

    # feature loop
    - title: "Tìm kiếm qua các bố cục bàn phím khác nhau"
      content: "Dễ dàng xử lý các truy vấn tìm kiếm qua 88 ngôn ngữ và 164 bố cục bàn phím với khả năng nhận diện thông minh của GroupDocs.Search for .NET."

    # feature loop
    - title: "Tìm kiếm từ ngữ hình thái"
      content: "GroupDocs.Search for .NET hỗ trợ tìm kiếm các biến thể từ như danh từ số ít/số nhiều và các dạng động từ khác nhau, có thể tùy chỉnh cho các ngôn ngữ khác nhau."

############################# Platforms ############################
platforms:
  enable: true
  title: "Khả năng độc lập của nền tảng"
  description: "GroupDocs.Search for .NET hoạt động liền mạch trên các hệ điều hành và trình quản lý gói lớn."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tệp được hỗ trợ"
  description: |
    Xử lý một loạt các định dạng tệp với GroupDocs.Search for .NET. [Xem tất cả các định dạng được hỗ trợ](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Các định dạng văn phòng phổ biến
        * **Portable:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Văn bản:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Các định dạng đa phương tiện
        * **Các định dạng hình ảnh phổ biến:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Hình ảnh nhiều trang:** GIF, WEBP, TIFF
        * **Âm thanh:** MP3, WAV
        * **Video:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Khác
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Khác:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Các tính năng chính của GroupDocs.Search for .NET"
  description: "Tối ưu hóa quản lý tài liệu với khả năng tìm kiếm nâng cao trong các định dạng phổ biến như PDF, DOCX, XLSX, PPTX, và hơn thế nữa."

  items:
    # feature loop
    - icon: "document_info"
      title: "Tham số tìm kiếm linh hoạt"
      content: "Sử dụng các bộ lọc như phạm vi ngày và tính nhạy cảm với chữ hoa để tinh chỉnh tìm kiếm của bạn."

    # feature loop
    - icon: "detect"
      title: "Kiểm tra chính tả thông minh"
      content: "Tìm kiếm cụm từ với sự sửa lỗi chính tả, kí hiệu thay thế và bỏ qua các ký tự đặc biệt."

    # feature loop
    - icon: "collect"
      title: "Kết quả tìm kiếm đã lọc"
      content: "Tùy chỉnh và lọc kết quả tìm kiếm theo loại tài liệu hoặc tiêu chí."

    # feature loop
    - icon: "get"
      title: "Nhập & Xuất chỉ mục"
      content: "Nhập dữ liệu, thay đổi cài đặt lập chỉ mục, và xuất các kết quả đã lập chỉ mục."

    # feature loop
    - icon: "remove"
      title: "Loại bỏ dữ liệu không liên quan"
      content: "Tối ưu hóa lập chỉ mục bằng cách bỏ qua các tệp hoặc từ cụ thể."

    # feature loop
    - icon: "style"
      title: "Trích xuất URL"
      content: "Chuyển đổi văn bản định dạng HTML thành các tệp và tạo liên kết cho kết quả tìm kiếm."

    # feature loop
    - icon: "detect"
      title: "Tìm kiếm tốc độ cao"
      content: "Chia nhỏ các chỉ mục lớn thành các phần nhỏ hơn để xử lý nhanh hơn."

    # feature loop
    - icon: "manipulate"
      title: "Xử lý dữ liệu mượt mà"
      content: "Lập chỉ mục các tài liệu trực tiếp từ các luồng và cấu trúc dữ liệu."

    # feature loop
    - icon: "compare"
      title: "Phát hiện lỗi chính tả"
      content: "Gợi ý các từ thay thế và theo dõi số lần xuất hiện để cải thiện độ chính xác."

    # feature loop
    - icon: "unreadable_characters"
      title: "Hỗ trợ lưu trữ"
      content: "Lập chỉ mục các tệp ZIP lồng vào nhau và truy xuất thông tin tệp bên trong chúng."

    # feature loop
    - icon: "hidden_print"
      title: "Lập chỉ mục hiệu quả"
      content: "Giảm không gian ổ đĩa với lập chỉ mục gọn nhẹ và xử lý các tài liệu được bảo vệ bằng mật khẩu."

    # feature loop
    - icon: "style"
      title: "Các từ đồng nghĩa tùy chỉnh"
      content: "Thêm và quản lý các từ đồng nghĩa để có kết quả tìm kiếm tùy chỉnh."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Khám phá khả năng mạnh mẽ của GroupDocs.Search for .NET với các ví dụ thực tế."
  items:
    # code sample loop
    - title: "Tăng năng suất với Tìm kiếm mờ"
      content: |
        Tận dụng GroupDocs.Search for .NET cho kiểm soát nội dung linh hoạt và chính xác thông qua các thuật toán tìm kiếm nâng cao. [Khám phá thêm](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Cách xử lý kết quả tìm kiếm">}}
        ```csharp {style=abap}
        // Tạo một chỉ mục
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Thiết lập tùy chọn tìm kiếm
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Tìm kiếm các tài liệu chứa từ 'nước' hoặc cụm từ 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Xử lý kết quả tìm kiếm
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tìm kiếm nâng cao với Biểu thức chính quy"
      content: |
        GroupDocs.Search for .NET hỗ trợ các biểu thức chính quy cho các tìm kiếm chính xác. [Tìm hiểu các kỹ thuật nâng cao](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Cách tìm kiếm bằng biểu thức chính quy">}}
        ```csharp {style=abap}   
        // Tạo một chỉ mục
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Tìm kiếm cụm từ ở dạng văn bản

        // Ký tự caret đầu tiên ở đầu chỉ ra rằng đây là truy vấn tìm kiếm bằng biểu thức chính quy
        string query = "^^(.)\\1{1,}";
        // Tìm kiếm hai hoặc nhiều ký tự giống nhau ở đầu một từ
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
