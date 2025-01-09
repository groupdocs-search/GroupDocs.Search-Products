---
############################# Static ############################
layout: "family"
date:  2025-01-09T15:38:59
draft: false

product: "Search"
product_tag: "search"

lang: vi

############################# Head ############################
head_title: "Tìm kiếm & Chỉ mục văn bản tài liệu | APIs & Ứng dụng Web Miễn phí"
head_description: "Thực hiện tìm kiếm văn bản hiệu quả và lập chỉ mục dữ liệu trên PDF, MS Office, OpenDocument, và các định dạng tệp phổ biến khác bằng cách sử dụng APIs của chúng tôi hoặc ứng dụng tìm kiếm tài liệu trực tuyến miễn phí."

############################# Header ############################
title: "Giải pháp Tìm kiếm và Lập chỉ mục Tài liệu Toàn diện"
description:  |
  Thực hiện tìm kiếm văn bản và lập chỉ mục trên PDF, Microsoft Office, OpenOffice và nhiều định dạng tệp tài liệu khác.

  Nhanh chóng tìm thông tin trong các bộ sưu tập tài liệu lớn với khả năng tìm kiếm toàn văn tiên tiến.

  Tùy chỉnh các tính năng tìm kiếm như từ đồng nghĩa, tìm kiếm mờ, và phân loại từ để nâng cao độ chính xác và kết quả.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Chọn nền tảng của bạn"
  title: "Khả năng độc lập của nền tảng"
  description: "GroupDocs.Search tương thích với các hệ điều hành và framework sau:"
  details_link_title: "Tìm hiểu thêm"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Bất kỳ trình soạn thảo văn bản nào khác
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Các tính năng chính của GroupDocs.Search"
  description: "GroupDocs.Search cung cấp các công cụ mạnh mẽ để lập chỉ mục và tìm kiếm văn bản trong các định dạng tài liệu phổ biến. Đơn giản hóa và nâng cao quản lý tài liệu với chức năng tìm kiếm nâng cao."

  items:
    # items loop
    - icon: "view"
      title: "Tìm kiếm văn bản nâng cao"
      content: "Thực hiện tìm kiếm văn bản nhanh chóng và chính xác trên các tài liệu đã được lập chỉ mục."

    # items loop
    - icon: "manipulate"
      title: "Tùy chọn tìm kiếm có thể tùy chỉnh"
      content: "Sử dụng các tính năng như tìm kiếm mờ, từ đồng nghĩa, và phân loại từ để có kết quả chính xác hơn."

    # items loop
    - icon: "merge"
      title: "Hỗ trợ nhiều định dạng"
      content: "Lập chỉ mục và tìm kiếm nội dung trong Microsoft Office, PDF, OpenOffice và các định dạng phổ biến khác."

    # items loop
    - icon: "additional"
      title: "Lập chỉ mục hiệu quả"
      content: "Xây dựng và duy trì chỉ mục nhanh chóng cho các bộ sưu tập tài liệu lớn."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Tìm kiếm văn bản trong các định dạng tài liệu phổ biến"
  description: "GroupDocs.Search ví dụ mã"
  items:
    # code sample loop
    - title: "Tìm kiếm văn bản"
      content: |
       GroupDocs.Search là một công cụ mạnh mẽ để tìm văn bản trong tài liệu. Bạn có thể tìm kiếm qua nhiều tài liệu ở các định dạng khác nhau được lưu trữ trong một thư mục cụ thể. Kết quả tìm kiếm được lưu trữ trong một thư mục riêng, cho phép bạn truy cập và tái sử dụng mà không cần thực hiện tìm kiếm lại.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Tạo một thể hiện của lớp Index, chỉ định thư mục để lưu trữ các chỉ mục.
            Index index = new Index("\\Index Folder");

            //Xác định đường dẫn đến các tài liệu nơi tìm kiếm sẽ được thực hiện.
            index.Add("\\Documents Folder");

            //Tạo một thể hiện của đối tượng SearchOptions.
            SearchOptions options = new SearchOptions();

            //Tiến hành tìm kiếm cho văn bản mong muốn.
            SearchResult result = index.Search("ipsum dolor", options);

            //Xử lý và quản lý kết quả tìm kiếm.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Tạo một thể hiện của lớp Index, chỉ định thư mục để lưu trữ các chỉ mục.
            Index index = new Index("\\Index Folder");

            //Xác định đường dẫn đến các tài liệu nơi tìm kiếm sẽ được thực hiện.
            index.add("\\Documents Folder");

            //Tạo một thể hiện của đối tượng SearchOptions.
            SearchOptions options = new SearchOptions();

            //Tiến hành tìm kiếm cho văn bản mong muốn.
            SearchResult result = index.search("ipsum dolor", options);

            //Xử lý và quản lý kết quả tìm kiếm.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Tạo một thể hiện của lớp Index, chỉ định thư mục để lưu trữ các chỉ mục.
            const index = new searchLib.Index('\\Index Folder');

            //Xác định đường dẫn đến các tài liệu nơi tìm kiếm sẽ được thực hiện.
            index.add('\\Documents Folder');

            //Tạo một thể hiện của đối tượng SearchOptions.
            const options = new searchLib.SearchOptions();

            //Tiến hành tìm kiếm cho văn bản mong muốn.
            const result = index.search('ipsum dolor', options);

            //Xử lý và quản lý kết quả tìm kiếm.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Hỗ trợ hơn 70+ định dạng tệp"
  description: "GroupDocs.Search hỗ trợ gần như tất cả các định dạng tệp được sử dụng rộng rãi."

