
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:52
draft: false
lang: id
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Cari frasa dalam XLSX menggunakan Java"
head_description: "GroupDocs.Search for Java memperkaya aplikasi Java dengan kemampuan pencarian frasa yang canggih untuk konten dokumen."

############################# Header ############################
title: "Temukan frasa dalam dokumen" 
description: "Dengan GroupDocs.Search for Java, temukan frasa spesifik dengan cepat. Tambahkan fungsionalitas pencarian yang kuat ke aplikasi Java Anda."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Fitur GroupDocs.Search"
    link: "/search/java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) adalah pustaka yang kuat untuk mengindeks dan mencari teks dalam dokumen. Ini mendukung lebih dari 70 format file, termasuk PDF, dokumen Word, spreadsheet Excel, gambar, dan file ZIP, memastikan hasil pencarian yang cepat dan tepat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menemukan frasa dalam dokumen XLSX"
    content: |
      [GroupDocs.Search](/search/java/) menyederhanakan pencarian frasa dalam dokumen XLSX. Gunakan berbagai opsi untuk memperbaiki hasil pencarian dalam aplikasi Java.
      
      1. Buat direktori indeks pencarian.
      2. Tentukan folder dengan file XLSX.
      3. Sesuaikan parameter pencarian.
      4. Ambil dan analisis hasil pencarian.
   
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
        // Tentukan jalur indeks pencarian
        Index index = new Index("c:/MyIndex");

        // Tentukan folder yang berisi dokumen
        index.add("c:/MyDocuments");

        // Atur preferensi pencarian
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Eksekusi kueri pencarian
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Jelajahi mesin pencarian dokumen Java"
  description: "GroupDocs.Search for Java memungkinkan pencarian frasa di lebih dari 70 format file. Temukan dan atur data dengan mudah menggunakan fitur pencarian canggih."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Kemampuan kunci dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian frasa"
      content: "Temukan frasa tepat dalam dokumen bisnis, seperti PDF, file Word, presentasi, dan spreadsheet. Gunakan karakter wildcard dan opsi lainnya saat frasa yang tepat tidak diketahui."

    # feature loop
    - title: "Pengindeksan data yang dioptimalkan"
      content: "Percepat pencarian dokumen dengan membuat dan menggunakan kembali indeks pencarian. Pengindeksan mengatur data secara efisien untuk pencarian yang lebih cepat dan lebih akurat."

    # feature loop
    - title: "Kompatibilitas multi-bahasa"
      content: "Cari dokumen dalam lebih dari 80 bahasa. Mendukung tata letak keyboard yang berbeda dan analisis morfologi untuk meningkatkan ketepatan pencarian."

    # feature loop
    - title: "Opsi pencarian canggih"
      content: "Sesuaikan pencarian dengan sensitivitas huruf besar, pencarian fuzzy, pencocokan homofon, pemfilteran dokumen, dan fitur kuat lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan metode pencarian canggih"
      content: |
        Pelajari cara menyusun kueri untuk pencarian dalam XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Tentukan direktori untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Atur jalur ke dokumen target
          index.add("c:/MyDocuments");

          // Buat kueri pencarian untuk frasa tertentu
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Ambil hasil pencarian
          SearchResult result = index.search(query);
          
          // Proses dan gunakan hasil yang diperoleh
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Kemampuan pencarian canggih"
    exclude: "phrase"
    description: "Manfaatkan fungsionalitas pencarian mutakhir untuk meningkatkan ketepatan dan kinerja."
    items: 
          
        # operation loop 1
        - name: "Cari berdasarkan kondisi"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "Temukan informasi dalam dokumen menggunakan kondisi boolean"

        # operation loop 2
        - name: "Pencarian sensitif huruf"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Tingkatkan akurasi pencarian dengan mempertimbangkan sensitivitas huruf"

        # operation loop 3
        - name: "Pengindeksan dokumen"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "Indeks dokumen sekali dan gunakan indeks untuk beberapa pencarian"

        # operation loop 4
        - name: "Filter pencarian"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "Gunakan filter untuk mempersempit data yang diproses"

        # operation loop 5
        - name: "Frasa tepat"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "Cari kalimat atau frasa tertentu"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Pencarian frasa dalam dokumen bisnis"
    exclude: "XLSX"
    description: "GroupDocs.Search memungkinkan pencarian frasa dalam lebih dari 70 format dokumen. Manfaatkan opsi canggih dan pengindeksan untuk pencarian yang efisien."
    items: 
        # format loop 1
        - name: "Pencarian frasa DOCX"
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Pencarian frasa PDF"
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Pencarian frasa PPTX"
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Pencarian frasa TXT"
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Pencarian frasa XLSX"
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---