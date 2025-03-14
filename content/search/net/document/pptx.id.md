
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: id
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cari dokumen PPTX di .NET dengan GroupDocs.Search"
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
    title: "Cara melakukan pencarian teks di dokumen PPTX"
    content: |
      [GroupDocs.Search](/search/net/) memungkinkan operasi pencarian konten canggih dalam dokumen PPTX, memungkinkan hasil pencarian yang lebih terperinci dalam aplikasi .NET.
      
      1. Siapkan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file PPTX.
      3. Konfigurasi opsi pencarian tambahan.
      4. Jalankan pencarian dan tinjau hasilnya.
   
    code:
      platform: "net"
      copy_title: "Salin"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Hasil pencarian"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "klik untuk menyalin"
        copy_done: "tersalin"
      links:
        #  loop
        - title: "Contoh lebih lanjut"
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
        Contoh ini menunjukkan bagaimana menerapkan kueri pencarian untuk dokumen PPTX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tentukan folder untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Tentukan jalur ke file dokumen
          index.Add("c:/MyDocuments");

          // Berikan kata sandi untuk dokumen yang dilindungi
          index.Dictionaries.DocumentPasswords.Add("protected.pptx", "123456");

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
          copy_done: "tersalin"
        top_links:
          #  loop
          - title: "Unduh hasil"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pptx"
        links:
          #  loop
          - title: "Contoh lebih lanjut"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "Dokumentasi"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Search secara gratis atau minta lisensi"
  items:
    #  loop
    - title: "unduh Nuget"
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
        - name: "Cari berdasarkan kondisi"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "Temukan informasi dalam dokumen menggunakan kondisi boolean"

        # operation loop 2
        - name: "Pencarian sensitif huruf"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "Tingkatkan akurasi pencarian dengan mempertimbangkan sensitivitas huruf"

        # operation loop 3
        - name: "Pengindeksan dokumen"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "Indeks dokumen sekali dan gunakan indeks untuk beberapa pencarian"

        # operation loop 4
        - name: "Filter pencarian"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "Gunakan filter untuk mempersempit data yang diproses"

        # operation loop 5
        - name: "Frasa tepat"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "Cari kalimat atau frasa tertentu"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Cari di dokumen bisnis Anda"
    exclude: "PPTX"
    description: "GroupDocs.Search mendukung lebih dari 70 format file, termasuk dokumen kantor, memungkinkan pencarian yang cepat dan efisien dengan kemampuan pengindeksan."
    items: 
        # format loop 1
        - name: "Cari dalam dokumen DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Cari dalam dokumen PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Cari dalam dokumen PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Cari dalam dokumen TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Cari dalam dokumen XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---