############################# Metrics ###############################
metrics:
  enable: true
  title: "Thống kê Sản phẩm của Chúng tôi"
  description: "Khám phá các chỉ số chính thể hiện hiệu suất, độ phủ sóng và sự phát triển của chúng tôi."

  items:
    # items loop
    - number: "70+"
      title: "Các định dạng được hỗ trợ"
      content: "Chúng tôi cung cấp khả năng tương thích với hơn 70 định dạng tài liệu phổ biến."

    # items loop
    - number: "500k"
      title: "Tải xuống NuGet"
      content: "GroupDocs.Search cho .NET đã được tải xuống hơn 500,000 lần trên NuGet."

    # items loop
    - number: "12k"
      title: "Tải xuống Maven"
      content: "Các nhà phát triển Java đã tải GroupDocs.Search hơn 12,000 lần từ Maven."

    # items loop
    - number: "150+"
      title: "Khách hàng hài lòng"
      content: "Các nhà phát triển và các doanh nghiệp hàng đầu trên toàn thế giới tin tưởng vào sản phẩm của chúng tôi để có giải pháp sáng tạo."


############################# Customers ###############################
customers:
  enable: true
  title: "Khách hàng Hài lòng của Chúng tôi"
  description: "Thư viện GroupDocs được tin tưởng bởi các thương hiệu và tổ chức hàng đầu trên toàn cầu."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Bắt đầu Hành Trình của Bạn Ngày Hôm Nay!"
  description: "Trải nghiệm GroupDocs.Search miễn phí trên nền tảng ưa thích của bạn."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Các câu hỏi thường gặp"
  description: "Tìm câu trả lời cho những câu hỏi thường gặp về GroupDocs.Search."

  items:
    # items loop
    - question: "Có cần công cụ bên ngoài để tìm kiếm tài liệu với GroupDocs.Search không?"
      answer: "Không, GroupDocs.Search hoạt động như một giải pháp độc lập và không cần các công cụ hoặc phần mềm bổ sung như Adobe Acrobat hoặc Microsoft Office để thực hiện tìm kiếm."

    # items loop
    - question: "Tôi có thể thử nghiệm GroupDocs.Search trước khi mua không?"
      answer: "Có, bạn có thể! GroupDocs.Search cung cấp một bản dùng thử miễn phí. Bạn có thể khám phá các tính năng của nó, tuy nhiên phiên bản dùng thử có thể bao gồm những hạn chế như hình mờ hoặc chức năng bị hạn chế. Để mở khóa tất cả các tính năng, bạn có thể yêu cầu một giấy phép tạm thời miễn phí trong 30 ngày. Tìm hiểu thêm trên trang [giấy phép tạm thời](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Có những tùy chọn cấp phép nào có sẵn?"
      answer: "Chúng tôi cung cấp nhiều mô hình cấp phép cho GroupDocs.Search, được điều chỉnh cho các nhu cầu khác nhau. Chọn một giấy phép dựa trên kích thước nhóm của bạn, phân cảnh sử dụng, hoặc liệu bạn có cần SDK/API để phân phối cho khách hàng hay không. Đối với việc sử dụng linh hoạt, hãy xem xét một giấy phép tính phí theo mức tiêu thụ, nơi bạn thanh toán dựa trên mức sử dụng thực tế. Tìm hiểu thêm về các tùy chọn của bạn trên trang [định giá](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Ứng dụng Web"
  description: "Khám phá GroupDocs.Search với ứng dụng web miễn phí của chúng tôi. Thực hiện tìm kiếm văn bản và lập chỉ mục trên hơn 70 định dạng tệp phổ biến trực tiếp trên trình duyệt của bạn—hoàn toàn miễn phí."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Tìm kiếm trong PDF, Excel, Word, PowerPoint, và các loại tệp khác ngay từ trình duyệt web của bạn."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Tải lên DOCX để thực hiện tìm kiếm văn bản nâng cao mà không cần cài đặt phần mềm."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Kiểm tra khả năng lập chỉ mục và truy xuất PDF trên các định dạng khác nhau miễn phí."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---