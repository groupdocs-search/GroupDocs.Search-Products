
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: id
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Cari di dokumen PPTX menggunakan Node.js"
head_description: "GroupDocs.Search for Node.js via Java menambahkan kemampuan pencarian teks yang cepat dan akurat ke aplikasi JavaScript, mendukung berbagai format dokumen."

############################# Header ############################
title: "Temukan teks dalam dokumen bisnis" 
description: "GroupDocs.Search for Node.js via Java menyediakan fungsi pencarian yang kuat dan fleksibel untuk dokumen. Integrasikan pencarian teks ke dalam aplikasi Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) adalah perpustakaan pencarian dan pengindeksan yang kuat yang memungkinkan pengambilan teks cepat dalam dokumen. Mendukung lebih dari 70 format file, termasuk PDF, Word, Excel, dan PowerPoint, memastikan pencarian yang akurat dan efisien.

############################# Steps ############################
steps:
    enable: true
    title: "Cara melakukan pencarian di dokumen PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) membuat pencarian teks di dokumen PPTX sederhana dan efisien untuk aplikasi Node.js via Java.
      
      1. Buat direktori untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi dokumen.
      3. Tetapkan opsi pencarian untuk menyertakan hanya file PPTX.
      4. Jalankan pencarian dan ambil hasilnya.
   
    code:
      platform: "nodejs-java"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Tentukan direktori untuk menyimpan indeks pencarian
        const index = new searchLib.Index("c:/MyIndex");

        // Tentukan folder yang berisi dokumen yang dapat dicari
        index.add("c:/MyDocuments");

        // Batasi pencarian ke format file tertentu
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".pptx");

        // Ambil dan proses hasil pencarian
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kemampuan pencarian lanjutan"
  description: "GroupDocs.Search for Node.js via Java meningkatkan efisiensi pencarian dokumen dengan mengindeks lebih dari 70 format file. Optimalkan pengambilan konten dengan teknik pencarian lanjutan."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Fitur utama dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks komprehensif"
      content: "Ekstrak dan temukan teks dalam format dokumen populer, seperti PDF, file Word, spreadsheet, dan presentasi. Mendukung pencarian fuzzy, homofon, dan kueri wildcard."

    # feature loop
    - title: "Pengindeksan yang dioptimalkan untuk performa"
      content: "Percepat pencarian dengan membuat indeks yang dapat digunakan kembali. Meningkatkan kecepatan dan efisiensi saat bekerja dengan koleksi dokumen besar."

    # feature loop
    - title: "Dukungan multi-bahasa"
      content: "Cari melalui dokumen dalam lebih dari 80 bahasa. Mengenali tata letak keyboard dan variasi kata untuk akurasi yang lebih baik."

    # feature loop
    - title: "Opsi pencarian yang dapat disesuaikan"
      content: "Sesuaikan hasil pencarian dengan filter, ekspresi reguler, sensitivitas huruf besar/kecil, dan pengaturan fleksibel lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter dokumen yang dapat dicari"
      content: |
        Pelajari cara memperhalus pencarian dokumen menggunakan filter.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Konfigurasi indeks untuk mengecualikan format file yang tidak diinginkan
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Tentukan direktori yang berisi dokumen
          index.add("c:/MyDocuments");

          // Proses output pencarian untuk digunakan lebih lanjut
          const result = index.Search("Lorem", options);
          
          // Proses output pencarian untuk digunakan lebih lanjut
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Salin"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pptx"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Cobalah fitur GroupDocs.Search secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Fungsi utama"
    exclude: "filters"
    description: "Lakukan pencarian teks yang cepat dan tepat di seluruh dokumen."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari dalam berbagai format dokumen"
    exclude: "PPTX"
    description: "GroupDocs.Search mendukung lebih dari 70 jenis file, memungkinkan pencarian teks yang efisien di berbagai dokumen kantor dan bisnis."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---