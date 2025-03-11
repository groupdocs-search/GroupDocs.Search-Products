
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: id
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Pencarian Sensitif Huruf pada XLSX Menggunakan .NET"
head_description: "API GroupDocs.Search for .NET memungkinkan pengembang C# untuk melakukan pencarian sensitif huruf di berbagai dokumen."

############################# Header ############################
title: "Pencarian Sensitif Huruf" 
description: "GroupDocs.Search for .NET memungkinkan Anda untuk membuat kueri pencarian sensitif huruf yang canggih dalam aplikasi .NET Anda."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Gratis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) adalah perpustakaan yang kuat untuk pencarian teks dan pengindeksan dalam dokumen. Ini mendukung lebih dari 70 format file, termasuk PDF, Word, PowerPoint, Excel, gambar, dan file ZIP, memastikan penanganan data besar yang efisien.

############################# Steps ############################
steps:
    enable: true
    title: "Cara Melakukan Pencarian Sensitif Huruf di Dokumen XLSX"
    content: |
      [GroupDocs.Search](/search/net/) menyederhanakan pencarian sensitif huruf dalam dokumen XLSX. Gunakan ini untuk memperbaiki hasil di aplikasi .NET.
      
      1. Tentukan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file XLSX.
      3. Jalankan pencarian dan ambil hasilnya.
      4. Proses hasil pencarian.
   
    code:
      platform: "net"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "klik untuk menyalin"
        copy_done: "disalin"
      links:
        #  loop
        - title: "Lebih banyak contoh"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "Dokumentasi"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // Tentukan jalur ke folder indeks
        Index index = new Index("c:/MyIndex");

        // Tentukan folder yang berisi dokumen untuk dicari
        index.Add("c:/MyDocuments");

        // Aktifkan pencarian sensitif huruf di opsi
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // Jalankan pencarian
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fitur Canggih untuk Pencarian dan Pengindeksan Dokumen"
  description: "Perpustakaan GroupDocs.Search for .NET menyederhanakan pencarian teks dan pengindeksan di lebih dari 70 format file. Temukan dan kelola informasi dengan alat pencarian yang kuat."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Fitur Utama GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian Teks Canggih"
      content: "Cari teks di berbagai format file, termasuk PDF, dokumen Word, spreadsheet, dan presentasi. Gunakan opsi seperti kecocokan tepat, pencarian kabur, dan wildcard untuk hasil yang akurat."

    # feature loop
    - title: "Indeks Data Besar"
      content: "Bangun dan kelola indeks untuk pencarian yang lebih cepat. Pengindeksan yang terorganisir menyederhanakan pencarian koleksi dokumen yang luas."

    # feature loop
    - title: "Dukungan Multi-Bahasa"
      content: "Cari dalam dokumen yang menggunakan lebih dari 80 bahasa, dengan dukungan untuk berbagai tata letak keyboard dan bentuk kata untuk hasil yang lebih akurat."

    # feature loop
    - title: "Opsi Pencarian yang Dapat Disesuaikan"
      content: "Sesuaikan pengaturan pencarian dengan sensitivitas huruf, filter rentang tanggal, dan kemampuan untuk mengecualikan kata-kata atau data tertentu selama pengindeksan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan Kuasi Pencarian Sensitif Huruf"
      content: |
        Contoh ini menunjukkan cara menggunakan kueri sensitif huruf untuk mencari dokumen XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tentukan folder untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Tentukan jalur ke dokumen yang akan dicari
          index.Add("c:/MyDocuments");

          // Buat kueri pencarian
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // Aktifkan opsi pencarian sensitif huruf
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // Cari teks dalam dokumen
          SearchResult result = index.Search(wordQuery, options);
          
          // Proses hasil pencarian
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "Salin"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "klik untuk menyalin"
          copy_done: "disalin"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
        links:
          #  loop
          - title: "Lebih banyak contoh"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Cobalah fitur GroupDocs.Search secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "Unduhan Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "Lisensi"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Temukan Fitur Utama"
    exclude: "case-sensitive"
    description: "Jelajahi fungsi pencarian yang canggih dan efisien."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari Format Dokumen Populer"
    exclude: "XLSX"
    description: "GroupDocs.Search mendukung lebih dari 70 format file. Sesuaikan aturan pencarian dan gunakan pengindeksan untuk menghemat waktu dan usaha."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---