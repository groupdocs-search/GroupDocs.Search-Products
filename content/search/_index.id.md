---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: id

############################# Head ############################
head_title: "Pencarian Teks dan Pengindeksan Dokumen | API & Aplikasi Web Gratis"
head_description: "Lakukan pencarian teks yang efisien dan pengindeksan data pada PDF, MS Office, OpenDocument, dan format file populer lainnya menggunakan API kami atau aplikasi Pencarian Dokumen online gratis."

############################# Header ############################
title: "Solusi Pencarian dan Pengindeksan Dokumen yang Komprehensif"
description:  |
  Lakukan pencarian teks dan pengindeksan pada PDF, Microsoft Office, OpenOffice, dan banyak format file dokumen lainnya.

  Temukan informasi dengan cepat dalam koleksi dokumen besar menggunakan kemampuan pencarian teks penuh yang canggih.

  Sesuaikan fitur pencarian seperti sinonim, pencarian fuzzy, dan stemming untuk meningkatkan akurasi dan hasil.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Pilih platform Anda"
  title: "Independensi Platform"
  description: "GroupDocs.Search kompatibel dengan sistem operasi dan kerangka kerja berikut:"
  details_link_title: "Pelajari lebih lanjut"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Editor teks lainnya
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Fitur Utama dari GroupDocs.Search"
  description: "GroupDocs.Search menyediakan alat yang kuat untuk pengindeksan dan pencarian teks dalam format dokumen populer. Permudah dan tingkatkan manajemen dokumen dengan fungsionalitas pencarian canggih."

  items:
    # items loop
    - icon: "view"
      title: "Pencarian teks yang canggih"
      content: "Lakukan pencarian teks yang cepat dan akurat di seluruh dokumen yang diindeks."

    # items loop
    - icon: "manipulate"
      title: "Opsi pencarian yang dapat disesuaikan"
      content: "Manfaatkan fitur seperti pencarian fuzzy, sinonim, dan stemming untuk hasil yang lebih tepat."

    # items loop
    - icon: "merge"
      title: "Dukungan untuk berbagai format"
      content: "Indeks dan cari konten dalam Microsoft Office, PDF, OpenOffice, dan format umum lainnya."

    # items loop
    - icon: "additional"
      title: "Pengindeksan yang efisien"
      content: "Dengan cepat membangun dan memelihara indeks untuk koleksi dokumen besar."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Mencari teks dalam format dokumen populer"
  description: "GroupDocs.Search contoh kode"
  items:
    # code sample loop
    - title: "Pencarian Teks"
      content: |
       GroupDocs.Search adalah alat yang kuat untuk menemukan teks dalam dokumen. Anda dapat mencari melalui beberapa dokumen dalam berbagai format yang disimpan dalam folder tertentu. Hasil pencarian disimpan dalam folder terpisah, memungkinkan Anda untuk mengakses dan menggunakannya kembali tanpa melakukan pencarian lagi.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Buat instansi dari kelas Index, tentukan folder untuk menyimpan indeks.
            Index index = new Index("\\Index Folder");

            //Tentukan jalur ke dokumen di mana pencarian akan dilakukan.
            index.Add("\\Documents Folder");

            //Buat instansi dari objek SearchOptions.
            SearchOptions options = new SearchOptions();

            //Lakukan pencarian untuk teks yang diinginkan.
            SearchResult result = index.Search("ipsum dolor", options);

            //Tangani dan proses hasil pencarian.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Buat instansi dari kelas Index, tentukan folder untuk menyimpan indeks.
            Index index = new Index("\\Index Folder");

            //Tentukan jalur ke dokumen di mana pencarian akan dilakukan.
            index.add("\\Documents Folder");

            //Buat instansi dari objek SearchOptions.
            SearchOptions options = new SearchOptions();

            //Lakukan pencarian untuk teks yang diinginkan.
            SearchResult result = index.search("ipsum dolor", options);

            //Tangani dan proses hasil pencarian.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Buat instansi dari kelas Index, tentukan folder untuk menyimpan indeks.
            const index = new searchLib.Index('\\Index Folder');

            //Tentukan jalur ke dokumen di mana pencarian akan dilakukan.
            index.add('\\Documents Folder');

            //Buat instansi dari objek SearchOptions.
            const options = new searchLib.SearchOptions();

            //Lakukan pencarian untuk teks yang diinginkan.
            const result = index.search('ipsum dolor', options);

            //Tangani dan proses hasil pencarian.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Mendukung 70+ format file"
  description: "GroupDocs.Search mendukung hampir semua format file yang umum digunakan"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Statistik Produk Kami"
  description: "Temukan metrik kunci yang menunjukkan kinerja, jangkauan, dan pertumbuhan kami."

  items:
    # items loop
    - number: "70+"
      title: "Format yang Didukung"
      content: "Kami menyediakan kompatibilitas dengan lebih dari 70 format dokumen populer."

    # items loop
    - number: "500k"
      title: "Unduhan NuGet"
      content: "GroupDocs.Search untuk .NET telah diunduh lebih dari 500.000 kali di NuGet."

    # items loop
    - number: "12k"
      title: "Unduhan Maven"
      content: "Pengembang Java telah mengunduh GroupDocs.Search lebih dari 12.000 kali dari Maven."

    # items loop
    - number: "150+"
      title: "Pelanggan yang Puas"
      content: "Pengembang dan bisnis terkemuka di seluruh dunia mengandalkan produk kami untuk solusi yang inovatif."


