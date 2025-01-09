---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: th
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
head_title: "ไลบรารีการค้นหาและจัดทำดัชนีข้อความ Node.js สำหรับเอกสาร, PDF, Office และเว็บ"
head_description: "โซลูชันการค้นหาข้อความขั้นสูงสำหรับแอปพลิเคชัน Node.js เพื่อค้นหา จัดทำดัชนีและรวบรวมข้อมูลจากเอกสาร: PDF, Word, Excel, การนำเสนอ, อีเมล และรูปแบบไฟล์เว็บ"

############################# Header ############################
title: "ค้นหาและจัดทำดัชนีเอกสารโดยใช้ API Node.js"
description: "เพิ่มประสิทธิภาพแอปพลิเคชัน Node.js โดยการนำเสนอการค้นหาข้อความในรูปแบบเอกสารยอดนิยมทั้งหมด"
words:
  for: "สำหรับ"

actions:
  main: "ดาวน์โหลด NPM ฟรี"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "การออกใบอนุญาต"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "เริ่มการเดินทางของคุณวันนี้!"
  description: "สำรวจความสามารถของ GroupDocs.Search ฟรี หรือขอใบอนุญาตเพื่อปลดล็อกศักยภาพทั้งหมด"

release:
  title: "รุ่น {0} ได้รับการเปิดตัว"
  notes: "ดูสิ่งที่ใหม่"
  downloads: "การดาวน์โหลด"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "ดำเนินการค้นหาข้อความในโฟลเดอร์ด้วย JavaScript"
  more: "ตัวอย่างเพิ่มเติม"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // สร้างดัชนีสำหรับเอกสารของคุณ
    const index = new searchLib.Index('c:/MyIndex');

    // เพิ่มเอกสารลงในดัชนีเพื่อการค้นหาที่มีประสิทธิภาพ
    index.add('c:/MyDocuments');
    
    // ค้นหาคำหรือวลีเฉพาะ เช่น
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search ภาพรวม"
  description: "ไลบรารี Node.js JavaScript สำหรับการค้นหาข้อความ"
  features:
    # feature loop
    - title: "การจัดทำดัชนีและการดำเนินการค้นหาใน Node.js"
      content: "การจัดทำดัชนีใน GroupDocs.Search for Node.js via Java รวบรวม เก็บ และวิเคราะห์ข้อมูลเพื่อการค้นหาที่แม่นยำและมีประสิทธิภาพ ดัชนีเหล่านี้มักใช้เพื่อการค้นหา"

    # feature loop
    - title: "รวมดัชนีหลายๆ ตัวเพื่อเพิ่มประสิทธิภาพการค้นหา"
      content: "GroupDocs.Search for Node.js via Java API อนุญาตให้มีการรวมหลายดัชนีเข้าด้วยกัน การแก้ไขบ่อยๆ สร้างดัชนีเดลต้า ซึ่งอาจทำให้ผลการค้นหาช้าลง โซลูชันของเรารวมดัชนีเดลต้าเหล่านี้เข้ากับดัชนีทั่วไปที่มีข้อมูลทั้งหมดจากดัชนีเดลต้านี้ เพื่อเพิ่มประสิทธิภาพการค้นหาในขณะที่เก็บดัชนีเดลต้าไว้ไม่เปลี่ยนแปลง ขนาดใหญ่"

    # feature loop
    - title: "รับรู้คำค้นหาจากรูปแบบแป้นพิมพ์ที่แตกต่างกัน"
      content: "GroupDocs.Search for Node.js via Java สามารถประมวลผลคำค้นหาที่ไม่ตรงกับรูปแบบแป้นพิมพ์ ปัจจุบันรองรับ 88 ภาษาและ 164 รูปแบบแป้นพิมพ์"

    # feature loop
    - title: "ค้นหาด้วยรูปแบบคำ Morphological"
      content: "ด้วย GroupDocs.Search for Node.js via Java คุณสามารถค้นหาคำรูปแบบต่างๆ เช่น คำนามเอกพจน์และพหูพจน์ หรือรูปแบบกริยา รวมทั้งปรับแต่งสำหรับภาษาอังกฤษและภาษาอื่นๆ"

