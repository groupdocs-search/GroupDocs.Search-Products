---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: vi
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Thư viện Tìm kiếm & Lập chỉ mục văn bản Node.js cho Tài liệu, PDF, Tệp Office và Web"
head_description: "Giải pháp tìm kiếm văn bản nâng cao cho các ứng dụng Node.js để tìm kiếm, lập chỉ mục & thu thập dữ liệu từ các tài liệu: PDF, Word, Excel, thuyết trình, email & định dạng tệp web."

############################# Header ############################
title: "Tìm kiếm & Lập chỉ mục tài liệu sử dụng API Node.js"
description: "Nâng cao các ứng dụng Node.js bằng cách triển khai Tìm kiếm văn bản trong Tất cả các định dạng tài liệu phổ biến."
words:
  for: "cho"

actions:
  main: "Tải xuống NPM miễn phí"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Cấp phép"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Bắt đầu Hành Trình của Bạn Ngày Hôm Nay!"
  description: "Khám phá các khả năng của GroupDocs.Search miễn phí hoặc bảo đảm một giấy phép để mở khóa toàn bộ tiềm năng của nó."

release:
  title: "Phiên bản {0} đã phát hành"
  notes: "Xem những gì mới"
  downloads: "Tải xuống"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Thực hiện tìm kiếm văn bản trong một thư mục với JavaScript"
  more: "Thêm ví dụ"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Tạo một chỉ mục cho tài liệu của bạn
    const index = new searchLib.Index('c:/MyIndex');

    // Thêm tài liệu vào chỉ mục để tìm kiếm hiệu quả
    index.add('c:/MyDocuments');
    
    // Tìm kiếm từ hoặc cụm từ cụ thể, chẳng hạn như
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Tổng quan về GroupDocs.Search"
  description: "Thư viện Node.js JavaScript cho tìm kiếm văn bản"
  features:
    # feature loop
    - title: "Tính năng Lập chỉ mục và Tìm kiếm của Node.js"
      content: "Lập chỉ mục trong GroupDocs.Search for Node.js via Java thu thập, lưu trữ và phân tích dữ liệu để thực hiện các hoạt động tìm kiếm chính xác và hiệu quả. Các chỉ mục này thường được sử dụng để thực hiện tìm kiếm."

    # feature loop
    - title: "Hợp nhất nhiều chỉ mục để nâng cao hiệu quả tìm kiếm"
      content: "GroupDocs.Search for Node.js via Java API cho phép hợp nhất nhiều chỉ mục thành một. Những thay đổi thường xuyên tạo ra nhiều chỉ mục delta, có thể làm chậm hiệu suất tìm kiếm. Giải pháp của chúng tôi hợp nhất những chỉ mục delta này vào một chỉ mục chung, chứa tất cả thông tin từ các chỉ mục delta đã hợp nhất, cải thiện đáng kể hiệu quả tìm kiếm trong khi vẫn giữ nguyên các chỉ mục delta không thay đổi. Nhiều chức năng có thể được cấu hình để tinh chỉnh quy trình này."

    # feature loop
    - title: "Nhận diện các truy vấn tìm kiếm từ các bố cục bàn phím khác nhau"
      content: "GroupDocs.Search for Node.js via Java nhận diện các truy vấn tìm kiếm không khớp với bố cục bàn phím. Hiện tại, 88 ngôn ngữ và 164 bố cục bàn phím khác nhau được hỗ trợ."

    # feature loop
    - title: "Tìm kiếm bằng hình thái từ"
      content: "Với GroupDocs.Search for Node.js via Java, bạn có thể tìm kiếm nhiều dạng từ khác nhau, chẳng hạn như danh từ số ít và số nhiều, hoặc tất cả các dạng của một động từ. Các ngôn ngữ tiếng Anh và không phải tiếng Anh có thể được tùy chỉnh cho các dạng từ cụ thể."

