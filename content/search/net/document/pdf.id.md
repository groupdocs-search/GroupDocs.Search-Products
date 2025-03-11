
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: id
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cari dokumen PDF di .NET dengan GroupDocs.Search"
head_description: "Gunakan GroupDocs.Search for .NET untuk melakukan pencarian teks yang efisien dalam berbagai format dokumen dengan C#."

############################# Header ############################
title: "Pencarian teks dokumen yang canggih" 
description: "GroupDocs.Search for .NET mempermudah pencarian teks dalam format dokumen populer, memungkinkan Anda untuk membuat kueri pencarian yang kuat dalam aplikasi .NET Anda."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh Secara Gratis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) adalah pustaka yang kuat dirancang untuk pencarian dan pengindeksan teks penuh dalam dokumen. Ini mendukung lebih dari 70 format file, termasuk PDF, Word, PowerPoint, Excel, gambar, dan file ZIP, memastikan hasil pencarian yang cepat dan akurat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara melakukan pencarian teks di dokumen PDF"
    content: |
      [GroupDocs.Search](/search/net/) memungkinkan operasi pencarian konten canggih dalam dokumen PDF, memungkinkan hasil pencarian yang lebih terperinci dalam aplikasi .NET.
      
      1. Siapkan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file PDF.
      3. Konfigurasi opsi pencarian tambahan.
      4. Jalankan pencarian dan tinjau hasilnya.
   
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
        // Tentukan jalur untuk indeks pencarian
        Index index = new Index("c:/MyIndex");

        // Pilih folder yang berisi dokumen yang akan dicari
        index.Add("c:/MyDocuments");

        // Aktifkan pencarian homofon untuk menemukan kata yang terdengar mirip
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // Jalankan kueri pencarian yang kompleks
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fitur pencarian dan pengindeksan yang canggih"
  description: "GroupDocs.Search for .NET meningkatkan pencarian teks dan pengindeksan di lebih dari 70 format file, menyediakan alat yang efisien untuk menemukan dan mengelola informasi."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Fitur Utama dari GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks yang kuat"
      content: "Cari teks di berbagai jenis dokumen, termasuk PDF, dokumen Word, presentasi PowerPoint, dan spreadsheet. Gunakan fitur seperti pencocokan tepat, pencarian fuzzy, dan wildcard untuk memperhalus hasil Anda."

    # feature loop
    - title: "Pengindeksan cepat untuk set data besar"
      content: "Buat dan kelola indeks pencarian untuk pengambilan informasi yang cepat. Pengindeksan mengoptimalkan pencarian di koleksi dokumen yang besar."

    # feature loop
    - title: "Dukungan multi-bahasa"
      content: "Lakukan pencarian dalam lebih dari 80 bahasa, dengan dukungan untuk berbagai tata letak keyboard dan variasi kata untuk meningkatkan akurasi."

    # feature loop
    - title: "Pengaturan pencarian yang dapat disesuaikan"
      content: "Sesuaikan parameter pencarian dengan opsi seperti sensitivitas huruf besar, filter rentang tanggal, dan pengecualian kata untuk hasil yang lebih baik."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Melakukan kueri pencarian yang canggih"
      content: |
        Contoh ini menunjukkan bagaimana menerapkan kueri pencarian untuk dokumen PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tentukan folder untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Tentukan jalur ke file dokumen
          index.Add("c:/MyDocuments");

          // Berikan kata sandi untuk dokumen yang dilindungi
          index.Dictionaries.DocumentPasswords.Add("protected.pdf", "123456");

          // Aktifkan pencarian fuzzy untuk menemukan kata yang mirip
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // Ambil hasil pencarian
          SearchResult result = index.Search("Loarem", options);
          
          // Proses output pencarian
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
            link: "/examples/search/formats/searchdocument.pdf"
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
    title: "Jelajahi fitur utama"
    exclude: "document"
    description: "Manfaatkan fungsionalitas pencarian yang canggih dan berkinerja tinggi."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari di dokumen bisnis Anda"
    exclude: "PDF"
    description: "GroupDocs.Search mendukung lebih dari 70 format file, termasuk dokumen kantor, memungkinkan pencarian yang cepat dan efisien dengan kemampuan pengindeksan."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---