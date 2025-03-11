
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: id
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Temukan teks dalam dokumen DOCX dengan GroupDocs.Search untuk Java"
head_description: "GroupDocs.Search for Java membantu pengembang Java untuk cepat mencari teks dalam berbagai format dokumen."

############################# Header ############################
title: "Pencarian teks dokumen yang cerdas" 
description: "Dengan GroupDocs.Search for Java, Anda dapat dengan mulus mencari dan mengekstrak teks dari berbagai jenis dokumen di aplikasi Java Anda."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan Uji Coba Gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa yang dilakukan GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) adalah pustaka pencarian dan pengindeksan dokumen yang kuat yang mendukung lebih dari 70 format file, termasuk PDF, Word, PowerPoint, Excel, gambar, dan arsip ZIP. Ini memungkinkan kemampuan pencarian yang cepat, akurat, dan dapat diskalakan untuk koleksi dokumen besar.

############################# Steps ############################
steps:
    enable: true
    title: "Lakukan pencarian teks dalam file DOCX"
    content: |
      [GroupDocs.Search](/search/java/) memudahkan pencarian file DOCX menggunakan logika canggih dan pengindeksan, meningkatkan akurasi pencarian dalam aplikasi Java.
      
      1. Siapkan direktori untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file DOCX.
      3. Tentukan opsi pencarian tambahan.
      4. Jalankan pencarian dan analisis hasilnya.
   
    code:
      platform: "java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Tentukan direktori untuk menyimpan indeks pencarian
        Index index = new Index("c:/MyIndex");

        // Tentukan folder yang berisi dokumen yang dapat dicari
        index.add("c:/MyDocuments");

        // Aktifkan pencarian homofon untuk mencocokkan kata dengan pengucapan serupa
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Jalankan kueri pencarian yang canggih
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kemampuan pencarian dan pengindeksan yang ditingkatkan"
  description: "GroupDocs.Search for Java menyederhanakan pencarian teks dan pengindeksan di lebih dari 70 format dokumen, menyediakan alat yang efisien untuk mengelola dan mengambil informasi dengan cepat."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Fitur Inti dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks yang komprehensif"
      content: "Temukan teks di berbagai format dokumen seperti PDF, dokumen Word, presentasi PowerPoint, dan spreadsheet. Gunakan pencocokan yang tepat, pencarian kabur, dan operator wildcard untuk hasil pencarian yang lebih terperinci."

    # feature loop
    - title: "Pengindeksan yang dioptimalkan untuk data besar"
      content: "Buat indeks terstruktur untuk mempercepat pencarian, memudahkan navigasi melalui repositori dokumen yang besar secara efisien."

    # feature loop
    - title: "Mendukung berbagai bahasa"
      content: "Lakukan pencarian dalam lebih dari 80 bahasa dengan dukungan bawaan untuk berbagai tata letak keyboard dan variasi morfologi kata, meningkatkan akurasi."

    # feature loop
    - title: "Pengaturan pencarian yang fleksibel"
      content: "Sesuaikan pencarian dengan opsi seperti sensitif terhadap kapitalisasi, pemfilteran berdasarkan tanggal, dan kemampuan untuk mengecualikan kata tertentu untuk hasil yang tepat."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menerapkan kueri pencarian canggih"
      content: |
        Contoh ini menggambarkan bagaimana menggunakan kueri pencarian untuk mencari dalam dokumen DOCX secara efisien.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Tentukan direktori untuk pengindeksan pencarian
          Index index = new Index("c:/MyIndex");
              
          // Berikan jalur file untuk dokumen
          index.add("c:/MyDocuments");

          // Masukkan kata sandi untuk dokumen terenkripsi
          index.getDictionaries().getDocumentPasswords().add("protected.docx", "123456");

          // Aktifkan pencarian kabur untuk mendeteksi kata-kata serupa
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Ambil hasil pencarian
          SearchResult result = index.Search("Loarem", options);
          
          // Proses dan analisis hasil pencarian
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Salin"
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
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchdocument.docx"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Cobalah fitur GroupDocs.Search secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Ikhtisar fitur kunci"
    exclude: "document"
    description: "Temukan fungsi pencarian teks berkinerja tinggi yang dirancang untuk efisiensi dan ketepatan."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Temukan informasi di dokumen DOCX dengan GroupDocs.Search"
    exclude: "DOCX"
    description: "GroupDocs.Search mendukung lebih dari 70 format, termasuk file kantor, memungkinkan pencarian cepat dengan fitur pengindeksan canggih."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---