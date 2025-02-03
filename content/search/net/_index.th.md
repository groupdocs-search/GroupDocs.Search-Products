---
############################# Static ############################
layout: "landing"
date: 2025-02-03T08:17:12
draft: false

lang: th
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
head_title: "ไลบรารีการค้นหาเอกสารและการจัดทำดัชนี .NET สำหรับ PDF, ไฟล์ Office และอื่นๆ"
head_description: "โซลูชัน .NET ที่ทรงพลังสำหรับการค้นหาและจัดทำดัชนีข้อความในเอกสารเช่น PDF, Word, Excel, การนำเสนอ, อีเมล และรูปแบบเว็บ"

############################# Header ############################
title: "การค้นหาและจัดทำดัชนีเอกสารขั้นสูงด้วย API .NET"
description: "เพิ่มประสิทธิภาพแอปพลิเคชัน .NET ด้วยความสามารถในการค้นหาข้อความที่ล้ำสมัยในรูปแบบเอกสารยอดนิยม"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลด Nuget ฟรี"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "เริ่มการเดินทางของคุณวันนี้!"
  description: "สำรวจความสามารถของ GroupDocs.Search ฟรี หรือขอใบอนุญาตเพื่อปลดล็อกศักยภาพทั้งหมด"

release:
  title: "รุ่น {0} ได้รับการเปิดตัว"
  notes: "ดูสิ่งที่ใหม่"
  downloads: "การดาวน์โหลด"

