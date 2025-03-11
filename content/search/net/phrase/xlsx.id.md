
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: id
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "Cari frasa dalam XLSX menggunakan .NET"
head_description: "GroupDocs.Search for .NET meningkatkan aplikasi C# dengan kemampuan pencarian frasa yang kuat untuk konten dokumen."

############################# Header ############################
title: "Cari frasa dalam dokumen" 
description: "Temukan frasa tertentu dengan cepat menggunakan GroupDocs.Search for .NET. Integrasikan fungsi pencarian yang efisien ke dalam aplikasi .NET Anda."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Unduh"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "Fitur GroupDocs.Search"
    link: "/search/net/"
    link_title: "Pelajari lebih lanjut"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) adalah pustaka yang kuat untuk mengindeks dan mencari teks dalam dokumen. Ini mendukung lebih dari 70 format file, termasuk PDF, dokumen Word, spreadsheet Excel, gambar, dan file ZIP, memungkinkan hasil pencarian yang cepat dan akurat.

############################# Steps ############################
steps:
    enable: true
    title: "Cara mencari frasa dalam dokumen XLSX"
    content: |
      [GroupDocs.Search](/search/net/) menyederhanakan pencarian dalam dokumen XLSX. Gunakan berbagai opsi untuk memperbaiki hasil pencarian dalam aplikasi .NET.
      
      1. Siapkan folder indeks pencarian.
      2. Tentukan folder yang berisi file XLSX.
      3. Konfigurasi pengaturan pencarian.
      4. Ambil dan proses hasil pencarian.
   
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
        // Path untuk menyimpan indeks pencarian
        Index index = new Index("c:/MyIndex");

        // Folder yang berisi dokumen
        index.Add("c:/MyDocuments");

        // Konfigurasi opsi pencarian
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // Lakukan pencarian
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Temukan mesin pencarian dokumen .NET"
  description: "GroupDocs.Search for .NET memungkinkan pencarian frasa di lebih dari 70 format file. Temukan dan kelola data dengan efisiensi pencarian yang canggih."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Fitur utama GroupDocs.Search"
  features:
    # feature loop
    - title: "Pencarian frasa"
      content: "Cari frasa persis dalam dokumen bisnis, termasuk PDF, file Word, presentasi, dan spreadsheet. Gunakan wildcard dan opsi lainnya jika frasa yang tepat tidak diketahui."

    # feature loop
    - title: "Pengindeksan data yang efisien"
      content: "Buat dan gunakan kembali indeks pencarian untuk mempercepat pencarian dokumen. Indeksasi mengatur data secara efisien, menjadikan pencarian frasa lebih cepat."

    # feature loop
    - title: "Dukungan multi-bahasa"
      content: "Cari dokumen dalam lebih dari 80 bahasa. Mendukung berbagai tata letak keyboard dan bentuk kata morfologis untuk akurasi pencarian yang lebih baik."

    # feature loop
    - title: "Opsi pencarian yang fleksibel"
      content: "Sesuaikan pencarian dengan fitur-fitur seperti sensitivitas huruf besar, pencarian fuzzy dan homofon, penyaringan dokumen, dan lainnya."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Menggunakan teknik pencarian lanjutan"
      content: |
        Pelajari cara membuat kueri untuk mencari dalam XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // Tentukan folder untuk indeks pencarian
          Index index = new Index("c:/MyIndex");
              
          // Atur path ke dokumen untuk pencarian
          index.Add("c:/MyDocuments");

          // Buat kueri untuk frasa tertentu
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // Ambil hasil pencarian
          SearchResult result = index.Search(query);
          
          // Proses dan gunakan hasilnya
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Fitur lanjutan"
    exclude: "phrase"
    description: "Manfaatkan fungsi pencarian yang kuat dan efisien."
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
    title: "Pencarian frasa dalam dokumen bisnis"
    exclude: "XLSX"
    description: "GroupDocs.Search mendukung pencarian dalam lebih dari 70 format dokumen. Gunakan opsi lanjutan dan pengindeksan untuk memperlancar proses pencarian Anda."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Dokumen Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Format Dokumen Portabel Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "Presentasi PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "Dokumen Teks"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Spreadsheet Microsoft Excel Open XML"
  

---