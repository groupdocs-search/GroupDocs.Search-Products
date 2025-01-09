---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
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
head_title: "Perpustakaan Pencarian & Pengindeksan Teks Node.js untuk Dokumen, PDF, Office & Web"
head_description: "Solusi pencarian teks canggih untuk aplikasi Node.js untuk mencari, mengindeks & mengumpulkan data dari dokumen: PDF, Word, Excel, presentasi, email & format file web."

############################# Header ############################
title: "Cari & Indeks Dokumen menggunakan API Node.js"
description: "Tingkatkan Aplikasi Node.js dengan mengimplementasikan Pencarian Teks di Semua Format Dokumen Populer."
words:
  for: "untuk"

actions:
  main: "Unduh NPM Secara Gratis"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "Lisensi"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "Mulai Perjalanan Anda Hari Ini!"
  description: "Jelajahi kemampuan GroupDocs.Search secara gratis atau amankan lisensi untuk membuka potensi penuhnya."

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "Lakukan Pencarian Teks di Folder dengan JavaScript"
  more: "Contoh lebih banyak"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // Buat indeks untuk dokumen Anda
    const index = new searchLib.Index('c:/MyIndex');

    // Tambahkan dokumen ke indeks untuk pencarian yang efisien
    index.add('c:/MyDocuments');
    
    // Cari kata atau frasa tertentu, seperti
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Ikhtisar GroupDocs.Search"
  description: "Perpustakaan Node.js JavaScript untuk pencarian teks"
  features:
    # feature loop
    - title: "Operasi Pengindeksan dan Pencarian Node.js"
      content: "Pengindeksan di GroupDocs.Search for Node.js via Java mengumpulkan, menyimpan, dan mem-parsing data untuk operasi pencarian yang tepat dan efisien. Indeks ini sering digunakan untuk melakukan pencarian."

    # feature loop
    - title: "Gabungkan Beberapa Indeks untuk Meningkatkan Efisiensi Pencarian"
      content: "API GroupDocs.Search for Node.js via Java memungkinkan penggabungan beberapa indeks menjadi satu. Modifikasi yang sering menciptakan beberapa indeks delta, yang dapat memperlambat kinerja pencarian. Solusi kami menggabungkan indeks delta ini menjadi indeks umum yang berisi semua informasi dari indeks delta yang digabungkan, secara signifikan meningkatkan efisiensi pencarian sambil menjaga indeks delta tidak berubah. Berbagai fungsionalitas dapat dikonfigurasi untuk menyempurnakan proses ini."

    # feature loop
    - title: "Mengenali Kueri Pencarian dari Berbagai Layout Keyboard"
      content: "GroupDocs.Search for Node.js via Java mengenali kueri pencarian yang tidak sesuai dengan layout keyboard. Saat ini, 88 bahasa dan 164 layout keyboard yang berbeda didukung."

    # feature loop
    - title: "Cari Menggunakan Bentuk Kata Morfologi"
      content: "Dengan GroupDocs.Search for Node.js via Java, Anda dapat mencari berbagai bentuk kata, seperti kata benda tunggal dan jamak, atau semua bentuk kata kerja. Bahasa Inggris dan bahasa non-Inggris dapat disesuaikan untuk bentuk kata tertentu."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi Platform"
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
    GroupDocs.Search for Node.js via Java memungkinkan pengolahan berbagai format file. [Jelajahi daftar lengkapnya](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/).
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
  title: "GroupDocs.Search for Node.js via Java Fitur"
  description: "Kontrol konten dokumen bisnis menggunakan mesin pencarian canggih kami, mendukung format file populer termasuk PDF, DOCX, XLSX, PPTX, dan lainnya."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parameter yang Fleksibel"
      content: "Gunakan Rentang Tanggal & Sensitivitas Huruf sebagai Parameter Pencarian"

    # feature loop
    - icon: "detect"
      title: "Pencarian Pemeriksaan Ejaan"
      content: "Gunakan Frasa Pencarian dengan Pemeriksaan Ejaan dan Wildcard & Lewati Karakter Khusus dalam Kueri"

    # feature loop
    - icon: "collect"
      title: "Penyaringan Hasil"
      content: "Siapkan Penyaringan Dokumen dalam Hasil Pencarian"

    # feature loop
    - icon: "get"
      title: "Impor & Ekspor"
      content: "Lakukan Impor atau Gunakan Daftar untuk Memodifikasi Karakter saat Pengindeksan & Ekspor ke File"

    # feature loop
    - icon: "remove"
      title: "Lewati Data yang Tidak Perlu"
      content: "Pilih untuk Melewati Pengindeksan untuk File Tertentu & Lewati Kata Tertentu untuk Mengindeks Lebih Cepat"

    # feature loop
    - icon: "style"
      title: "Pemrosesan URL"
      content: "Ekstrak Teks yang Diformat HTML ke File & Buat URL untuk Menavigasi Hasil Pencarian dalam HTML"

    # feature loop
    - icon: "detect"
      title: "Pencarian Cepat"
      content: "Bagi Pencarian ke dalam Chunks yang Lebih Kecil untuk Segera Mencari Indeks Besar"

    # feature loop
    - icon: "manipulate"
      title: "Pemrosesan Aliran"
      content: "Indeks Dokumen dari Aliran dan Struktur Data"

    # feature loop
    - icon: "compare"
      title: "Tangani Kesalahan Ejaan"
      content: "Aktifkan Jumlah Kemunculan yang Tepat untuk Setiap Kata yang Ditemukan untuk Menawarkan Saran Kata Alternatif jika Terjadi Kesalahan Ejaan"

    # feature loop
    - icon: "unreadable_characters"
      title: "Dukungan Arsip"
      content: "Indeks Arsip ZIP yang Terletak di Dalam Arsip ZIP Lainnya & Ambil Daftar File yang Diindeks di Dalam Arsip"

    # feature loop
    - icon: "hidden_print"
      title: "Penghematan Ruang Disk"
      content: "Hemat Ruang dengan Pengindeksan Ringkas & Indeks Dokumen yang Dilindungi Kata Sandi"

    # feature loop
    - icon: "style"
      title: "Sinonim Kustom"
      content: "Tambahkan Sinonim Bahasa Inggris ke Kamus Sinonim Default"

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Jelajahi fungsionalitas GroupDocs.Search for Node.js via Java dengan contoh"
  items:
    # code sample loop
    - title: "Gunakan pencarian 'fuzzy' untuk meningkatkan produktivitas"
      content: |
        Nikmati fungsionalitas GroupDocs.Search for Node.js via Java yang fleksibel untuk meningkatkan kontrol konten dokumen melalui algoritma pencarian yang canggih. [Pelajari lebih lanjut](https://docs.groupdocs.com/search/nodejs-java/search-results/).
        {{< landing/code title="Cara mengolah hasil pencarian">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // Buat indeks
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // Atur opsi pencarian
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Cari dokumen yang mengandung kata 'air' atau frasa 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // Proses hasil pencarian
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Ekspresi reguler tersedia untuk skenario pencarian yang canggih"
      content: |
        GroupDocs.Search for Node.js via Java memungkinkan kita menggunakan ekspresi reguler untuk mempersempit hasil pencarian. [Selami teknik pencarian lanjutan](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/).
        {{< landing/code title="Cara mencari menggunakan ekspresi reguler">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // Buat indeks
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // Cari frasa dalam bentuk teks

        // Karakter caret pertama di awal menunjukkan bahwa ini adalah kueri pencarian ekspresi reguler
        const query = '^^(.)\\1{1,}';
        // Cari dua atau lebih karakter yang identik di awal kata
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