code:
  title: "ค้นหาข้อความในไฟล์ในไดเร็คทอรี"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // สร้างดัชนีสำหรับเอกสารของคุณ
    Index index = new Index("c:/MyIndex");

    // เพิ่มเอกสารลงในดัชนีเพื่อการค้นหาที่มีประสิทธิภาพ
    index.Add("c:/MyDocuments");
    
    // ค้นหาคำหรือวลีเฉพาะ เช่น
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search ภาพรวม"
  description: "สำรวจไลบรารี .NET C# สำหรับการค้นหาและจัดทำดัชนีข้อความที่แข็งแกร่ง"
  features:
    # feature loop
    - title: "ฟีเจอร์การจัดทำดัชนีและการค้นหา .NET"
      content: "จัดทำดัชนี เก็บ และประมวลผลข้อมูลเอกสารอย่างมีประสิทธิภาพด้วย GroupDocs.Search for .NET สำหรับการค้นหาที่แม่นยำและรวดเร็ว"

    # feature loop
    - title: "รวมดัชนีเพื่อความเร็วในการค้นหาที่ดีขึ้น"
      content: "GroupDocs.Search for .NET ช่วยให้คุณรวมหลายดัชนีเพื่อเพิ่มประสิทธิภาพ ลดผลกระทบของดัชนีแบบเดลต้าโดยการรวมเข้ากับดัชนีรวมเพื่อให้การค้นหาเรียบลื่นขึ้น"

    # feature loop
    - title: "ค้นหาข้ามแป้นพิมพ์ที่แตกต่างกัน"
      content: "จัดการคำค้นหาที่หลากหลายได้อย่างง่ายดายโดยมีแป้นพิมพ์ 88 ภาษาและ 164 รูปแบบ"

    # feature loop
    - title: "การค้นหาคำในรูปแบบ Morphological"
      content: "GroupDocs.Search for .NET รองรับการค้นหาคำแปรต่างๆ เช่น คำนามเอกพจน์/พหูพจน์ และรูปแบบกริยาที่แตกต่างกันสามารถปรับแต่งสำหรับภาษาที่หลากหลาย"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Search for .NET ทำงานได้อย่างราบรื่นข้ามระบบปฏิบัติการและผู้จัดการแพ็กเกจหลัก"
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
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    ประมวลผลไฟล์รูปแบบที่หลากหลายด้วย GroupDocs.Search for .NET [ดูรูปแบบที่รองรับทั้งหมด](https://docs.groupdocs.com/search/net/supported-document-formats/)
  groups:
    # group loop
    - color: "green"
      content: |
        ### รูปแบบสำนักงานยอดนิยม
        * **พกพาได้:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **ข้อความ:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### รูปแบบสื่อ
        * **รูปแบบภาพยอดนิยม:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **ภาพหลายหน้า:** GIF, WEBP, TIFF
        * **เสียง:** MP3, WAV
        * **วิดีโอ:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### อื่นๆ
        * **อีเมล:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **เว็บ:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **อื่นๆ:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "ฟีเจอร์หลักของ GroupDocs.Search for .NET"
  description: "ปรับปรุงการจัดการเอกสารด้วยความสามารถในการค้นขั้นสูงในรูปแบบยอดนิยมเช่น PDF, DOCX, XLSX, PPTX และอื่นๆ"

  items:
    # feature loop
    - icon: "document_info"
      title: "พารามิเตอร์การค้นหาที่ยืดหยุ่น"
      content: "ใช้ตัวกรองเช่น ช่วงวันที่และความไวต่ออักษรในการปรับแต่งการค้นหาของคุณ"

    # feature loop
    - icon: "detect"
      title: "การตรวจสอบการสะกดที่ชาญฉลาด"
      content: "ค้นหาวลีด้วยการแก้ไขการสะกด, ตัวอักษรแทนและการข้ามอักขระพิเศษ"

    # feature loop
    - icon: "collect"
      title: "ผลลัพธ์การค้นหาที่กรองแล้ว"
      content: "ปรับแต่งและกรองผลลัพธ์การค้นหาโดยประเภทเอกสารหรือเกณฑ์"

    # feature loop
    - icon: "get"
      title: "นำเข้าข้อมูลและส่งออก"
      content: "นำเข้าข้อมูล แก้ไขการตั้งค่าการจัดทำดัชนี และส่งออกผลลัพธ์ที่จัดทำดัชนี"

    # feature loop
    - icon: "remove"
      title: "ข้ามข้อมูลที่ไม่เกี่ยวข้อง"
      content: "เพิ่มประสิทธิภาพการจัดทำดัชนีโดยการข้ามไฟล์หรือคำเฉพาะ"

    # feature loop
    - icon: "style"
      title: "การดึง URL"
      content: "แปลงข้อความที่มีรูปแบบ HTML เป็นไฟล์และสร้างลิงก์สำหรับผลลัพธ์การค้นหา"

    # feature loop
    - icon: "detect"
      title: "การค้นหาความเร็วสูง"
      content: "แบ่งดัชนีขนาดใหญ่เป็นชิ้นเล็กๆ เพื่อการประมวลผลที่รวดเร็วขึ้น"

    # feature loop
    - icon: "manipulate"
      title: "การจัดการข้อมูลโดยตรง"
      content: "จัดทำดัชนีเอกสารโดยตรงจากสตรีมข้อมูลและโครงสร้าง"

    # feature loop
    - icon: "compare"
      title: "การตรวจจับการสะกดผิด"
      content: "เสนอคำที่เหมาะสมทางเลือกและติดตามความถี่สำหรับการปรับปรุงความแม่นยำ"

    # feature loop
    - icon: "unreadable_characters"
      title: "การสนับสนุนการจัดเก็บ"
      content: "จัดทำดัชนี ZIP ที่ซ้อนกันและเรียกดูรายละเอียดไฟล์ภายใน"

    # feature loop
    - icon: "hidden_print"
      title: "การจัดทำดัชนีที่มีประสิทธิภาพ"
      content: "ประหยัดพื้นที่ดิสก์ด้วยการจัดทำดัชนีอย่างกระชับ และจัดการเอกสารที่มีรหัสผ่าน"

    # feature loop
    - icon: "style"
      title: "คำพ้องแบบกำหนดเอง"
      content: "เพิ่มและจัดการคำพ้องเพื่อผลลัพธ์การค้นหาที่ปรับแต่ง"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "ค้นพบความสามารถที่ทรงพลังของ GroupDocs.Search for .NET ผ่านตัวอย่างปฏิบัติ"
  items:
    # code sample loop
    - title: "เพิ่มประสิทธิภาพด้วยการค้นหาแบบใกล้เคียง"
      content: |
        ใช้ประโยชน์จาก GroupDocs.Search for .NET สำหรับการควบคุมเนื้อหาที่ยืดหยุ่นและแม่นยำผ่านอัลกอริธึมการค้นหาที่ทันสมัย [ค้นคว้าเพิ่มเติม](https://docs.groupdocs.com/search/net/search-results/)
        {{< landing/code title="วิธีการจัดการผลลัพธ์การค้นหา">}}
        ```csharp {style=abap}
        // สร้างดัชนี
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // ตั้งค่าตัวเลือกการค้นหา
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // ค้นหาสำหรับเอกสารที่มีคำว่า 'น้ำ' หรือวลี 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // ประมวลผลผลลัพธ์การค้นหา
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
    - title: "การค้นหาขั้นสูงด้วย Expressions ปกติ"
      content: |
        GroupDocs.Search for .NET รองรับการค้นหาด้วย Regular Expressions สำหรับการค้นที่แม่นยำ [ศึกษาเทคนิคขั้นสูง](https://docs.groupdocs.com/search/net/regular-expression-search/)
        {{< landing/code title="วิธีการค้นหาด้วยการแสดงผลปกติ">}}
        ```csharp {style=abap}   
        // สร้างดัชนี
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // ค้นหาวลีในรูปแบบข้อความ

        // อักขระ caret ตัวแรกที่ต้นบ่งบอกว่านี่เป็นคำค้นหาที่ใช้การแสดงผลปกติ
        string query = "^^(.)\\1{1,}";
        // ค้นหาสำหรับตัวอักษรที่ซ้ำกันสองตัวหรือมากกว่าที่ต้นคำ
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
