
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: id
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Temukan teks dalam PDF dengan GroupDocs.Search di Node.js"
head_description: "Gunakan GroupDocs.Search for Node.js via Java dengan JavaScript untuk mencari teks secara efisien dalam berbagai format dokumen."

############################# Header ############################
title: "Solusi pencarian dokumen cerdas" 
description: "Temukan teks dalam berbagai format dokumen dengan GroupDocs.Search for Node.js via Java. Buat kueri pencarian lanjutan dalam aplikasi Node.js Anda."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Coba Gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Pendahuluan ke GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) adalah perpustakaan berkinerja tinggi untuk pencarian teks penuh dan pengindeksan dokumen. Ini mendukung lebih dari 70 jenis file, termasuk PDF, Word, PowerPoint, Excel, gambar, dan arsip ZIP, sehingga memastikan hasil yang cepat dan akurat.

############################# Steps ############################
steps:
    enable: true
    title: "Lakukan pencarian di file PDF"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) memungkinkan Anda untuk melakukan pencarian dalam file PDF, memperhalus hasil di aplikasi Node.js via Java.
      
      1. Tentukan folder penyimpanan untuk indeks pencarian.
      2. Pilih folder dengan file PDF.
      3. Atur parameter pencarian tambahan.
      4. Jalankan pencarian dan analisis hasilnya.
   
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

        // Tentukan direktori untuk penyimpanan indeks pencarian
        const index = new searchLib.Index("c:/MyIndex");

        // Pilih folder yang berisi dokumen untuk dicari
        index.add("c:/MyDocuments");

        // Aktifkan pencarian homofon untuk kata-kata yang terdengar mirip
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Jalankan kueri pencarian kompleks
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Kemampuan pencarian & pengindeksan lanjutan"
  description: "GroupDocs.Search for Node.js via Java menyediakan alat pencarian teks dan pengindeksan yang kuat di lebih dari 70 format dokumen, memudahkan untuk menemukan dan mengatur informasi."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Manfaat Utama dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks komprehensif"
      content: "Temukan teks dalam beberapa jenis dokumen, termasuk PDF, dokumen Word, presentasi PowerPoint, dan spreadsheet. Gunakan kecocokan tepat, pencarian fuzzy, dan wildcard untuk hasil yang lebih terperinci."

    # feature loop
    - title: "Pengindeksan efisien untuk data besar"
      content: "Percepat pencarian dengan membuat indeks terstruktur, memudahkan pengambilan informasi dari koleksi dokumen yang besar."

    # feature loop
    - title: "Mendukung lebih dari 80 bahasa"
      content: "Cari dalam dokumen dalam berbagai bahasa, dengan pengenalan otomatis berbagai bentuk kata dan tata letak keyboard."

    # feature loop
    - title: "Pengaturan pencarian kustom"
      content: "Sesuaikan opsi pencarian seperti sensitivitas huruf besar kecil, filter tanggal, dan pengecualian kata untuk mendapatkan hasil yang tepat."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan pencarian untuk dokumen PDF"
      content: |
        Contoh ini menunjukkan cara menggunakan kueri pencarian dalam dokumen PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Setel direktori untuk pengindeksan pencarian
          const index = new searchLib.Index("c:/MyIndex");
              
          // Berikan jalur file untuk penyimpanan dokumen
          index.add("c:/MyDocuments");

          // Masukkan kata sandi untuk file yang dilindungi
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", '123456');

          // Aktifkan pencarian fuzzy untuk deteksi kata serupa
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Ekstrak hasil pencarian
          const result = index.search("Loarem", options);
          
          // Proses dan tinjau hasilnya
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "Jelajahi fitur utama"
    exclude: "document"
    description: "Temukan fitur pencarian berkecepatan tinggi yang dirancang untuk meningkatkan efisiensi dan akurasi."
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
    title: "Cari di berbagai dokumen"
    exclude: "PDF"
    description: "GroupDocs.Search bekerja dengan lebih dari 70 format file, termasuk dokumen kantor, memastikan pencarian yang cepat dan akurat dengan dukungan pengindeksan."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---