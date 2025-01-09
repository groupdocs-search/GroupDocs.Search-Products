---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: th
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
head_title: "โซลูชันการค้นหาและจัดทำดัชนีเอกสาร Java สำหรับ PDF, ไฟล์ Office และเนื้อหาเว็บ"
head_description: "การค้นหาและจัดทำดัชนีข้อความที่ทรงพลังสำหรับแอปพลิเคชัน Java ค้นหาและจัดระเบียบข้อมูลในไฟล์ PDF, Word, Excel, การนำเสนอ, อีเมล และรูปแบบเว็บอย่างง่ายดาย"

############################# Header ############################
title: "การค้นหาเอกสารและจัดทำดัชนีอย่างมีประสิทธิภาพด้วย API Java"
description: "เพิ่มประสิทธิภาพแอปพลิเคชัน Java ด้วยคุณสมบัติการค้นหาข้อความที่ทรงพลังในรูปแบบเอกสารยอดนิยมทั้งหมด"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลด Maven ฟรี"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "เริ่มการเดินทางของคุณวันนี้!"
  description: "สำรวจความสามารถของ GroupDocs.Search ฟรี หรือขอใบอนุญาตเพื่อปลดล็อกศักยภาพทั้งหมด"

release:
  title: "รุ่น {0} ได้รับการเปิดตัว"
  notes: "ดูสิ่งที่ใหม่"
  downloads: "การดาวน์โหลด"

