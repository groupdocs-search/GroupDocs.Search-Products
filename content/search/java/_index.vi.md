---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: vi
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Giải pháp Tìm kiếm & Lập chỉ mục tài liệu Java cho PDF, Tệp Office và Nội dung Web"
head_description: "Giải pháp tìm kiếm văn bản và lập chỉ mục mạnh mẽ cho các ứng dụng Java. Tìm kiếm và tổ chức dữ liệu trong PDF, Word, Excel, thuyết trình, email và các định dạng web một cách dễ dàng."

############################# Header ############################
title: "Tìm kiếm và Lập chỉ mục tài liệu hiệu quả với API Java"
description: "Tăng cường các ứng dụng Java với các tính năng tìm kiếm văn bản mạnh mẽ trên tất cả các định dạng tài liệu phổ biến."
words:
  for: "cho"

actions:
  main: "Tải Maven miễn phí"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Bắt đầu Hành Trình của Bạn Ngày Hôm Nay!"
  description: "Khám phá các khả năng của GroupDocs.Search miễn phí hoặc bảo đảm một giấy phép để mở khóa toàn bộ tiềm năng của nó."

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"

code:
  title: "Tìm văn bản trong các tệp sử dụng Java"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Tạo một chỉ mục cho tài liệu của bạn
    Index index = new Index("c:/MyIndex");

    // Thêm tài liệu vào chỉ mục để tìm kiếm hiệu quả
    index.add("c:/MyDocuments");
    
    // Tìm kiếm từ hoặc cụm từ cụ thể, chẳng hạn như
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Search"
  description: "Khám phá khả năng tìm kiếm văn bản mạnh mẽ của thư viện Java Java."
  features:
    # feature loop
    - title: "Tính năng Lập chỉ mục và Tìm kiếm trong Java"
      content: "Với GroupDocs.Search for Java, bạn có thể thu thập, lưu trữ và phân tích dữ liệu hiệu quả để tạo các chỉ mục chi tiết cho các tìm kiếm nhanh hơn, chính xác hơn."

    # feature loop
    - title: "Tối ưu hóa tìm kiếm bằng cách kết hợp các chỉ mục"
      content: "Dễ dàng kết hợp nhiều chỉ mục với GroupDocs.Search for Java để tối ưu hóa việc tìm kiếm. Giảm ảnh hưởng của các chỉ mục delta nhỏ hơn bằng cách hợp nhất chúng thành một chỉ mục hiệu suất cao."

    # feature loop
    - title: "Hỗ trợ cho các bố cục bàn phím đa ngôn ngữ"
      content: "Tìm kiếm qua các ngôn ngữ và bố cục bàn phím khác nhau với GroupDocs.Search for Java. Nó hỗ trợ 88 ngôn ngữ và 164 cấu hình bàn phím cho tính linh hoạt vượt trội."

    # feature loop
    - title: "Khả năng tìm kiếm dạng hình thái"
      content: "Tìm các dạng từ khác nhau như danh từ số ít/số nhiều hoặc biến thể động từ bằng cách sử dụng GroupDocs.Search for Java. Tùy chỉnh các tùy chọn tìm kiếm cho tiếng Anh và các ngôn ngữ khác."

