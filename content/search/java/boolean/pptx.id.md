
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: id
format: Pptx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Pencarian Boolean di PPTX dengan Java"
head_description: "Dengan GroupDocs.Search for Java, pengembang dapat melakukan pencarian dokumen menggunakan operator Boolean seperti AND, OR, dan NOT."

############################# Header ############################
title: "Pencarian teks Boolean" 
description: "Gunakan GroupDocs.Search for Java untuk membuat kueri pencarian boolean (AND, OR, NOT) yang canggih dalam proyek Java Anda."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Tentang GroupDocs.Search"
    link: "/search/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) adalah pustaka serbaguna yang dirancang untuk pencarian teks dan pengindeksan data dalam dokumen. Ini mendukung lebih dari 70 tipe file, termasuk PDF, Word, Excel, PowerPoint, gambar, dan arsip ZIP, yang memungkinkan pencarian efisien melalui kumpulan data besar.

############################# Steps ############################
steps:
    enable: true
    title: "Cara melakukan pencarian boolean dalam dokumen PPTX"
    content: |
      [GroupDocs.Search](/search/java/) memfasilitasi pencarian teks dalam dokumen PPTX. Dengan dukungan untuk kondisi boolean, Anda dapat meningkatkan akurasi pencarian dalam aplikasi Java.
      
      1. Tentukan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi dokumen PPTX.
      3. Jalankan kueri pencarian dan ambil hasilnya.
      4. Proses hasil yang diperoleh.
   
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
        // Tentukan jalur untuk folder indeks
        Index index = new Index("c:/MyIndex");

        // Berikan jalur folder yang berisi dokumen untuk pencarian
        index.add("c:/MyDocuments");

        // Jalankan pencarian dengan kueri kompleks
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Alat kuat untuk pencarian dan pengindeksan dokumen"
  description: "GroupDocs.Search for Java menyederhanakan pencarian teks dan pengindeksan data untuk lebih dari 70 format. Alat canggihnya memungkinkan Anda menemukan dan mengelola konten dengan efektif."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks yang komprehensif"
      content: "Telusuri melalui berbagai format seperti PDF, dokumen Word, presentasi, spreadsheet, dan lainnya. Gunakan opsi seperti pencocokan tepat, pencarian fuzzy, dan kueri wildcard untuk memperhalus hasil."

    # feature loop
    - title: "Pengindeksan data yang efisien"
      content: "Bangun dan pertahankan indeks untuk pencarian dokumen yang lebih cepat. Fitur ini mengorganisir data dengan efisien, memudahkan penanganan koleksi dokumen besar."

    # feature loop
    - title: "Dukungan multi-bahasa"
      content: "Lakukan pencarian dalam dokumen yang ditulis dalam lebih dari 80 bahasa. Tingkatkan akurasi dengan memanfaatkan bentuk kata morfologis dan berbagai tata letak keyboard."

    # feature loop
    - title: "Kustomisasi pencarian yang fleksibel"
      content: "Sesuaikan pengaturan pencarian dengan fitur-fitur seperti sensitivitas huruf, filter rentang tanggal, dan pengecualian untuk memperhalus hasil Anda."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan kueri pencarian boolean yang kompleks"
      content: |
        Contoh ini menunjukkan cara melakukan pencarian Boolean dalam file PPTX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Tentukan folder untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Berikan jalur ke dokumen untuk dicari
          index.add("c:/MyDocuments");

          // Bangun kueri menggunakan logika Boolean
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Ambil hasil pencarian
          SearchResult result = index.search(booleanQuery);
          
          // Proses hasil yang diperoleh
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
            link: "/examples/search/formats/searchboolean.pptx"
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
    title: "Fitur utama dalam satu pandangan"
    exclude: "boolean"
    description: "Buka kemampuan pencarian yang kuat dan efisien"
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
    title: "Cari format dokumen populer"
    exclude: "PPTX"
    description: "GroupDocs.Search mendukung lebih dari 70 format file, memungkinkan Anda menyesuaikan aturan pencarian dan menggunakan pengindeksan untuk mengoptimalkan kinerja."
    items: 
        # format loop 1
        - name: "Cari DOCX dengan kondisi logika"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Cari PDF dengan kondisi logika"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Cari PPTX dengan kondisi logika"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Cari TXT dengan kondisi logika"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Cari XLSX dengan kondisi logika"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---