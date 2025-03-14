
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: id
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cari dalam dokumen PPTX menggunakan Java"
head_description: "GroupDocs.Search for Java menambahkan pencarian teks yang kuat ke aplikasi Java, mendukung berbagai format dokumen bisnis."

############################# Header ############################
title: "Temukan teks dalam dokumen bisnis" 
description: "GroupDocs.Search for Java memungkinkan Anda mencari teks dalam dokumen menggunakan kueri yang fleksibel dan tepat. Integrasikan fungsionalitas pencarian ke dalam aplikasi Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) adalah pustaka kokoh untuk pencarian teks cepat dan pengindeksan dokumen. Ini mendukung lebih dari 70 format file, termasuk standar industri seperti PDF, Word, Excel, dan PowerPoint. Tingkatkan aplikasi Anda dengan kemampuan pencarian yang cepat dan akurat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mencari dalam dokumen PPTX"
    content: |
      [GroupDocs.Search](/search/java/) memungkinkan pencarian teks yang cepat dan efisien dalam dokumen PPTX, sempurna untuk aplikasi Java.
      
      1. Tentukan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi dokumen Anda.
      3. Konfigurasikan opsi pencarian untuk membatasi hasil hanya pada dokumen PPTX.
      4. Jalankan pencarian dan dapatkan hasilnya.
   
    code:
      platform: "java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Hasil pencarian"
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
        copy_done: "tersalin"
      links:
        #  loop
        - title: "Contoh lebih lanjut"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Direktori untuk menyimpan indeks pencarian yang dapat digunakan kembali
        Index index = new Index("c:/MyIndex");

        // Folder yang berisi dokumen
        index.add("c:/MyDocuments");

        // Filter pencarian berdasarkan format dokumen
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pptx");

        // Ambil hasil pencarian
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kemampuan pencarian yang ditingkatkan"
  description: "GroupDocs.Search for Java menyediakan pencarian teks lanjutan di lebih dari 70 format file. Pengindeksan mempercepat pencarian dan meningkatkan efisiensi manajemen dokumen."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Fitur kunci GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks yang kuat"
      content: "Temukan teks dalam format dokumen populer seperti PDF, file Word, presentasi, dan spreadsheet. Mendukung berbagai metode pencarian, termasuk pencarian fuzzy, homofon, dan wildcard."

    # feature loop
    - title: "Pengindeksan yang dioptimalkan untuk kinerja lebih baik"
      content: "Buat dan gunakan kembali indeks pencarian untuk meningkatkan kecepatan dan efisiensi pencarian, terutama dalam koleksi dokumen besar."

    # feature loop
    - title: "Dukungan pencarian multibahasa"
      content: "Cari dalam dokumen yang ditulis dalam lebih dari 80 bahasa. Mendeteksi berbagai tata letak keyboard dan variasi kata untuk meningkatkan akurasi."

    # feature loop
    - title: "Opsi pencarian yang dapat disesuaikan"
      content: "Persempit hasil pencarian dengan filter, ekspresi reguler, dan pengaturan pencarian lanjutan lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter dokumen sebelum mencari"
      content: |
        Pelajari cara menyaring pencarian menggunakan filter
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Atur indeks yang mengecualikan format file tertentu
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Tentukan jalur penyimpanan dokumen
          index.add("c:/MyDocuments");

          // Ambil hasil pencarian
          SearchResult result = index.search("Lorem", options);
          
          // Proses dan gunakan hasil pencarian
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
          copy_done: "tersalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pptx"
        links:
          #  loop
          - title: "Contoh lebih lanjut"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Search secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "unduh Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Fitur kunci"
    exclude: "filters"
    description: "Lakukan pencarian teks yang tepat dan efisien."
    items: 
          
        # operation loop 1
        - name: "Cari berdasarkan kondisi"
          operation: "boolean"
          link: "/search/java/boolean/pptx/"
          description: "Temukan informasi dalam dokumen menggunakan kondisi boolean"

        # operation loop 2
        - name: "Pencarian sensitif huruf"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pptx/"
          description: "Tingkatkan akurasi pencarian dengan mempertimbangkan sensitivitas huruf"

        # operation loop 3
        - name: "Pengindeksan dokumen"
          operation: "document"
          link: "/search/java/document/pptx/"
          description: "Indeks dokumen sekali dan gunakan indeks untuk beberapa pencarian"

        # operation loop 4
        - name: "Filter pencarian"
          operation: "filters"
          link: "/search/java/filters/pptx/"
          description: "Gunakan filter untuk mempersempit data yang diproses"

        # operation loop 5
        - name: "Frasa tepat"
          operation: "phrase"
          link: "/search/java/phrase/pptx/"
          description: "Cari kalimat atau frasa tertentu"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari dalam dokumen bisnis"
    exclude: "PPTX"
    description: "GroupDocs.Search mendukung lebih dari 70 format file, memudahkan pencarian melalui dokumen kantor yang banyak digunakan."
    items: 
        # format loop 1
        - name: "Filter pencarian untuk DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Filter pencarian untuk PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Filter pencarian untuk PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Filter pencarian untuk TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Filter pencarian untuk XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---