############################# Platforms ############################
platforms:
  enable: true
  title: "Khả năng độc lập của nền tảng"
  description: "GroupDocs.Search for Node.js via Java hỗ trợ tất cả các hệ điều hành và trình quản lý gói phổ biến."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Các định dạng tệp được hỗ trợ"
  description: |
    GroupDocs.Search for Node.js via Java cho phép xử lý một loạt các định dạng tệp. [Khám phá danh sách đầy đủ](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
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
  title: "Các tính năng của GroupDocs.Search for Node.js via Java"
  description: "Kiểm soát nội dung tài liệu kinh doanh bằng cách sử dụng công cụ tìm kiếm nâng cao của chúng tôi, hỗ trợ các định dạng tệp phổ biến bao gồm PDF, DOCX, XLSX, PPTX và nhiều hơn nữa."

  items:
    # feature loop
    - icon: "document_info"
      title: "Tham số linh hoạt"
      content: "Sử dụng Phạm vi Ngày & Tính nhạy cảm với chữ hoa làm tham số tìm kiếm."

    # feature loop
    - icon: "detect"
      title: "Tìm kiếm kiểm tra chính tả"
      content: "Sử dụng các cụm từ tìm kiếm với kiểm tra chính tả và ký hiệu thay thế & Bỏ qua các ký tự đặc biệt trong truy vấn."

    # feature loop
    - icon: "collect"
      title: "Lọc kết quả"
      content: "Thiết lập Lọc tài liệu trong các kết quả tìm kiếm."

    # feature loop
    - icon: "get"
      title: "Nhập & Xuất"
      content: "Thực hiện Nhập hoặc Sử dụng danh sách để sửa đổi ký tự trong quá trình lập chỉ mục & Xuất ra một tệp."

    # feature loop
    - icon: "remove"
      title: "Bỏ qua dữ liệu không cần thiết"
      content: "Chọn lọc để Bỏ qua lập chỉ mục cho các tệp cụ thể & Bỏ qua các từ cụ thể để lập chỉ mục nhanh hơn."

    # feature loop
    - icon: "style"
      title: "Xử lý URL"
      content: "Trích xuất văn bản định dạng HTML thành tệp & Tạo URL để điều hướng các kết quả tìm kiếm trong HTML."

    # feature loop
    - icon: "detect"
      title: "Tìm kiếm nhanh"
      content: "Chia nhỏ Tìm kiếm thành các phần nhỏ hơn để Tìm kiếm nhanh hơn trong các chỉ mục lớn."

    # feature loop
    - icon: "manipulate"
      title: "Xử lý dòng"
      content: "Lập chỉ mục các tài liệu từ các dòng và cấu trúc dữ liệu."

    # feature loop
    - icon: "compare"
      title: "Xử lý lỗi chính tả"
      content: "Kích hoạt Số lần xuất hiện chính xác cho mỗi từ tìm thấy để cung cấp các gợi ý từ thay thế trong trường hợp có lỗi chính tả."

    # feature loop
    - icon: "unreadable_characters"
      title: "Hỗ trợ lưu trữ"
      content: "Lập chỉ mục các lưu trữ nén bên trong các lưu trữ ZIP khác và truy xuất danh sách các tệp đã lập chỉ mục trong một lưu trữ."

    # feature loop
    - icon: "hidden_print"
      title: "Tiết kiệm không gian đĩa"
      content: "Tiết kiệm không gian với lập chỉ mục gọn gàng & Lập chỉ mục các tài liệu được bảo vệ bằng mật khẩu."

    # feature loop
    - icon: "style"
      title: "Từ đồng nghĩa tùy chỉnh"
      content: "Thêm từ đồng nghĩa tiếng Anh vào từ điển đồng nghĩa mặc định."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mẫu mã"
  description: "Khám phá các chức năng của GroupDocs.Search for Node.js via Java với các ví dụ."
  items:
    # code sample loop
    - title: "Sử dụng tìm kiếm 'fuzzy' để nâng cao năng suất"
      content: |
        Tận hưởng tính năng linh hoạt của GroupDocs.Search for Node.js via Java để tăng cường kiểm soát nội dung tài liệu với các thuật toán tìm kiếm tinh vi. [Tìm hiểu thêm](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Cách xử lý kết quả tìm kiếm">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Tạo một chỉ mục
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Thiết lập tùy chọn tìm kiếm
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Tìm kiếm các tài liệu chứa từ 'nước' hoặc cụm từ 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Xử lý kết quả tìm kiếm
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Biểu thức chính quy có sẵn cho các kịch bản tìm kiếm nâng cao"
      content: |
        GroupDocs.Search for Node.js via Java cho phép chúng ta sử dụng biểu thức chính quy để thu hẹp kết quả tìm kiếm. [Khám phá sâu vào các kỹ thuật tìm kiếm nâng cao](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Cách tìm kiếm bằng biểu thức chính quy">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Tạo một chỉ mục
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Tìm kiếm cụm từ ở dạng văn bản

        // Ký tự caret đầu tiên ở đầu chỉ ra rằng đây là truy vấn tìm kiếm bằng biểu thức chính quy
        const query = '^^(.)\\1{1,}';
        // Tìm kiếm hai hoặc nhiều ký tự giống nhau ở đầu một từ
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
