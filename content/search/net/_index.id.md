---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: id
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Perpustakaan Pencarian dan Pengindeksan Dokumen .NET untuk PDF, File Office, dan Lainnya"
head_description: "Solusi .NET yang kuat untuk pencarian teks dan pengindeksan dalam dokumen seperti PDF, Word, Excel, presentasi, email, dan format web."

############################# Header ############################
title: "Pencarian dan Pengindeksan Dokumen Lanjutan dengan API .NET"
description: "Tingkatkan aplikasi .NET dengan kemampuan pencarian teks canggih di berbagai format dokumen populer."
words:
  for: "untuk"

actions:
  main: "Unduh Nuget Secara Gratis"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Lisensi"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Mulai Perjalanan Anda Hari Ini!"
  description: "Jelajahi kemampuan GroupDocs.Search secara gratis atau amankan lisensi untuk membuka potensi penuhnya."

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Cari Teks di File Direktori"
  more: "Contoh lebih banyak"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Buat indeks untuk dokumen Anda
    Index index = new Index("c:/MyIndex");

    // Tambahkan dokumen ke indeks untuk pencarian yang efisien
    index.Add("c:/MyDocuments");
    
    // Cari kata atau frasa tertentu, seperti
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Ikhtisar GroupDocs.Search"
  description: "Jelajahi perpustakaan .NET C# untuk pencarian teks dan pengindeksan yang kuat."
  features:
    # feature loop
    - title: "Fitur Pengindeksan dan Pencarian .NET"
      content: "Secara efisien indeks, simpan, dan proses data dokumen dengan GroupDocs.Search for .NET untuk operasi pencarian yang sangat akurat dan cepat."

    # feature loop
    - title: "Gabungkan Indeks untuk Kecepatan Pencarian yang Lebih Baik"
      content: "GroupDocs.Search for .NET memungkinkan Anda menggabungkan beberapa indeks untuk mengoptimalkan kinerja. Kurangi dampak indeks delta dengan menggabungkannya menjadi satu indeks komprehensif untuk pencarian yang lebih lancar."

    # feature loop
    - title: "Cari Di Seluruh Layout Keyboard yang Berbeda"
      content: "Dengan mudah menangani kueri pencarian di lebih dari 88 bahasa dan 164 layout keyboard dengan pengenalan cerdas GroupDocs.Search for .NET."

    # feature loop
    - title: "Pencarian Kata Morfologi"
      content: "GroupDocs.Search for .NET mendukung pencarian variasi kata seperti kata benda tunggal/jamak dan berbagai bentuk kata kerja, dapat disesuaikan untuk berbagai bahasa."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi Platform"
  description: "GroupDocs.Search for .NET berfungsi dengan lancar di semua sistem operasi dan pengelola paket utama."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    Proses berbagai format file dengan GroupDocs.Search for .NET. [Lihat semua format yang didukung](https://docs.groupdocs.com/search/net/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Format Kantor Populer
        * **Portabel:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Teks:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Format Media
        * **Format gambar populer:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Gambar multi-halaman:** GIF, WEBP, TIFF
        * **Audio:** MP3, WAV
        * **Video:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Lainnya
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Lainnya:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Fitur Utama dari GroupDocs.Search for .NET"
  description: "Permudah manajemen dokumen dengan kemampuan pencarian canggih dalam format populer seperti PDF, DOCX, XLSX, PPTX, dan lainnya."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parameter Pencarian yang Fleksibel"
      content: "Gunakan filter seperti rentang tanggal dan sensitivitas huruf untuk memperbaiki pencarian Anda."

    # feature loop
    - icon: "detect"
      title: "Pemeriksaan Ejaan Cerdas"
      content: "Cari frasa dengan koreksi ejaan, wildcard, dan karakter khusus yang diabaikan."

    # feature loop
    - icon: "collect"
      title: "Hasil Pencarian yang Difilter"
      content: "Sesuaikan dan filter hasil pencarian berdasarkan jenis dokumen atau kriteria."

    # feature loop
    - icon: "get"
      title: "Impor & Ekspor Indeks"
      content: "Impor data, ubah pengaturan pengindeksan, dan ekspor hasil yang diindeks."

    # feature loop
    - icon: "remove"
      title: "Pengecualian Data yang Tidak Relevan"
      content: "Optimalkan pengindeksan dengan melewatkan file atau kata tertentu."

    # feature loop
    - icon: "style"
      title: "Ekstraksi URL"
      content: "Ubah teks yang diformat HTML menjadi file dan buat tautan untuk hasil pencarian."

    # feature loop
    - icon: "detect"
      title: "Pencarian Kecepatan Tinggi"
      content: "Bagi indeks besar menjadi bagian yang lebih kecil untuk pemrosesan yang lebih cepat."

    # feature loop
    - icon: "manipulate"
      title: "Penanganan Data yang Efisien"
      content: "Indeks dokumen langsung dari aliran dan struktur data."

    # feature loop
    - icon: "compare"
      title: "Deteksi Kesalahan Pengetikan"
      content: "Usulkan kata alternatif dan lacak kemunculan untuk meningkatkan akurasi."

    # feature loop
    - icon: "unreadable_characters"
      title: "Dukungan Arsip"
      content: "Indeks arsip ZIP bersarang dan ambil detail file di dalamnya."

    # feature loop
    - icon: "hidden_print"
      title: "Pengindeksan yang Efisien"
      content: "Hemat ruang disk dengan pengindeksan yang ringkas dan proses dokumen yang dilindungi kata sandi."

    # feature loop
    - icon: "style"
      title: "Sinonim Kustom"
      content: "Tambah dan kelola sinonim untuk hasil pencarian yang disesuaikan."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Temukan kemampuan kuat GroupDocs.Search for .NET dengan contoh praktis."
  items:
    # code sample loop
    - title: "Tingkatkan Produktivitas dengan Pencarian Fuzzy"
      content: |
        Manfaatkan GroupDocs.Search for .NET untuk kontrol konten yang fleksibel dan akurat melalui algoritma pencarian canggih. [Jelajahi lebih lanjut](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Cara mengolah hasil pencarian">}}
        ```csharp {style=abap}
        // Buat indeks
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Atur opsi pencarian
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Cari dokumen yang mengandung kata 'air' atau frasa 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Proses hasil pencarian
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Pencarian Lanjutan dengan Ekspresi Reguler"
      content: |
        GroupDocs.Search for .NET mendukung ekspresi reguler untuk pencarian yang tepat. [Pelajari teknik lanjutan](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Cara mencari menggunakan ekspresi reguler">}}
        ```csharp {style=abap}   
        // Buat indeks
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Cari frasa dalam bentuk teks

        // Karakter caret pertama di awal menunjukkan bahwa ini adalah kueri pencarian ekspresi reguler
        string query = "^^(.)\\1{1,}";
        // Cari dua atau lebih karakter yang identik di awal kata
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
