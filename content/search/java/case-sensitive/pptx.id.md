
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: id
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Lakukan Pencarian Sensitif Huruf di PPTX dengan Java"
head_description: "API GroupDocs.Search for Java membantu pengembang Java untuk menjalankan pencarian yang peka terhadap huruf di berbagai jenis dokumen."

############################# Header ############################
title: "Pencarian Dokumen Sensitif Huruf" 
description: "GroupDocs.Search for Java memungkinkan Anda untuk mengimplementasikan fungsi pencarian yang tepat dan peka terhadap huruf dalam proyek Java Anda."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Dapatkan Secara Gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Pelajari Tentang GroupDocs.Search"
    link: "/search/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) adalah alat serbaguna untuk pencarian teks dan pengindeksan di berbagai dokumen. Alat ini mendukung lebih dari 70 format seperti PDF, file Word, presentasi PowerPoint, lembar Excel, gambar, dan ZIP, memungkinkan Anda untuk menangani kumpulan data besar secara efisien.

############################# Steps ############################
steps:
    enable: true
    title: "Panduan untuk Pencarian Sensitif Huruf di File PPTX"
    content: |
      Dengan [GroupDocs.Search](/search/java/), Anda dapat melakukan pencarian sensitif huruf dalam dokumen PPTX, meningkatkan proyek Java Anda.
      
      1. Tetapkan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file PPTX.
      3. Jalankan pencarian sensitif huruf dan kumpulkan hasilnya.
      4. Proses dan gunakan hasil pencarian.
   
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
        // Tentukan lokasi untuk penyimpanan indeks
        Index index = new Index("c:/MyIndex");

        // Tunjuk ke folder yang berisi dokumen untuk dicari
        index.add("c:/MyDocuments");

        // Aktifkan mode sensitif huruf di pengaturan pencarian
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Laksanakan pencarian
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Alat Pencarian dan Pengindeksan yang Ditingkatkan"
  description: "Dengan GroupDocs.Search for Java, Anda dapat menyederhanakan pencarian dokumen dan pengindeksan untuk lebih dari 70 format, memudahkan Anda menemukan dan mengorganisasi informasi."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Sorotan dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian Teks yang Fleksibel"
      content: "Telusuri dokumen seperti PDF, file Word, spreadsheet, dan presentasi. Gunakan alat seperti pencocokan tepat, pencarian fuzzy, dan dukungan karakter joker untuk memperhalus hasil Anda."

    # feature loop
    - title: "Manajemen Indeks yang Efisien"
      content: "Atur dan indeks dataset besar untuk meningkatkan kecepatan dan performa pencarian saat menangani koleksi dokumen yang besar."

    # feature loop
    - title: "Dukungan untuk Bahasa Global"
      content: "Lakukan pencarian dalam lebih dari 80 bahasa, mendukung berbagai tata letak keyboard dan variasi linguistik untuk akurasi yang lebih baik."

    # feature loop
    - title: "Filter Pencarian yang Dapat Disesuaikan"
      content: "Sesuaikan kriteria pencarian dengan opsi seperti sensitivitas huruf, filter rentang tanggal, dan pengecualian kata atau data yang tidak diinginkan selama pengindeksan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Contoh: Kueri Pencarian Sensitif Huruf"
      content: |
        Contoh ini menunjukkan cara mengimplementasikan pencarian sensitif huruf untuk dokumen PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Tentukan direktori untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Tentukan lokasi folder dokumen
          index.add("c:/MyDocuments");

          // Siapkan kueri pencarian
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Aktifkan sensitivitas huruf di opsi pencarian
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Lakukan pencarian dokumen
          SearchResult result = index.search(wordQuery, options);
          
          // Proses hasil yang diambil
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
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    title: "Ikhtisar Fitur Utama"
    exclude: "case-sensitive"
    description: "Temukan kemampuan pencarian yang kuat dan efektif yang ditawarkan oleh GroupDocs.Search for Java."
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
    title: "Format File yang Didukung untuk Pencarian"
    exclude: "PPTX"
    description: "GroupDocs.Search bekerja dengan lebih dari 70 format dokumen populer, menawarkan pengaturan pencarian yang dapat disesuaikan dan pengindeksan yang efisien."
    items: 
        # format loop 1
        - name: "Pencarian DOCX sensitif huruf"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Pencarian PDF sensitif huruf"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Pencarian PPTX sensitif huruf"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Pencarian TXT sensitif huruf"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Pencarian XLSX sensitif huruf"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---