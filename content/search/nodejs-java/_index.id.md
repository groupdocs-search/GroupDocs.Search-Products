---
############################# Static ############################
layout: "landing"
date: 2024-07-04T14:43:38
draft: false

lang: id
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js Pencarian Teks & Perpustakaan Pengindeksan untuk Dokumen, PDF, Office & Web"
head_description: "Solusi pencarian teks tingkat lanjut untuk aplikasi Node.js untuk mencari, mengindeks & mengumpulkan data dari dokumen: PDF, Word, Excel, presentasi, email & format file web."

############################# Header ############################
title: "Pencarian & Indeks Dokumen menggunakan API Node.js"
description: "Tingkatkan Aplikasi Node.js dengan menerapkan Pencarian Teks di Semua Format Dokumen Populer."
words:
  for: "untuk"

actions:
  main: "Unduh NPM Gratis"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Perizinan"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Siap untuk memulai?"
  description: "Coba fitur GroupDocs.Search secara gratis atau minta lisensi"

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Cari di folder dengan JavaScript"
  more: "Lebih banyak contoh"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // Membuat indeks
    const index = new Index('c:/MyIndex');

    // Menambahkan dokumen ke indeks
    index.add('c:/MyDocuments');
    
    // Mencari berbagai kata seperti
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search sekilas"
  description: "Pustaka Node.js JavaScript untuk pencarian teks"
  features:
    # feature loop
    - title: "Node.js Operasi Pengindeksan dan Pencarian"
      content: "Pengindeksan di GroupDocs.Search for Node.js via Java mengumpulkan, menyimpan, dan menguraikan data untuk operasi pencarian yang tepat dan efisien. Indeks ini sering digunakan untuk melakukan pencarian."

    # feature loop
    - title: "Gabungkan Beberapa Indeks untuk Meningkatkan Efisiensi Pencarian"
      content: "GroupDocs.Search for Node.js via Java API memungkinkan penggabungan beberapa indeks menjadi satu. Modifikasi yang sering dilakukan membuat beberapa indeks delta, yang dapat memperlambat kinerja pencarian. Solusi kami menggabungkan indeks delta ini menjadi indeks umum, yang berisi semua informasi dari indeks delta gabungan, sehingga secara signifikan meningkatkan efisiensi pencarian sekaligus menjaga indeks delta tidak berubah. Berbagai fungsi dapat dikonfigurasi untuk menyempurnakan proses ini."

    # feature loop
    - title: "Kenali Kueri Pencarian dari Berbagai Tata Letak Keyboard"
      content: "GroupDocs.Search for Node.js via Java mengenali kueri penelusuran yang tidak cocok dengan tata letak keyboard. Saat ini, 88 bahasa dan 164 tata letak keyboard berbeda didukung."

    # feature loop
    - title: "Pencarian Menggunakan Bentuk Kata Morfologis"
      content: "Dengan GroupDocs.Search for Node.js via Java, Anda dapat mencari berbagai bentuk kata, seperti kata benda tunggal dan jamak, atau semua bentuk kata kerja. Bahasa Inggris dan non-Inggris dapat disesuaikan untuk bentuk kata tertentu."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi platform"
  description: "GroupDocs.Search for Node.js via Java mendukung semua sistem operasi dan pengelola paket populer."
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    GroupDocs.Search for Node.js via Java memungkinkan pemrosesan berbagai format file. [Jelajahi daftar lengkapnya](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Format Office Populer
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
        * **Surel:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **jaring:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Yang lain:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java Fitur"
  description: "Kontrol konten dokumen bisnis menggunakan mesin pencari canggih kami, mendukung format file populer termasuk PDF, DOCX, XLSX, PPTX, dan banyak lagi."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parameter Fleksibel"
      content: "Gunakan Rentang Tanggal & Sensitivitas Huruf sebagai Parameter Pencarian"

    # feature loop
    - icon: "detect"
      title: "Pencarian Periksa Ejaan"
      content: "Gunakan Frasa Pencarian dengan Pemeriksaan Ejaan dan Wildcard & Lewati Karakter Khusus dalam Kueri"

    # feature loop
    - icon: "collect"
      title: "Penyaringan Hasil"
      content: "Atur Pemfilteran Dokumen di Hasil Pencarian"

    # feature loop
    - icon: "get"
      title: "Ekspor Impor"
      content: "Lakukan Impor atau Gunakan Daftar untuk Memodifikasi Karakter selama Pengindeksan & Ekspor ke File"

    # feature loop
    - icon: "remove"
      title: "Lewati Data yang Tidak Diperlukan"
      content: "Lewati Pengindeksan Secara Selektif untuk File Tertentu & Lewati Kata Tertentu untuk Mengindeks Lebih Cepat"

    # feature loop
    - icon: "style"
      title: "Pemrosesan URL"
      content: "Ekstrak Teks Berformat HTML ke File & Hasilkan URL untuk Menavigasi Hasil Pencarian dalam HTML"

    # feature loop
    - icon: "detect"
      title: "Pencarian Cepat"
      content: "Bagilah Pencarian menjadi Bagian-bagian yang Lebih Kecil untuk Mencari Indeks Besar dengan Cepat"

    # feature loop
    - icon: "manipulate"
      title: "Pemrosesan Aliran"
      content: "Dokumen Indeks dari Aliran dan Struktur Data"

    # feature loop
    - icon: "compare"
      title: "Menangani Kesalahan Ejaan"
      content: "Aktifkan Jumlah Kemunculan Tepat untuk setiap Kata yang Ditemukan untuk Menawarkan Saran Kata Alternatif jika terjadi Kesalahan Ejaan"

    # feature loop
    - icon: "unreadable_characters"
      title: "Dukungan Arsip"
      content: "Indeks Arsip ZIP di dalam Arsip ZIP lainnya & Ambil Daftar File Terindeks dalam Arsip"

    # feature loop
    - icon: "hidden_print"
      title: "Penghematan Ruang Disk"
      content: "Hemat Ruang dengan Pengindeksan Ringkas & Indeks Dokumen Terlindungi Kata Sandi"

    # feature loop
    - icon: "style"
      title: "Sinonim Khusus"
      content: "Tambahkan Sinonim Bahasa Inggris ke Kamus Sinonim Default"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Jelajahi fungsi GroupDocs.Search for Node.js via Java beserta contohnya"
  items:
    # code sample loop
    - title: "Gunakan pencarian fuzzy untuk meningkatkan produktivitas"
      content: |
        Nikmati fungsionalitas GroupDocs.Search for Node.js via Java yang fleksibel untuk meningkatkan kontrol konten dokumen melalui algoritma pencarian yang canggih. [Pelajari lebih lanjut](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Cara memproses hasil pencarian">}}
        ```javascript {style=abap}
        // Buat indeks
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Siapkan opsi pencarian
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Telusuri dokumen yang mengandung kata 'air' atau kalimat 'Lorem ipsum'
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // Proses hasil pencarian
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ekspresi reguler tersedia untuk skenario pencarian lanjutan"
      content: |
        GroupDocs.Search for Node.js via Java memungkinkan kita menggunakan ekspresi reguler untuk mempersempit hasil pencarian. [Selami teknik penelusuran lanjutan](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Cara mencari menggunakan ekspresi reguler">}}
        ```javascript {style=abap}   
        // Buat indeks
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Cari frasa dalam bentuk teks

        // Karakter tanda sisipan pertama di awal menunjukkan bahwa ini adalah kueri penelusuran ekspresi reguler
        var query = "^^(.)\\1{1,}";
        // Cari dua atau lebih karakter identik di awal kata
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
