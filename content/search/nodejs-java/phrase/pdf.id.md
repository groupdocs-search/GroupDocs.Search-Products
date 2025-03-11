
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: id
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Mencari frasa dalam PDF menggunakan Node.js"
head_description: "GroupDocs.Search for Node.js via Java menambahkan fungsionalitas pencarian frasa yang kuat ke aplikasi JavaScript untuk pencarian dokumen yang efisien."

############################# Header ############################
title: "Temukan frasa dalam dokumen" 
description: "Dengan GroupDocs.Search for Node.js via Java, Anda dapat dengan cepat menemukan frasa tertentu. Integrasikan kemampuan pencarian yang cepat dan akurat ke dalam aplikasi Node.js Anda."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Fitur GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) adalah perpustakaan berkinerja tinggi untuk mengindeks dan mencari teks dalam dokumen. Ini mendukung lebih dari 70 format file, termasuk PDF, dokumen Word, spreadsheet Excel, gambar, dan arsip ZIP, memastikan hasil pencarian yang akurat dan cepat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara menemukan frasa dalam dokumen PDF"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) memudahkan pencarian frasa dalam dokumen PDF. Terapkan berbagai opsi pencarian untuk memperbaiki hasil dalam aplikasi Node.js via Java.
      
      1. Siapkan folder indeks pencarian.
      2. Tentukan folder yang berisi file PDF.
      3. Konfigurasikan parameter pencarian.
      4. Ambil dan proses hasil pencarian.
   
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

        // Tentukan jalur untuk menyimpan indeks pencarian
        const index = new searchLib.Index("c:/MyIndex");

        // Tetapkan folder yang berisi dokumen-dokumen
        index.add("c:/MyDocuments");

        // Konfigurasi pengaturan pencarian
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Jalankan kueri pencarian
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Temukan mesin pencarian dokumen Node.js"
  description: "GroupDocs.Search for Node.js via Java memungkinkan pencarian frasa di lebih dari 70 format file, memudahkan menemukan dan mengatur data dengan fitur pencarian yang canggih."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Kemampuan kunci GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian frasa"
      content: "Temukan frasa tepat dalam dokumen bisnis seperti PDF, file Word, presentasi, dan spreadsheet. Gunakan karakter pengganti dan opsi pencarian fleksibel ketika frasa lengkap tidak diketahui."

    # feature loop
    - title: "Pengindeksan data yang dioptimalkan"
      content: "Tingkatkan kinerja pencarian dengan membuat indeks yang dapat digunakan kembali. Pengindeksan terstruktur mempercepat pencarian dokumen dan meningkatkan akurasi."

    # feature loop
    - title: "Kompatibilitas multi-bahasa"
      content: "Cari dokumen dalam lebih dari 80 bahasa dengan dukungan untuk berbagai tata letak keyboard dan variasi kata morfologis, memastikan hasil yang tepat."

    # feature loop
    - title: "Opsi pencarian canggih"
      content: "Sesuaikan pencarian dengan sensitifitas huruf, pencocokan fuzzy, deteksi homofon, pemfilteran dokumen, dan fitur kuat lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan teknik pencarian canggih"
      content: |
        Pelajari cara menyusun kueri untuk pencarian dalam PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Tentukan direktori indeks pencarian
          const index = new searchLib.Index("c:/MyIndex");
              
          // Tetapkan jalur ke dokumen target
          index.add("c:/MyDocuments");

          // Buat kueri untuk frasa yang diinginkan
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Ambil hasil pencarian
          const result = index.search(query);
          
          // Proses dan gunakan hasilnya
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "Kemampuan pencarian canggih"
    exclude: "phrase"
    description: "Manfaatkan fitur pencarian yang kuat untuk mendapatkan hasil yang lebih cepat dan lebih akurat."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Mencari frasa dalam dokumen bisnis"
    exclude: "PDF"
    description: "GroupDocs.Search mendukung pencarian frasa dalam lebih dari 70 format dokumen. Gunakan opsi canggih dan pengindeksan untuk memperlancar proses pencarian."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---