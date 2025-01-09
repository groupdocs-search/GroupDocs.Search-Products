---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: id
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

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
head_title: "Solusi Pencarian & Pengindeksan Dokumen Java untuk PDF, File Office, dan Konten Web"
head_description: "Pencarian teks dan pengindeksan yang kuat untuk aplikasi Java. Dengan mudah mencari dan mengorganisir data di PDF, Word, Excel, presentasi, email, dan format web."

############################# Header ############################
title: "Pencarian dan Pengindeksan Dokumen yang Efisien dengan API Java"
description: "Memberdayakan aplikasi Java dengan fitur pencarian teks yang kuat di semua format dokumen populer."
words:
  for: "untuk"

actions:
  main: "Unduh Maven Secara Gratis"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Lisensi"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Mulai Perjalanan Anda Hari Ini!"
  description: "Jelajahi kemampuan GroupDocs.Search secara gratis atau amankan lisensi untuk membuka potensi penuhnya."

release:
  title: "Versi {0} dirilis"
  notes: "Lihat apa yang baru"
  downloads: "Unduhan"

code:
  title: "Temukan Teks di File Menggunakan Java"
  more: "Contoh lebih banyak"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Buat indeks untuk dokumen Anda
    Index index = new Index("c:/MyIndex");

    // Tambahkan dokumen ke indeks untuk pencarian yang efisien
    index.add("c:/MyDocuments");
    
    // Cari kata atau frasa tertentu, seperti
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "Ikhtisar GroupDocs.Search"
  description: "Temukan kemampuan pencarian teks yang kuat dari perpustakaan Java Java."
  features:
    # feature loop
    - title: "Operasi Pengindeksan dan Pencarian di Java"
      content: "Dengan GroupDocs.Search for Java, Anda dapat mengumpulkan, menyimpan, dan menganalisis data secara efisien untuk membuat indeks yang detail untuk pencarian yang lebih cepat dan lebih akurat."

    # feature loop
    - title: "Optimalkan Pencarian dengan Menggabungkan Indeks"
      content: "Dengan mudah menggabungkan beberapa indeks menggunakan GroupDocs.Search for Java untuk menyederhanakan pencarian. Kurangi dampak dari indeks delta yang lebih kecil dengan mengkonsolidasikan mereka menjadi satu indeks berkinerja tinggi."

    # feature loop
    - title: "Dukungan untuk Layout Keyboard Multibahasa"
      content: "Cari di berbagai bahasa dan layout keyboard dengan GroupDocs.Search for Java. Ini mendukung 88 bahasa dan 164 konfigurasi keyboard untuk fleksibilitas yang tak tertandingi."

    # feature loop
    - title: "Kemampuan Pencarian Morfologi"
      content: "Temukan berbagai bentuk kata seperti kata benda tunggal/jamak atau variasi kata kerja menggunakan GroupDocs.Search for Java. Sesuaikan opsi pencarian untuk bahasa Inggris dan bahasa lainnya."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independensi Platform"
  description: "GroupDocs.Search for Java kompatibel dengan sistem operasi dan pengelola paket utama."
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Format file yang didukung"
  description: |
    Bekerja dengan berbagai format file menggunakan GroupDocs.Search for Java. [Lihat daftar lengkap](https://docs.groupdocs.com/search/java/supported-document-formats/).
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
  title: "Fitur dari GroupDocs.Search for Java"
  description: "Kelola konten dokumen secara efektif dengan kemampuan pencarian canggih yang mendukung format seperti PDF, DOCX, XLSX, PPTX, dan lainnya."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parameter Pencarian yang Dapat Disesuaikan"
      content: "Perbaiki pencarian menggunakan rentang tanggal dan filter sensitivitas huruf."

    # feature loop
    - icon: "detect"
      title: "Pemeriksaan Ejaan yang Ditingkatkan"
      content: "Cari dengan efisien menggunakan pemeriksaan ejaan, wildcard, dan dengan mengabaikan karakter khusus."

    # feature loop
    - icon: "collect"
      title: "Hasil Pencarian yang Difilter"
      content: "Terapkan filter untuk fokus pada hasil pencarian berdasarkan jenis dokumen tertentu atau kriteria."

    # feature loop
    - icon: "get"
      title: "Impor dan Ekspor Data Indeks"
      content: "Dengan mudah impor data untuk pengindeksan atau ekspor hasil ke file untuk digunakan lebih lanjut."

    # feature loop
    - icon: "remove"
      title: "Lewati File yang Tidak Diperlukan"
      content: "Optimalisasi pengindeksan dengan mengecualikan file atau kata tertentu."

    # feature loop
    - icon: "style"
      title: "Pemrosesan HTML dan URL"
      content: "Ekstrak konten HTML ke file dan buat URL untuk navigasi melalui hasil pencarian."

    # feature loop
    - icon: "detect"
      title: "Pencarian Cepat di Indeks Besar"
      content: "Percepat operasi pencarian dengan membagi indeks besar menjadi bagian yang dapat dikelola."

    # feature loop
    - icon: "manipulate"
      title: "Pengindeksan Berdasarkan Aliran"
      content: "Indeks data langsung dari aliran atau struktur data."

    # feature loop
    - icon: "compare"
      title: "Tangani Kueri yang Salah Eja"
      content: "Deteksi kesalahan pengetikan dan usulkan kata alternatif untuk akurasi pencarian yang lebih baik."

    # feature loop
    - icon: "unreadable_characters"
      title: "Dukungan Arsip yang Komprehensif"
      content: "Indeks arsip bersarang dan ambil daftar rinci file dalam file ZIP."

    # feature loop
    - icon: "hidden_print"
      title: "Pengindeksan yang Menghemat Ruang"
      content: "Indeks yang ringkas untuk menghemat ruang disk dan memproses file yang dilindungi kata sandi."

    # feature loop
    - icon: "style"
      title: "Dukungan Sinonim Kustom"
      content: "Perluas kamus sinonim untuk meningkatkan akurasi pencarian dengan opsi yang disesuaikan."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Contoh kode"
  description: "Coba fitur GroupDocs.Search for Java dengan contoh kode ini."
  items:
    # code sample loop
    - title: "Tingkatkan Akurasi Pencarian dengan Pencocokan Fuzzy"
      content: |
        Jelajahi fleksibilitas GroupDocs.Search for Java dalam mengelola konten dengan kemampuan pencarian fuzzy yang canggih. [Pelajari lebih lanjut](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Cara mengolah hasil pencarian">}}
        ```java {style=abap}
        // Buat indeks
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Atur opsi pencarian
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Cari dokumen yang mengandung kata 'air' atau frasa 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Proses hasil pencarian
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Perbaiki Hasil dengan Ekspresi Reguler"
      content: |
        Gunakan ekspresi reguler di GroupDocs.Search for Java untuk menghasilkan hasil pencarian yang tepat dan terperinci. [Temukan teknik lanjutan](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Cara mencari menggunakan ekspresi reguler">}}
        ```java {style=abap}   
        // Buat indeks
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Cari frasa dalam bentuk teks

        // Karakter caret pertama di awal menunjukkan bahwa ini adalah kueri pencarian ekspresi reguler
        String query = "^^(.)\\1{1,}";
        // Cari dua atau lebih karakter yang identik di awal kata
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