############################# Platforms ############################
platforms:
  enable: true
  title: "Khả năng độc lập của nền tảng"
  description: "GroupDocs.Search for Java tương thích với các hệ điều hành chính và trình quản lý gói."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tệp được hỗ trợ"
  description: |
    Làm việc với một loạt các định dạng tệp bằng GroupDocs.Search for Java. [Xem danh sách đầy đủ](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Các tính năng của GroupDocs.Search for Java"
  description: "Quản lý nội dung tài liệu một cách hiệu quả với các khả năng tìm kiếm nâng cao hỗ trợ các định dạng như PDF, DOCX, XLSX, PPTX, và nhiều hơn nữa."

  items:
    # feature loop
    - icon: "document_info"
      title: "Tham số tìm kiếm có thể tùy chỉnh"
      content: "Tinh chỉnh tìm kiếm bằng cách sử dụng bộ lọc phạm vi ngày và tính nhạy cảm với chữ hoa."

    # feature loop
    - icon: "detect"
      title: "Kiểm tra chính tả nâng cao"
      content: "Tìm kiếm hiệu quả với kiểm tra chính tả, các ký hiệu thay thế, và bỏ qua các ký tự đặc biệt."

    # feature loop
    - icon: "collect"
      title: "Kết quả tìm kiếm đã lọc"
      content: "Áp dụng bộ lọc để tập trung vào kết quả tìm kiếm dựa trên các loại tài liệu hoặc tiêu chí cụ thể."

    # feature loop
    - icon: "get"
      title: "Nhập và Xuất dữ liệu chỉ mục"
      content: "Dễ dàng nhập dữ liệu để lập chỉ mục hoặc xuất các kết quả vào tệp để sử dụng sau."

    # feature loop
    - icon: "remove"
      title: "Bỏ qua các tệp không cần thiết"
      content: "Tối ưu hóa lập chỉ mục bằng cách loại trừ các tệp hoặc từ cụ thể."

    # feature loop
    - icon: "style"
      title: "Xử lý HTML và URL"
      content: "Trích xuất nội dung HTML thành các tệp và tạo liên kết để điều hướng qua các kết quả tìm kiếm."

    # feature loop
    - icon: "detect"
      title: "Tìm kiếm nhanh trong các chỉ mục lớn"
      content: "Tăng tốc các hoạt động tìm kiếm bằng cách chia nhỏ các chỉ mục lớn thành các phần có thể quản lý."

    # feature loop
    - icon: "manipulate"
      title: "Lập chỉ mục từ dòng"
      content: "Lập chỉ mục trực tiếp dữ liệu từ các dòng hoặc cấu trúc dữ liệu."

    # feature loop
    - icon: "compare"
      title: "Xử lý các truy vấn viết sai"
      content: "Phát hiện lỗi chính tả và gợi ý các từ thay thế để cải thiện độ chính xác trong tìm kiếm."

    # feature loop
    - icon: "unreadable_characters"
      title: "Hỗ trợ lưu trữ toàn diện"
      content: "Lập chỉ mục các lưu trữ lồng vào trong và truy xuất danh sách chi tiết các tệp bên trong các tệp ZIP."

    # feature loop
    - icon: "hidden_print"
      title: "Lập chỉ mục tiết kiệm không gian"
      content: "Lập chỉ mục gọn gàng để tiết kiệm không gian ổ đĩa và xử lý các tệp được bảo vệ bằng mật khẩu."

    # feature loop
    - icon: "style"
      title: "Hỗ trợ từ đồng nghĩa tùy chỉnh"
      content: "Mở rộng từ điển đồng nghĩa để nâng cao độ chính xác trong tìm kiếm với các tùy chọn được tùy chỉnh."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Thử nghiệm các tính năng của GroupDocs.Search for Java với những ví dụ mã này."
  items:
    # code sample loop
    - title: "Tăng độ chính xác tìm kiếm với Tìm kiếm Mờ"
      content: |
        Khám phá tính linh hoạt của GroupDocs.Search for Java để quản lý nội dung với khả năng tìm kiếm mờ nâng cao. [Tìm hiểu thêm](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Cách xử lý kết quả tìm kiếm">}}
        ```java {style=abap}
        // Tạo một chỉ mục
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Thiết lập tùy chọn tìm kiếm
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Tìm kiếm các tài liệu chứa từ 'nước' hoặc cụm từ 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Xử lý kết quả tìm kiếm
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Tinh chỉnh kết quả với Biểu thức chính quy"
      content: |
        Sử dụng biểu thức chính quy trong GroupDocs.Search for Java để tạo kết quả tìm kiếm chính xác và chi tiết. [Khám phá các kỹ thuật nâng cao](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Cách tìm kiếm bằng biểu thức chính quy">}}
        ```java {style=abap}   
        // Tạo một chỉ mục
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Tìm kiếm cụm từ ở dạng văn bản

        // Ký tự caret đầu tiên ở đầu chỉ ra rằng đây là truy vấn tìm kiếm bằng biểu thức chính quy
        String query = "^^(.)\\1{1,}";
        // Tìm kiếm hai hoặc nhiều ký tự giống nhau ở đầu một từ
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