code:
  title: "ค้นหาข้อความในไฟล์ด้วย Java"
  more: "ตัวอย่างเพิ่มเติม"
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
    // สร้างดัชนีสำหรับเอกสารของคุณ
    Index index = new Index("c:/MyIndex");

    // เพิ่มเอกสารลงในดัชนีเพื่อการค้นหาที่มีประสิทธิภาพ
    index.add("c:/MyDocuments");
    
    // ค้นหาคำหรือวลีเฉพาะ เช่น
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search ภาพรวม"
  description: "ค้นพบความสามารถในการค้นหาข้อความที่ยอดเยี่ยมของไลบรารี Java Java"
  features:
    # feature loop
    - title: "การจัดทำดัชนีและการดำเนินการค้นหาใน Java"
      content: "ด้วย GroupDocs.Search for Java คุณสามารถรวบรวม เก็บ และวิเคราะห์ข้อมูลได้อย่างมีประสิทธิภาพเพื่อสร้างดัชนีที่มีรายละเอียดสำหรับการค้นหาที่รวดเร็วและแม่นยำยิ่งขึ้น"

    # feature loop
    - title: "เพิ่มประสิทธิภาพการค้นหาด้วยการรวมดัชนี"
      content: "คุณสามารถรวมดัชนีหลายๆ ตัวด้วย GroupDocs.Search for Java เพื่อปรับปรุงการค้นหา ลดผลกระทบของดัชนีแบบเดลต้าเล็กๆ โดยการผนวกเข้ากับดัชนีที่มีประสิทธิภาพสูง"

    # feature loop
    - title: "รองรับรูปแบบแป้นพิมพ์หลายภาษา"
      content: "ค้นหาข้ามภาษาต่างๆ และรูปแบบแป้นพิมพ์ด้วย GroupDocs.Search for Java ซึ่งรองรับ 88 ภาษา และ 164 รูปแบบการจัดเรียงแป้นพิมพ์"

    # feature loop
    - title: "ฟังก์ชันการค้นหาคำในรูปแบบ Morphological"
      content: "ค้นหาคำรูปแบบต่าง ๆ เช่น คำนามเอกพจน์/พหูพจน์หรือรูปแบบกริยาที่แตกต่างกัน ด้วย GroupDocs.Search for Java ตัวเลือกการค้นหาสามารถปรับแต่งให้เหมาะสมกับภาษาอังกฤษและภาษาดอื่น ๆ"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Search for Java รองรับระบบปฏิบัติการและผู้จัดการแพ็คเกจหลัก"
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
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    ทำงานกับไฟล์รูปแบบที่หลากหลายด้วย GroupDocs.Search for Java [ดูรายการทั้งหมด](https://docs.groupdocs.com/search/java/supported-document-formats/)
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
  title: "ฟีเจอร์ของ GroupDocs.Search for Java"
  description: "จัดการเนื้อหาของเอกสารอย่างมีประสิทธิภาพด้วยความสามารถในการค้นหาขั้นสูงที่รองรับรูปแบบต่างๆ เช่น PDF, DOCX, XLSX, PPTX และอื่นๆ"

  items:
    # feature loop
    - icon: "document_info"
      title: "พารามิเตอร์การค้นหาที่ปรับแต่งได้"
      content: "ตีกรอบการค้นหาด้วยตัวกรองช่วงวันที่และความไวต่ออักษร"

    # feature loop
    - icon: "detect"
      title: "การตรวจสอบการสะกดที่มีการปรับปรุง"
      content: "ค้นหาอย่างมีประสิทธิภาพด้วยการตรวจสอบการสะกด ตัวแทนไวลด์การ์ด และการละเว้นอักขระพิเศษ"

    # feature loop
    - icon: "collect"
      title: "ผลลัพธ์การค้นหาที่กรองแล้ว"
      content: "ใช้การกรองเพื่อลดผลลัพธ์การค้นหาตามประเภทเอกสารหรือเกณฑ์เฉพาะ"

    # feature loop
    - icon: "get"
      title: "นำเข้าข้อมูลและส่งออก"
      content: "นำเข้าข้อมูลเพื่อนำไปจัดทำดัชนีหรือส่งออกผลลัพธ์ไปยังไฟล์เพื่อการใช้งานต่อ"

    # feature loop
    - icon: "remove"
      title: "ข้ามไฟล์ที่ไม่จำเป็น"
      content: "เพิ่มประสิทธิภาพการจัดทำดัชนีโดยการละเว้นไฟล์หรือคำเฉพาะ"

    # feature loop
    - icon: "style"
      title: "การจัดการ HTML และ URL"
      content: "ดึงข้อมูล HTML ไปยังไฟล์และสร้าง URL สำหรับการเดินทางผ่านผลลัพธ์การค้นหา"

    # feature loop
    - icon: "detect"
      title: "การค้นหาอย่างรวดเร็วในดัชนีขนาดใหญ่"
      content: "เพิ่มความเร็วในการค้นหาด้วยการแบ่งดัชนีขนาดใหญ่ให้เป็นชิ้นเล็ก"

    # feature loop
    - icon: "manipulate"
      title: "การจัดทำดัชนีจากสตรีม"
      content: "จัดทำดัชนีข้อมูลโดยตรงจากสตรีมหรือโครงสร้างข้อมูล"

    # feature loop
    - icon: "compare"
      title: "จัดการคำค้นหาที่สะกดผิด"
      content: "ตรวจจับคำที่สะกดผิดและเสนอคำทางเลือกเพื่อเพิ่มความแม่นยำในการค้นหา"

    # feature loop
    - icon: "unreadable_characters"
      title: "การสนับสนุนการจัดเก็บที่ครอบคลุม"
      content: "จัดทำดัชนี ZIP ที่ซ้อนกันและเรียกดูรายการไฟล์ภายในได้อย่างละเอียด"

    # feature loop
    - icon: "hidden_print"
      title: "การจัดทำดัชนีที่ประหยัดพื้นที่"
      content: "ประหยัดพื้นที่ดิสก์ด้วยการจัดทำดัชนีที่กระชับและจัดการไฟล์ที่มีรหัสผ่าน"

    # feature loop
    - icon: "style"
      title: "การสนับสนุนคำพ้องแบบกำหนดเอง"
      content: "ขยายพจนานุกรมคำพ้องเพื่อเพิ่มความแม่นยำในการค้นหาด้วยตัวเลือกที่ปรับแต่ง"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "ลองใช้ฟีเจอร์ของ GroupDocs.Search for Java ด้วยตัวอย่างโค้ดเหล่านี้"
  items:
    # code sample loop
    - title: "เพิ่มประสิทธิภาพการค้นหาด้วยการจับคู่แบบใกล้เคียง"
      content: |
        สำรวจความยืดหยุ่นของ GroupDocs.Search for Java สำหรับการจัดการเนื้อหาด้วยความสามารถในการค้นหาที่ล้ำสมัย [เรียนรู้เพิ่มเติม](https://docs.groupdocs.com/search/java/search-results/)
        {{< landing/code title="วิธีการจัดการผลลัพธ์การค้นหา">}}
        ```java {style=abap}
        // สร้างดัชนี
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // ตั้งค่าตัวเลือกการค้นหา
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // ค้นหาสำหรับเอกสารที่มีคำว่า 'น้ำ' หรือวลี 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // ประมวลผลผลลัพธ์การค้นหา
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
    - title: "ปรับปรุงผลลัพธ์ด้วย Expressions ปกติ"
      content: |
        ใช้การแสดงผลปกติใน GroupDocs.Search for Java เพื่อสร้างผลลัพธ์การค้นหาที่แม่นยำและละเอียด [ค้นพบเทคนิคขั้นสูง](https://docs.groupdocs.com/search/java/regular-expression-search/)
        {{< landing/code title="วิธีการค้นหาด้วยการแสดงผลปกติ">}}
        ```java {style=abap}   
        // สร้างดัชนี
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // ค้นหาวลีในรูปแบบข้อความ

        // อักขระ caret ตัวแรกที่ต้นบ่งบอกว่านี่เป็นคำค้นหาที่ใช้การแสดงผลปกติ
        String query = "^^(.)\\1{1,}";
        // ค้นหาสำหรับตัวอักษรที่ซ้ำกันสองตัวหรือมากกว่าที่ต้นคำ
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
