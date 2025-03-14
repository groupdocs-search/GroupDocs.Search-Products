
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: id
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cari dalam dokumen XLSX menggunakan .NET"
head_description: "GroupDocs.Search for .NET meningkatkan aplikasi C# dengan pencarian teks yang efisien di berbagai format dokumen bisnis."

############################# Header ############################
title: "Cari teks dalam dokumen bisnis" 
description: "GroupDocs.Search for .NET memungkinkan pencarian teks yang kuat dan fleksibel dalam dokumen Anda. Integrasikan fungsionalitas pencarian ke dalam aplikasi .NET."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh gratis"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Apa itu GroupDocs.Search?"
    link: "/search/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) adalah perpustakaan yang kuat untuk pencarian teks yang efisien dan pengindeksan dokumen. Ini mendukung lebih dari 70 format file, termasuk dokumen standar industri seperti PDF, Word, Excel, dan PowerPoint. Tingkatkan performa pencarian dengan hasil yang cepat dan akurat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mencari dalam data XLSX"
    content: |
      [GroupDocs.Search](/search/net/) memungkinkan pencarian teks yang efisien dalam dokumen XLSX, menjadikannya ideal untuk aplikasi .NET.
      
      1. Siapkan folder untuk menyimpan indeks pencarian.
      2. Pilih folder yang berisi file Anda.
      3. Konfigurasi opsi pencarian untuk memproses hanya dokumen XLSX.
      4. Laksanakan pencarian dan ambil hasil.
   
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
        // Jalan untuk menyimpan indeks pencarian yang dapat digunakan kembali
        Index index = new Index("c:/MyIndex");

        // Folder yang berisi dokumen
        index.Add("c:/MyDocuments");

        // Cari hanya di dalam format file tertentu
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".xlsx");

        // Ambil hasil pencarian
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Fitur pencarian canggih"
  description: "GroupDocs.Search for .NET memungkinkan pencarian teks yang canggih di lebih dari 70 format file. Pengindeksan meningkatkan efisiensi pencarian dan membantu mengelola konten dokumen secara efektif."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian teks canggih"
      content: "Ekstrak teks relevan dari dokumen bisnis populer, termasuk PDF, file Word, presentasi, dan spreadsheet. Mendukung berbagai teknik pencarian seperti pencarian fuzzy, deteksi homofon, dan wildcard."

    # feature loop
    - title: "Pengindeksan yang dioptimalkan untuk pencarian yang lebih cepat"
      content: "Buat dan gunakan kembali indeks pencarian untuk meningkatkan kecepatan pencarian. Pengindeksan mengoptimalkan kinerja saat mencari melalui kumpulan dokumen besar."

    # feature loop
    - title: "Dukungan untuk berbagai bahasa"
      content: "Lakukan pencarian dalam dokumen yang ditulis dalam lebih dari 80 bahasa. Mendeteksi berbagai tata letak keyboard dan variasi kata untuk meningkatkan akurasi."

    # feature loop
    - title: "Pengaturan pencarian yang fleksibel"
      content: "Perbaiki hasil pencarian dengan opsi yang dapat disesuaikan, termasuk filter, ekspresi reguler, dan pengaturan sensitivitas huruf besar."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filter dokumen yang akan diproses"
      content: |
        Pelajari cara mempersempit pencarian dokumen dengan menggunakan filter.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Siapkan indeks yang mengecualikan format file tertentu.
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // Tentukan direktori dokumen.
          index.Add("c:/MyDocuments");

          // Ambil hasil pencarian.
          SearchResult result = index.Search("Lorem");
          
          // Proses dan gunakan output pencarian.
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
            link: "/examples/search/formats/searchfilters.xlsx"
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
    title: "Fitur kunci"
    exclude: "filters"
    description: "Lakukan pencarian data yang akurat dan efisien."
    items: 
          
        # operation loop 1
        - name: "Cari berdasarkan kondisi"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "Temukan informasi dalam dokumen menggunakan kondisi boolean"

        # operation loop 2
        - name: "Pencarian sensitif huruf"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Tingkatkan akurasi pencarian dengan mempertimbangkan sensitivitas huruf"

        # operation loop 3
        - name: "Pengindeksan dokumen"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "Indeks dokumen sekali dan gunakan indeks untuk beberapa pencarian"

        # operation loop 4
        - name: "Filter pencarian"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "Gunakan filter untuk mempersempit data yang diproses"

        # operation loop 5
        - name: "Frasa tepat"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "Cari kalimat atau frasa tertentu"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Temukan data dalam dokumen bisnis Anda"
    exclude: "XLSX"
    description: "GroupDocs.Search mendukung lebih dari 70 format file, memungkinkan pemrosesan dan pencarian yang efisien pada dokumen kantor yang populer."
    items: 
        # format loop 1
        - name: "Filter pencarian untuk DOCX"
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Dokumen Open XML Microsoft Word"
          
        # format loop 2
        - name: "Filter pencarian untuk PDF"
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: "Filter pencarian untuk PPTX"
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "Presentasi Open XML PowerPoint"

        # format loop 4
        - name: "Filter pencarian untuk TXT"
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: "Filter pencarian untuk XLSX"
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Spreadsheet Open XML Microsoft Excel"
  

---