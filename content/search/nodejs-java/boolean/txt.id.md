
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: id
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Pencarian Boolean TXT melalui Node.js"
head_description: "Gunakan API GroupDocs.Search for Node.js via Java untuk melaksanakan pencarian lanjutan dalam konten dokumen dengan operator boolean seperti AND, OR, dan NOT, yang dirancang untuk pengembang JavaScript."

############################# Header ############################
title: "Lakukan pencarian logika boolean" 
description: "Dengan GroupDocs.Search for Node.js via Java, Anda dapat membuat kueri pencarian lanjutan menggunakan operator boolean (AND, OR, NOT) tanpa hambatan dalam lingkungan Node.js Anda."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Sekarang"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) adalah alat yang kuat untuk mencari dan mengindeks teks dalam dokumen. Ini mendukung lebih dari 70 format seperti PDF, Word, Excel, PowerPoint, gambar, dan file ZIP, sehingga memudahkan pemrosesan sejumlah besar informasi secara efisien.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mencari dalam dokumen TXT menggunakan operator boolean"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) memungkinkan Anda mencari konten dalam file TXT dengan efektif. Dengan logika boolean, Anda dapat menyempurnakan kueri pencarian Anda dalam aplikasi Node.js via Java untuk akurasi yang lebih baik.
      
      1. Siapkan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file TXT untuk pencarian.
      3. Jalankan kueri pencarian dan ambil hasilnya.
      4. Proses dan analisis hasil pencarian.
   
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

        // Setel lokasi untuk folder indeks
        const index = new searchLib.Index("c:/MyIndex");

        // Tentukan folder yang berisi dokumen untuk dicari
        index.add("c:/MyDocuments");

        // Laksanakan kueri pencarian dengan logika lanjutan
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Alat canggih untuk pencarian dan pengindeksan dokumen"
  description: "GroupDocs.Search for Node.js via Java menyederhanakan pencarian teks dan pengindeksan untuk lebih dari 70 jenis file, membantu Anda menemukan dan mengelola informasi dengan lebih cepat dan akurat."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks yang ditingkatkan"
      content: "Temukan teks dengan cepat di berbagai format seperti PDF, dokumen Word, presentasi, dan spreadsheet. Gunakan fitur seperti pencocokan tepat, pencarian wildcard, dan pencarian fuzzy untuk hasil yang akurat."

    # feature loop
    - title: "Pengindeksan data yang efisien"
      content: "Bangun dan kelola indeks untuk mempercepat pencarian dalam koleksi dokumen besar. Pengindeksan memastikan akses cepat dan terstruktur ke data Anda."

    # feature loop
    - title: "Dukungan multibahasa"
      content: "Cari di dokumen yang ditulis dalam lebih dari 80 bahasa. Dukungan morfologi dan kompatibilitas tata letak keyboard meningkatkan hasil pencarian dalam berbagai bahasa."

    # feature loop
    - title: "Pengaturan pencarian yang fleksibel"
      content: "Kustomisasi pencarian Anda dengan mengaktifkan sensitivitas huruf, menerapkan filter tanggal, atau melewatkan kata dan data tertentu selama pengindeksan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Contoh pencarian boolean lanjutan"
      content: |
        Contoh ini menunjukkan cara membuat kueri berbasis Boolean untuk mencari konten dalam dokumen TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Tentukan folder untuk indeks pencarian
          const index = new searchLib.Index("c:/MyIndex");
              
          // Berikan lokasi dokumen untuk dicari
          index.add("c:/MyDocuments");

          // Buat kueri menggunakan operator Boolean
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Ambil hasil pencarian
          const result = index.search(booleanQuery);
          
          // Proses dan gunakan hasil pencarian
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "Kemampuan utama GroupDocs.Search"
    exclude: "boolean"
    description: "Buka fitur pencarian yang canggih, efisien, dan dapat disesuaikan."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari format dokumen populer"
    exclude: "TXT"
    description: "GroupDocs.Search mendukung lebih dari 70 format file, menyediakan aturan pencarian yang fleksibel dan pengindeksan yang efisien untuk menghemat waktu dan usaha."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---