############################# Platforms ############################
platforms:
  enable: true
  title: "ความเป็นอิสระของแพลตฟอร์ม"
  description: "GroupDocs.Search for Node.js via Java รองรับระบบปฏิบัติการและผู้จัดการแพ็กเกจที่เป็นที่นิยมทั้งหมด"
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
  title: "รูปแบบไฟล์ที่รองรับ"
  description: |
    GroupDocs.Search for Node.js via Java เปิดโอกาสให้ประมวลผลไฟล์รูปแบบมากมาย [สำรวจรายการทั้งหมด](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/)
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
  title: "ฟีเจอร์ของ GroupDocs.Search for Node.js via Java"
  description: "ควบคุมเนื้อหาของเอกสารธุรกิจโดยใช้เครื่องมือค้นหาที่มีความก้าวหน้า รองรับไฟล์รูปแบบที่ยอดนิยมรวมถึง PDF, DOCX, XLSX, PPTX และอื่นๆ"

  items:
    # feature loop
    - icon: "document_info"
      title: "พารามิเตอร์ที่ยืดหยุ่น"
      content: "ใช้ช่วงวันที่และความไวต่ออักษรเป็นพารามิเตอร์การค้นหา"

    # feature loop
    - icon: "detect"
      title: "ค้นหาแบบตรวจสอบการสะกด"
      content: "ใช้คำค้นหาที่ตรวจสอบการสะกดและไวลด์การ์ดแล้วข้ามอักขระพิเศษในการค้นหา"

    # feature loop
    - icon: "collect"
      title: "การกรองผลลัพธ์"
      content: "ตั้งค่าการกรองเอกสารในผลลัพธ์การค้นหา"

    # feature loop
    - icon: "get"
      title: "นำเข้าและส่งออก"
      content: "ทำการนำเข้าใช้รายการเพื่อลดเสียงที่เป็นระเบียบในการจัดทำดัชนีและส่งออกไปที่ไฟล์"

    # feature loop
    - icon: "remove"
      title: "ข้ามข้อมูลที่ไม่จำเป็น"
      content: "เลือกข้ามการจัดทำดัชนีสำหรับไฟล์เฉพาะและข้ามคำเฉพาะเพื่อให้เกิดความรวดเร็วในการจัดทำดัชนี"

    # feature loop
    - icon: "style"
      title: "การประมวลผล URL"
      content: "ดึงข้อความที่มีรูปแบบ HTML ไปยังไฟล์และสร้าง URL เพื่อเข้าสู่ผลการค้นหาใน HTML"

    # feature loop
    - icon: "detect"
      title: "ค้นหาอย่างรวดเร็ว"
      content: "แบ่งการค้นหาให้เป็นชิ้นเล็กเพื่อการค้นหาในดัชนีขนาดใหญ่ที่รวดเร็ว"

    # feature loop
    - icon: "manipulate"
      title: "การประมวลผลสตรีม"
      content: "จัดทำดัชนีเอกสารจากสตรีมและโครงสร้างข้อมูล"

    # feature loop
    - icon: "compare"
      title: "จัดการการสะกดผิด"
      content: "ใช้จำนวนที่ปรากฏสำหรับคำที่พบแต่ละคำและเสนอคำเลือกในกรณีที่มีการสะกดผิด"

    # feature loop
    - icon: "unreadable_characters"
      title: "การสนับสนุนการจัดเก็บ"
      content: "จัดทำดัชนี ZIP ที่บรรจุไฟล์ไว้ภายในอื่น ZIP และเรียกดูรายการไฟล์ที่ได้จัดทำดัชนีในบรรจุภัณฑ์"

    # feature loop
    - icon: "hidden_print"
      title: "การประหยัดพื้นที่ดิสก์"
      content: "ประหยัดพื้นที่ด้วยการจัดทำดัชนีที่กระชับและจัดทำดัชนีไฟล์ที่มีรหัสผ่าน"

    # feature loop
    - icon: "style"
      title: "คำพ้องแบบกำหนดเอง"
      content: "เพิ่มคำพ้องภาษาอังกฤษลงในพจนานุกรมคำพ้องเริ่มต้น"

############################# Code samples ############################
code_samples:
  enable: true
  title: "ตัวอย่างโค้ด"
  description: "สำรวจฟังก์ชันการทำงานของ GroupDocs.Search for Node.js via Java ด้วยตัวอย่าง"
  items:
    # code sample loop
    - title: "ใช้การค้นหาแบบ 'fuzzy' เพื่อเพิ่มประสิทธิภาพ"
      content: |
        สนุกกับความสามารถในการฟังก์ชัน GroupDocs.Search for Node.js via Java เพื่อเพิ่มการควบคุมเนื้อหาของเอกสารโดยอัลกอริธึมการค้นหาที่ซับซ้อน [เรียนรู้เพิ่มเติม](https://docs.groupdocs.com/search/nodejs-java/search-results/)
        {{< landing/code title="วิธีการจัดการผลลัพธ์การค้นหา">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // สร้างดัชนี
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // ตั้งค่าตัวเลือกการค้นหา
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // ค้นหาสำหรับเอกสารที่มีคำว่า 'น้ำ' หรือวลี 'Lorem ipsum'
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // ประมวลผลผลลัพธ์การค้นหา
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
    - title: "การแสดงผลปกติสามารถใช้สำหรับสถานการณ์การค้นหาขั้นสูง"
      content: |
        GroupDocs.Search for Node.js via Java ช่วยให้เราสามารถใช้การแสดงผลปกติเพื่อลดผลการค้นหา [ดำน้ำลงไปในเทคนิคการค้นหาขั้นสูง](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/)
        {{< landing/code title="วิธีการค้นหาด้วยการแสดงผลปกติ">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // สร้างดัชนี
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // ค้นหาวลีในรูปแบบข้อความ

        // อักขระ caret ตัวแรกที่ต้นบ่งบอกว่านี่เป็นคำค้นหาที่ใช้การแสดงผลปกติ
        const query = '^^(.)\\1{1,}';
        // ค้นหาสำหรับตัวอักษรที่ซ้ำกันสองตัวหรือมากกว่าที่ต้นคำ
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
