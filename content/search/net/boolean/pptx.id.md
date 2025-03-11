
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: id
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cari PPTX di .NET menggunakan operator boolean"
head_description: "API GroupDocs.Search for .NET memungkinkan pengembang C# untuk mencari konten dokumen menggunakan operator boolean seperti AND, OR, dan NOT."

############################# Header ############################
title: "Pencarian teks logika boolean" 
description: "GroupDocs.Search for .NET memudahkan pembuatan kueri pencarian lanjutan menggunakan operator boolean (AND, OR, NOT) dalam aplikasi .NET Anda."
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
       [GroupDocs.Search for .NET](/search/net/) adalah pustaka komprehensif untuk mencari dan mengindeks teks dalam dokumen. Ini mendukung lebih dari 70 format file, seperti PDF, Word, PowerPoint, Excel, gambar, dan file ZIP, memungkinkan pemrosesan yang efisien dari sejumlah besar informasi.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mencari konten dokumen PPTX menggunakan logika boolean"
    content: |
      [GroupDocs.Search](/search/net/) membuat pencarian konten dokumen PPTX menjadi sederhana. Ini menyediakan kondisi pencarian logika Boolean untuk memperhalus hasil di aplikasi .NET.
      
      1. Tentukan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file PPTX.
      3. Jalankan pencarian dan ambil hasilnya.
      4. Proses hasilnya.
   
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

        // Lakukan pencarian menggunakan kueri kompleks
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Jelajahi fitur-fitur canggih untuk pencarian dan pengindeksan dokumen"
  description: "Pustaka GroupDocs.Search for .NET menyederhanakan pencarian teks dan pengindeksan untuk lebih dari 70 format file. Temukan dan kelola informasi dengan alat pencarian canggih."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Fitur utama dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks yang kuat"
      content: "Cari teks di berbagai jenis file, termasuk PDF, dokumen Word, presentasi PowerPoint, dan spreadsheet. Gunakan fitur seperti pencocokan tepat, pencarian fuzzy, dan wildcard untuk memperhalus hasil."

    # feature loop
    - title: "Indeks set data besar"
      content: "Buat dan kelola indeks untuk pencarian yang lebih cepat. Pengindeksan menyusun dan mengorganisir data, membuatnya lebih mudah untuk mencari koleksi dokumen yang luas."

    # feature loop
    - title: "Mendukung berbagai bahasa"
      content: "Cari dokumen dalam lebih dari 80 bahasa, dengan dukungan untuk berbagai tata letak keyboard dan bentuk kata morfologis untuk meningkatkan akurasi pencarian."

    # feature loop
    - title: "Opsi pencarian yang dapat disesuaikan"
      content: "Sesuaikan pengaturan pencarian dengan fitur seperti sensitif terhadap huruf besar/kecil, filter rentang tanggal, dan kemampuan untuk mengecualikan kata atau data tertentu selama pengindeksan."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan kueri pencarian boolean yang canggih"
      content: |
        Contoh ini menunjukkan bagaimana menerapkan kueri boolean untuk mencari dokumen PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tetapkan folder untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Tentukan jalur ke dokumen yang akan dicari
          index.Add("c:/MyDocuments");

          // Buat kueri pencarian menggunakan logika Boolean
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // Ambil hasil pencarian
          SearchResult result = index.Search(booleanQuery);
          
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
            link: "/examples/search/formats/searchboolean.pptx"
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
    title: "Temukan fitur-fitur kunci"
    exclude: "boolean"
    description: "Jelajahi fungsi pencarian yang canggih dan efisien."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari di berbagai format dokumen populer"
    exclude: "PPTX"
    description: "GroupDocs.Search mendukung lebih dari 70 format file. Sesuaikan aturan pencarian dan manfaatkan pengindeksan untuk menghemat waktu dan usaha."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---