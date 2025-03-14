
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: id
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Lakukan Pencarian Sensi Huruf Besar di XLSX dengan Node.js"
head_description: "API GroupDocs.Search for Node.js via Java memungkinkan pengembang JavaScript untuk melakukan pencarian sensi huruf besar di berbagai jenis dokumen."

############################# Header ############################
title: "Pencarian Sensi Huruf Besar" 
description: "GroupDocs.Search for Node.js via Java memungkinkan Anda mengimplementasikan fungsi pencarian sensi huruf besar yang canggih dalam aplikasi Node.js Anda."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) adalah perpustakaan yang kuat untuk mencari dan mengindeks teks dalam dokumen. Ini mendukung lebih dari 70 format, termasuk PDF, Word, Excel, Presentasi, gambar, dan file ZIP, memungkinkan penanganan data dalam jumlah besar secara efisien.

############################# Steps ############################
steps:
    enable: true
    title: "Langkah untuk Melakukan Pencarian Sensi Huruf Besar di File XLSX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) memudahkan melakukan pencarian sensi huruf besar di file XLSX, meningkatkan alur kerja Node.js via Java Anda.
      
      1. Siapkan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file XLSX.
      3. Jalankan pencarian dan dapatkan hasilnya.
      4. Proses dan gunakan hasilnya.
   
    code:
      platform: "nodejs-java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Hasil pencarian"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "klik untuk menyalin"
        copy_done: "tersalin"
      links:
        #  loop
        - title: "Contoh lebih lanjut"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Tentukan jalur untuk folder indeks
        const index = new searchLib.Index("c:/MyIndex");

        // Setel folder yang berisi dokumen untuk dicari
        index.add("c:/MyDocuments");

        // Aktifkan pencarian sensi huruf besar dalam pengaturan
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Lakukan pencarian
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fitur Utama untuk Pencarian dan Pengindeksan Dokumen"
  description: "Dengan GroupDocs.Search for Node.js via Java, Anda dapat mencari dan mengindeks teks dalam lebih dari 70 format file. Akses dan atur informasi dengan mudah menggunakan alat pencarian yang canggih."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Fitur Inti dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian Teks Komprehensif"
      content: "Temukan teks dalam berbagai jenis dokumen seperti PDF, file Word, spreadsheet, dan presentasi. Gunakan opsi seperti pencocokan tepat, pencarian fuzzy, dan wildcard untuk hasil yang akurat."

    # feature loop
    - title: "Pengindeksan Data yang Efisien"
      content: "Buat dan kelola indeks untuk mempercepat pencarian. Pengindeksan membantu Anda mengatur dan dengan cepat menemukan data dalam koleksi dokumen yang besar."

    # feature loop
    - title: "Mendukung Banyak Bahasa"
      content: "Cari dokumen dalam lebih dari 80 bahasa dengan dukungan untuk berbagai tata letak keyboard dan variasi kata, memastikan hasil pencarian yang akurat."

    # feature loop
    - title: "Pengaturan Pencarian yang Dapat Disesuaikan"
      content: "Sesuaikan pengaturan pencarian, termasuk sensi huruf besar, filter tanggal, dan pengecualian istilah atau data tertentu selama pengindeksan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Contoh: Implementasi Pencarian Sensi Huruf Besar"
      content: |
        Contoh ini menunjukkan cara melakukan pencarian sensi huruf besar untuk dokumen XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Tentukan folder untuk indeks pencarian
          const index = new searchLib.Index("c:/MyIndex");
              
          // Berikan jalur ke folder dokumen
          index.add("c:/MyDocuments");

          // Atur kueri pencarian
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Aktifkan pengaturan pencarian sensi huruf besar
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Cari teks dalam dokumen
          const result = index.search(wordQuery, options);
          
          // Proses dan tangani hasilnya
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Salin"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "klik untuk menyalin"
          copy_done: "tersalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
        links:
          #  loop
          - title: "Contoh lebih lanjut"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Search secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "unduh NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Fungsi Utama"
    exclude: "case-sensitive"
    description: "Jelajahi fitur canggih untuk pencarian dokumen yang cepat dan tepat."
    items: 
          
        # operation loop 1
        - name: "Cari berdasarkan kondisi"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Temukan informasi dalam dokumen menggunakan kondisi boolean"

        # operation loop 2
        - name: "Pencarian sensitif huruf"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Tingkatkan akurasi pencarian dengan mempertimbangkan sensitivitas huruf"

        # operation loop 3
        - name: "Pengindeksan dokumen"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Indeks dokumen sekali dan gunakan indeks untuk beberapa pencarian"

        # operation loop 4
        - name: "Filter pencarian"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Gunakan filter untuk mempersempit data yang diproses"

        # operation loop 5
        - name: "Frasa tepat"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Cari kalimat atau frasa tertentu"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Format Dokumen yang Kompatibel"
    exclude: "XLSX"
    description: "GroupDocs.Search mendukung lebih dari 70 format dokumen. Sesuaikan opsi pencarian Anda dan hemat waktu dengan pengindeksan."
    items: 
        # format loop 1
        - name: "Pencarian DOCX sensitif huruf"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Pencarian PDF sensitif huruf"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Pencarian PPTX sensitif huruf"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Pencarian TXT sensitif huruf"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Pencarian XLSX sensitif huruf"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---