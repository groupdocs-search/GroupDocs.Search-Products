
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: vi
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Tìm kiếm cụm từ trong PPTX sử dụng Java"
head_description: "GroupDocs.Search for Java nâng cao các ứng dụng Java với khả năng tìm kiếm cụm từ tiên tiến cho nội dung tài liệu."

############################# Header ############################
title: "Tìm cụm từ trong tài liệu" 
description: "Nhanh chóng định vị các cụm từ cụ thể với GroupDocs.Search for Java. Thêm chức năng tìm kiếm mạnh mẽ vào các ứng dụng Java của bạn."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Tải về"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Các tính năng của GroupDocs.Search"
    link: "/search/java/"
    link_title: "Tìm hiểu thêm"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) là một thư viện mạnh mẽ để lập chỉ mục và tìm kiếm văn bản trong tài liệu. Nó hỗ trợ hơn 70 định dạng tệp, bao gồm PDF, tài liệu Word, bảng tính Excel, hình ảnh và tệp ZIP, đảm bảo kết quả tìm kiếm nhanh chóng và chính xác.

############################# Steps ############################
steps:
    enable: true
    title: "Cách tìm cụm từ trong tài liệu PPTX"
    content: |
      [GroupDocs.Search](/search/java/) đơn giản hóa việc tìm kiếm cụm từ trong các tài liệu PPTX. Sử dụng nhiều tùy chọn khác nhau để tinh chỉnh kết quả tìm kiếm trong các ứng dụng Java.
      
      1. Tạo một thư mục chỉ mục tìm kiếm.
      2. Chỉ định thư mục chứa các tệp PPTX.
      3. Điều chỉnh các tham số tìm kiếm.
      4. Lấy và phân tích kết quả tìm kiếm.
   
    code:
      platform: "java"
      copy_title: "Sao chép"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Kết quả tìm kiếm"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "nhấn để sao chép"
        copy_done: "đã sao chép"
      links:
        #  loop
        - title: "Thêm ví dụ"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Tài liệu hướng dẫn"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Định nghĩa đường dẫn chỉ mục tìm kiếm
        Index index = new Index("c:/MyIndex");

        // Chỉ định thư mục chứa tài liệu
        index.add("c:/MyDocuments");

        // Cài đặt tùy chọn tìm kiếm
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Thực hiện truy vấn tìm kiếm
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Khám phá công cụ tìm kiếm tài liệu Java"
  description: "GroupDocs.Search for Java cho phép tìm kiếm cụm từ trong hơn 70 định dạng tệp. Tìm kiếm và tổ chức dữ liệu một cách hiệu quả bằng cách sử dụng các tính năng tìm kiếm tiên tiến."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Các khả năng chính của GroupDocs.Search"
  features:
    # feature loop
    - title: "Tìm kiếm cụm từ"
      content: "Xác định các cụm từ chính xác trong các tài liệu kinh doanh, chẳng hạn như PDF, tệp Word, thuyết trình và bảng tính. Sử dụng ký tự đại diện và các tùy chọn khác khi cụm từ chính xác không rõ ràng."

    # feature loop
    - title: "Tối ưu hóa lập chỉ mục dữ liệu"
      content: "Tăng tốc độ tìm kiếm tài liệu bằng cách tạo và tái sử dụng các chỉ mục tìm kiếm. Việc lập chỉ mục giúp tổ chức dữ liệu một cách hiệu quả để tìm kiếm nhanh hơn và chính xác hơn."

    # feature loop
    - title: "Tương thích đa ngôn ngữ"
      content: "Tìm kiếm tài liệu bằng hơn 80 ngôn ngữ khác nhau. Hỗ trợ các bố cục bàn phím khác nhau và phân tích hình thái để cải thiện độ chính xác của tìm kiếm."

    # feature loop
    - title: "Tùy chọn tìm kiếm nâng cao"
      content: "Tùy chỉnh tìm kiếm với độ nhạy cảm với chữ hoa, tìm kiếm mờ, kết hợp đồng âm, lọc tài liệu và nhiều tính năng mạnh mẽ khác."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Sử dụng các phương pháp tìm kiếm nâng cao"
      content: |
        Tìm hiểu cách xây dựng truy vấn để tìm kiếm trong PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Định nghĩa thư mục cho chỉ mục tìm kiếm
          Index index = new Index("c:/MyIndex");
              
          // Cài đặt đường dẫn đến các tài liệu mục tiêu
          index.add("c:/MyDocuments");

          // Tạo một truy vấn tìm kiếm cho một cụm từ cụ thể
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Lấy kết quả tìm kiếm
          SearchResult result = index.search(query);
          
          // Xử lý và sử dụng các kết quả đã lấy
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Sao chép"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "nhấn để sao chép"
          copy_done: "đã sao chép"
        top_links:
          #  loop
          - title: "Tải xuống kết quả"
            icon: "download"
            link: "/examples/search/formats/searchphrase.pptx"
        links:
          #  loop
          - title: "Thêm ví dụ"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Tài liệu hướng dẫn"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Sẵn sàng để bắt đầu?"
  description: "Hãy thử các tính năng của GroupDocs.Search miễn phí hoặc yêu cầu giấy phép"
  items:
    #  loop
    - title: "Tải xuống Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Giấy phép"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Khả năng tìm kiếm nâng cao"
    exclude: "phrase"
    description: "Sử dụng các chức năng tìm kiếm tiên tiến để cải thiện độ chính xác và hiệu suất."
    items: 
          
        # operation loop 1
        - name: "Tìm kiếm theo điều kiện"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "Tìm thông tin trong tài liệu sử dụng các điều kiện boolean"

        # operation loop 2
        - name: "Tìm kiếm phân biệt chữ hoa chữ thường"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "Cải thiện độ chính xác của tìm kiếm bằng cách xem xét sự phân biệt chữ hoa chữ thường"

        # operation loop 3
        - name: "Lập chỉ mục tài liệu"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "Lập chỉ mục tài liệu một lần và tái sử dụng chỉ mục cho nhiều lần tìm kiếm"

        # operation loop 4
        - name: "Bộ lọc tìm kiếm"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "Sử dụng bộ lọc để thu hẹp dữ liệu đang được xử lý"

        # operation loop 5
        - name: "Cụm từ chính xác"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "Tìm kiếm một câu hoặc cụm từ cụ thể"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Tìm kiếm cụm từ trong tài liệu kinh doanh"
    exclude: "PPTX"
    description: "GroupDocs.Search cho phép tìm kiếm cụm từ trong hơn 70 định dạng tài liệu. Tận dụng các tùy chọn tiên tiến và lập chỉ mục cho việc tìm kiếm hiệu quả."
    items: 
        # format loop 1
        - name: "Tìm kiếm cụm từ trong DOCX"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Tài liệu Microsoft Word Open XML"
          
        # format loop 2
        - name: "Tìm kiếm cụm từ trong PDF"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Định dạng Tài liệu Di động Adobe"
          
        # format loop 3
        - name: "Tìm kiếm cụm từ trong PPTX"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Bài thuyết trình PowerPoint Open XML"

        # format loop 4
        - name: "Tìm kiếm cụm từ trong TXT"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Tài liệu văn bản"
          
        # format loop 5
        - name: "Tìm kiếm cụm từ trong XLSX"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Bảng tính Microsoft Excel Open XML"
  

---