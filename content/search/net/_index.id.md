---
layout: "product"
date: 2022-07-07T12:44:18+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

head_title: "C# .NET Text Search & Indexing API untuk Word Excel PDF Email HTML"
head_description: "API pencarian teks C# .NET untuk mengindeks & mengambil data dengan cerdas dari PDF, Microsoft Office Word, Excel, presentasi, OneNote, Email, ZIP, EPUB & file web."

title: ".NET API untuk Mencari & Mengindeks Dokumen"
description: "API untuk Mengindeks Data & Melakukan Pencarian Teks di semua Format Dokumen Populer menggunakan Aplikasi .NET."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-net.png"
        product: "GroupDocs.Search"
        platform: ".NET"

    middle:
        button:
            - link: "#overview"
              text: "Ringkasan"

            - link: "#features"
              text: "Fitur"

            - link: "#support"
              text: "Mendukung"

            - link: "https://products.groupdocs.app/search"
              text: "Demo Langsung"

            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "Harga"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Search for .NET adalah API pencarian dokumen dan teks untuk aplikasi bisnis yang dikembangkan di C#, ASP.NET dan teknologi .NET lainnya. .NET API ini mendukung fitur pencarian dasar hingga lanjutan, misalnya, pembuatan dan penggabungan beberapa indeks, pencarian melalui indeks menggunakan Simple, Boolean, Fuzzy, Regular Expression (regex) dan jenis kueri lainnya untuk mengambil data yang Anda perlukan, dari file, dokumen, dan email, melalui pencarian cerdas. Jika Anda ingin membangun aplikasi pencarian yang cepat, andal, cerdas dan kaya fitur untuk pengguna akhir Anda, mendukung semua format file populer, GroupDocs.Search untuk .NET adalah semua yang Anda butuhkan.
    tabs:
      enable: true
      
      tab_one:
        description: |
          Berikut ini adalah ikhtisar GroupDocs.Search untuk .NET:
      
        left:
          enable: true
          icon: "fas fa-search"
          title: "Pengindeksan"
          content: |
            * Buat & Kelola
            * Gabungkan Beberapa Indeks
            * Pengindeksan Async Multi-Threading
            * Pengindeksan Ringkas
            * Pengindeksan File yang Diarsipkan
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "Pencarian Lanjutan & Kueri Pencarian"
          content: |
            * Pencarian Fuzzy
            * Pencarian Sinonim
            * Pencarian Email
            * Penanganan Istilah Homophonic
            * Mencari File yang Dilindungi
            * Sederhana
            * Kartu Liar
            * Ekspresi Reguler (Regex)
            * Segi & Boolean
            * Hal - hal sensitif
      
      tab_two:
        description: |
          GroupDocs.Search untuk .NET mendukung [format file dokumen] berikut (https://docs.groupdocs.com/search/net/supported-document-formats/):

        left:
          enable: true
          table:
            - title: "Format Microsoft Office"
              content: |
                * **Kata**: DOC, DOCX, DOCM, DOT, DOTX, DOTM
                * **Excel**: XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
                * **PowerPoint**: PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
                * **Proyek**: MPP
                * **Diagram**: VSD, VSS
                * **Microsoft Compiled HTML**: CHM
                * **OneNote**: SATU

        right:
          enable: true
          table:
            - title: "OpenDocument & Format Lainnya"
              content: |
                * **Format Dokumen Portabel**: PDF
                * **OpenDocument**: ODT, OTT, ODS, OTS, ODP
                * **Email**: PST, OST, MSG, EML, EMLX
                * **Format File Web**: XML, HTM, HTML, XHTML, MHT, MHTML
                * **Audio**: MP3, WAV
                * **Video**: AVI, MOV, QT, FLV, ASF
                * **Teks**: TXT
                * **Format Teks Kaya**: RTF
                * **File Dokumentasi Penurunan Harga**: MD
                * **Gambar**: BMP, GIF, JP2, PNG, WEBP, TIFF, EMF, WMF, JPG, PSD
                * **Lainnya**: TORRENT, ZIP, DCM, DJVU, EPUB, FB2

      tab_three:
        description: |
          GroupDocs.Search untuk .NET mendukung Sistem Operasi, Kerangka & Manajer Paket berikut:
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "Sistem operasi"
              content: |
                * Desktop Windows
                * Windows Server
                * Windows Azure
                * Linux

            - icon: "fas fa-code"
              title: "Kerangka yang Didukung"
              content: |
                * .NET Framework 2.0 atau lebih tinggi
                * Kerangka Mono 1.2 atau lebih tinggi
                * .NET Standar 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "Manajer Paket"
              content: |
                * NuGet

            - icon: "fas fa-tools"
              title: "Lingkungan Pengembangan"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

features:
    enable: true
    title: "GroupDocs.Search for .NET Features"

    feature:
      - icon: "fas fa-copy"
        content: "Buat Indeks di Memori atau di Disk & Lakukan Pengindeksan & Penggabungan Multi-utas"

      - icon: "fas fa-eye"
        content: "Cegah Pengindeksan untuk File yang Sudah Diindeks atau dengan String Tertentu di Namanya"

      - icon: "fas fa-bolt"
        content: "Lihat Persentase Kemajuan Pembuatan dan Pembaruan Indeks & Dapatkan Laporan Pencarian"
      
      - icon: "fas fa-file-powerpoint"
        content: "Pengindeksan Lebih Cepat dengan Mengecualikan Kata Tertentu & Pemberitahuan Status Indeks untuk File yang Baru Diproses"

      - icon: "fas fa-code"
        content: "Indeks Arsip ZIP dalam Arsip ZIP & Dapatkan Daftar File Terindeks yang terdapat dalam Arsip"

      - icon: "fas fa-cloud"
        content: "Gunakan Daftar atau Impor untuk Mengganti Karakter selama Pengindeksan & Ekspor ke File"

      - icon: "fas fa-remove-format"
        content: "Indeks & Cari File yang Dilindungi Kata Sandi & Pengindeksan Ringkas untuk Menghemat Ruang Disk"

      - icon: "fas fa-comment-slash"
        content: "Ekstrak Teks dari Indeks atau File Sumber & Secara Otomatis Simpan Pengkodean File Teks di Indeks"

      - icon: "fas fa-location-arrow"
        content: "Tambahkan Bidang Tambahan Sewenang-wenang ke setiap Dokumen selama Pengindeksan"

      - icon: "fas fa-border-all"
        content: "Siapkan Pemfilteran Dokumen di Hasil Pencarian"

      - icon: "fas fa-wrench"
        content: "Tangani Kesalahan Pengetikan melalui Pencarian Fuzzy, Tetapkan Tingkat Kesamaan di Pencarian Fuzzy & Tampilkan Hasil Terbaik Saja"

      - icon: "fas fa-columns"
        content: "Mengindeks Dokumen dari Aliran dan Struktur Data"

      - icon: "fas fa-file-word"
        content: "Cari Frasa Lengkap dengan Stop Words dan Gabungkan Faceted Search dengan Boolean Search"

      - icon: "fas fa-envelope"
        content: "Cari berdasarkan Istilah Homofonik, Sinonim, Rentang Tanggal, Kartu Liar & Sensitivitas Huruf"

      - icon: "fas fa-print"
        content: "Indeks & Cari Email dari Outlook & Jelajahi menggunakan Aspose.Email API"

      - icon: "fas fa-file-archive"
        content: "Mendukung Pemeriksaan Ejaan & Kartu Liar di Kueri Pencarian & Lewati Karakter Khusus di Frasa Pencarian"

      - icon: "fas fa-lock"
        content: "Batasi Hasil untuk Setiap Istilah dalam Kueri Penelusuran serta untuk Semua Hasil"

      - icon: "fas fa-file-code"
        content: "Ekstrak Teks HTML ke File & Hasilkan URL untuk Menavigasi Hasil Pencarian Berformat HTML"
      
      - icon: "fas fa-fill-drip"
        content: "Gabungkan Beberapa Kueri menjadi Pohon Objek Tunggal"

      - icon: "fas fa-file-excel"
        content: "Peringatkan Pengguna untuk Pengaturan Non-Mendukung & Pemuatan Ulang Indeks Otomatis jika terjadi Kesalahan Pengindeksan"

      - icon: "fas fa-heading"
        content: "Aktifkan Jumlah Tepat Kejadian untuk setiap Kata yang Ditemukan untuk Menawarkan Saran Kata Alternatif jika terjadi Salah Eja"

      - icon: "fas fa-project-diagram"
        content: "Tambahkan Atribut Teks ke Dokumen yang Diindeks tanpa Pengindeksan Ulang"

      - icon: "fas fa-cube"
        content: "Lakukan Pengindeksan dan Operasi Pencarian Berdasarkan Karakter"

      - icon: "fab fa-uncharted"
        content: "Metadata Indeks Format Dokumen Non-Tekstual"

    more_feature:
      - title: "Pengindeksan & Pencarian"
        content: |
          GroupDocs.Search untuk .NET API sering menggunakan indeks untuk melakukan pencarian. Indeks digunakan untuk mengumpulkan, mengurai, atau menyimpan data untuk pencarian yang cepat dan akurat.

          * **Buat Indeks**: Buat folder Indeks dan tambahkan/indeks dokumen ke folder itu.
          * **Muat Indeks**: Muat Indeks yang ada.
          * **Tambahkan Dokumen ke Indeks**: Tambahkan dokumen ke Indeks yang ada, secara asinkron.
          * **Perbarui Indeks**: Perbarui Indeks yang ada, setiap kali dokumen diubah, ditambahkan, atau dihapus. Ini membuat hasil pencarian tetap up to date.

          ```cs
           // Buat indeks
          Index  index = new Index(@"c:\MyIndex");
          // Tambahkan dokumen ke indeks
          index.AddToIndex(@"c:\MyDocuments");
          // Cari di indeks
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      - title: "Gabungkan Beberapa Indeks untuk Meningkatkan Efisiensi Pencarian"
        content: "GroupDocs.Search untuk .NET mampu menggabungkan beberapa indeks menjadi indeks tunggal. Jika indeks sering diperbarui, ia memiliki beberapa indeks delta, tetapi pendekatan ini mengurangi kinerja pencarian. GroupDocs.Search untuk .NET API menggabungkan semua indeks delta menjadi satu indeks gabungan. Indeks gabungan utama akan berisi semua informasi dari indeks delta gabungan; namun, indeks delta akan tetap tidak berubah. Pendekatan yang digunakan oleh API kami ini sangat meningkatkan efisiensi pencarian. Fitur penggabungan indeks, menyediakan banyak fungsi untuk men-tweak untuk lebih men-tweak proses ini."

      - title: "Simpan Teks dalam Indeks untuk Menghasilkan Markup HTML"
        content: "GroupDocs.Search untuk .NET dapat menyimpan teks dari dokumen yang diindeks dalam indeks. Teks yang di-cache ini kemudian digunakan untuk menghasilkan markup HTML dengan cepat dengan menyorot hasil pencarian. Pendekatan ini jauh lebih cepat daripada mengekstrak teks langsung dari file. Mengambil teks dari cache akan tersedia bahkan jika file sumber tidak lagi tersedia. Teks yang di-cache dapat disimpan dengan menerapkan berbagai tingkat kompresi untuk menempati ruang disk yang lebih sedikit dan waktu pengindeksan yang lebih cepat."

      - title: "Dapatkan Dokumen Terkait dengan Pencarian Fuzzy & Regex"
        content: "Saat Anda melakukan pencarian Fuzzy atau Regex, Anda bisa mendapatkan daftar dokumen yang sama persis dengan input yang Anda berikan. Namun, Anda juga akan mendapatkan daftar dokumen yang berisi kata atau istilah yang mirip dengan input Anda. Misalnya, jika menggunakan GroupDocs.Search untuk .NET, Anda melakukan pencarian fuzzy untuk kueri biaya, Anda akan mendapatkan dokumen yang berisi kata biaya dan dokumen yang berisi kata serupa seperti mantel. Hasilnya akan tergantung pada tingkat ketidakjelasan yang telah Anda konfigurasikan menggunakan API ini."

      - title: "Kenali Kueri Pencarian dari Tata Letak Keyboard yang Berbeda"
        content: "GroupDocs.Search for .Net dapat mengenali kueri penelusuran yang ditulis dalam bahasa yang tidak cocok dengan tata letak keyboard Anda. Saat ini, .NET API ini berhasil mengenali 88 bahasa dan 164 tata letak keyboard yang berbeda."

      - title: "Cari Menggunakan Bentuk Kata Morfologis"
        content: "GroupDocs.Search for .NET API memungkinkan Anda mencari berbagai bentuk kata. Misalnya, untuk kata benda Anda dapat mencari bentuk tunggal dan jamaknya. Untuk kata kerja, Anda dapat mencari semua bentuk kata kerja tersebut. Anda juga dapat mencari root, third-person singular, simple past dan berbagai bentuk lainnya. Untuk bahasa selain bahasa Inggris, Anda dapat menerapkan bentuk kata yang disesuaikan."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Search menawarkan API tampilan dokumen untuk lingkungan pengembangan populer lainnya"

    solution:
        - img_alt: "GroupDocs.Search for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-java.png"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

back_to_top:
  enable: true
---