############################# Customers ###############################
customers:
  enable: true
  title: "Pelanggan Kami yang Puas"
  description: "Perpustakaan GroupDocs dipercaya oleh merek dan organisasi terkemuka di seluruh dunia."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "Mulai Perjalanan Anda Hari Ini!"
  description: "Rasakan GroupDocs.Search secara gratis di platform pilihan Anda."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Pertanyaan yang Sering Diajukan"
  description: "Temukan jawaban atas pertanyaan umum tentang GroupDocs.Search."

  items:
    # items loop
    - question: "Apakah GroupDocs.Search memerlukan alat eksternal untuk mencari dokumen?"
      answer: "Tidak, GroupDocs.Search berfungsi sebagai solusi mandiri dan tidak memerlukan alat atau perangkat lunak tambahan seperti Adobe Acrobat atau Microsoft Office untuk melakukan pencarian."

    # items loop
    - question: "Bisakah saya menguji GroupDocs.Search sebelum membeli?"
      answer: "Ya, Anda bisa! GroupDocs.Search menawarkan uji coba gratis. Anda dapat menjelajahi fitur-fiturnya, meskipun versi uji coba mungkin menyertakan batasan seperti watermark atau fungsi yang terbatas. Untuk membuka semua fitur, Anda dapat meminta lisensi sementara gratis selama 30 hari. Pelajari lebih lanjut di halaman [lisensi sementara](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "Opsi lisensi apa yang tersedia?"
      answer: "Kami menyediakan beberapa model lisensi untuk GroupDocs.Search, yang disesuaikan dengan berbagai kebutuhan. Pilih lisensi berdasarkan ukuran tim Anda, skenario penggunaan, atau apakah Anda memerlukan SDK/API untuk distribusi klien. Untuk penggunaan yang fleksibel, pertimbangkan lisensi terukur di mana Anda membayar berdasarkan penggunaan aktual. Pelajari lebih lanjut tentang pilihan Anda di halaman [harga](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Aplikasi Web"
  description: "Jelajahi GroupDocs.Search dengan aplikasi web gratis kami. Lakukan pencarian teks dan pengindeksan di lebih dari 70 format file populer langsung di browser Anda—sepenuhnya gratis."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Cari dalam PDF, Excel, Word, PowerPoint, dan jenis file lainnya langsung dari browser web Anda."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Unggah DOCX untuk melakukan pencarian teks lanjutan tanpa perlu menginstal perangkat lunak."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Uji kemampuan pengindeksan dan pengambilan PDF pada berbagai format secara gratis."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---