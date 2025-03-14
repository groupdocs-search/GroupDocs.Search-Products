
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: th
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ค้นหาข้อความใน PDF ด้วย GroupDocs.Search ใน Node.js"
head_description: "ใช้ GroupDocs.Search for Node.js via Java ร่วมกับ JavaScript ในการค้นหาข้อความอย่างมีประสิทธิภาพในรูปแบบเอกสารต่างๆ."

############################# Header ############################
title: "โซลูชันการค้นหาเอกสารอัจฉริยะ" 
description: "ค้นหาข้อความในรูปแบบเอกสารที่หลากหลายด้วย GroupDocs.Search for Node.js via Java สร้างคำค้นหาที่ซับซ้อนภายในแอปพลิเคชัน Node.js ของคุณ."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ลองใช้งานฟรี"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "แนะนำเกี่ยวกับ GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) เป็นไลบรารีประสิทธิภาพสูงสำหรับการค้นหาข้อความเต็มรูปแบบและการจัดทำดัชนีเอกสาร รองรับประเภทไฟล์กว่า 70 ประเภท รวมถึง PDF, Word, PowerPoint, Excel, รูปภาพ และไฟล์ ZIP เพื่อให้ได้ผลลัพธ์ที่รวดเร็วและแม่นยำ.

############################# Steps ############################
steps:
    enable: true
    title: "ดำเนินการค้นหาในไฟล์ PDF"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ช่วยให้คุณสามารถดำเนินการค้นหาในไฟล์ PDF โดยการปรับผลลัพธ์ในแอปพลิเคชัน Node.js via Java.
      
      1. กำหนดโฟลเดอร์สำหรับการจัดเก็บดัชนีการค้นหา.
      2. เลือกโฟลเดอร์ที่มีไฟล์ PDF.
      3. ตั้งค่าพารามิเตอร์การค้นหาเพิ่มเติม.
      4. ดำเนินการค้นหาและวิเคราะห์ผลลัพธ์.
   
    code:
      platform: "nodejs-java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "ผลการค้นหา"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "เอกสารประกอบ"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // กำหนดไดเรกทอรีสำหรับการจัดเก็บดัชนีการค้นหา
        const index = new searchLib.Index("c:/MyIndex");

        // เลือกโฟลเดอร์ที่มีเอกสารสำหรับการค้นหา
        index.add("c:/MyDocuments");

        // เปิดใช้งานการค้นหาคำเหมือนที่ฟังดูคล้ายกัน
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // ดำเนินการค้นหาที่ซับซ้อน
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ความสามารถในการค้นหาและจัดทำดัชนีขั้นสูง"
  description: "GroupDocs.Search for Node.js via Java ให้เครื่องมือค้นหาและจัดทำดัชนีที่ทรงพลังสำหรับเอกสารกว่า 70 รูปแบบ ทำให้ค้นหาและจัดระเบียบข้อมูลได้ง่าย."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "ประโยชน์หลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "ค้นหาข้อความอย่างครอบคลุม"
      content: "ค้นหาข้อความในเอกสารประเภทต่างๆ รวมถึง PDF, เอกสาร Word, งานนำเสนอ PowerPoint และสเปรดชีต ใช้การจับคู่ที่แน่นอน การค้นหาแบบเบลอ และอักขระพิเศษสำหรับผลลัพธ์ที่แม่นยำ."

    # feature loop
    - title: "การจัดทำดัชนีที่มีประสิทธิภาพสำหรับข้อมูลขนาดใหญ่"
      content: "เพิ่มความเร็วในการค้นหาด้วยการสร้างดัชนีที่มีโครงสร้าง ทำให้การดึงข้อมูลจากคอลเล็กชันเอกสารขนาดใหญ่เป็นไปได้ง่าย."

    # feature loop
    - title: "รองรับ 80+ ภาษา"
      content: "ค้นหาในเอกสารที่แตกต่างกันในหลายภาษา พร้อมการรู้จำอัตโนมัติของรูปแบบคำต่าง ๆ และรูปแบบแป้นพิมพ์."

    # feature loop
    - title: "การตั้งค่าการค้นหาที่กำหนดเอง"
      content: "ปรับแต่งตัวเลือกการค้นหา เช่น ความไวต่อพิมพ์ใหญ่พิมพ์เล็ก ตัวกรองวันที่ และคำที่ไม่รวม เพื่อให้ได้ผลลัพธ์ที่แม่นยำ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้การค้นหาสำหรับเอกสาร PDF"
      content: |
        ตัวอย่างนี้แสดงวิธีการใช้คำค้นหาในเอกสาร PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // ตั้งค่าไดเรกทอรีสำหรับการจัดทำดัชนีการค้นหา
          const index = new searchLib.Index("c:/MyIndex");
              
          // ระบุที่อยู่ไฟล์สำหรับการจัดเก็บเอกสาร
          index.add("c:/MyDocuments");

          // ป้อนรหัสผ่านสำหรับไฟล์ที่ปกป้อง
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", '123456');

          // เปิดใช้งานการค้นหาคำที่ฟังดูคล้ายกัน
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // ดึงผลลัพธ์การค้นหา
          const result = index.search("Loarem", options);
          
          // ประมวลผลและตรวจสอบผลลัพธ์
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "คัดลอก"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pdf"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "เอกสารประกอบ"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นแล้วหรือยัง?"
  description: "ทดลองฟีเจอร์ของ GroupDocs.Search ฟรีหรือขอใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "การอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "สำรวจฟีเจอร์หลัก"
    exclude: "document"
    description: "ค้นพบฟีเจอร์ค้นหาที่มีความเร็วสูงออกแบบมาเพื่อเพิ่มประสิทธิภาพและความแม่นยำ."
    items: 
          
        # operation loop 1
        - name: "ค้นหาตามเงื่อนไข"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "ค้นหาข้อมูลในเอกสารโดยใช้เงื่อนไขเชิงบูลีน"

        # operation loop 2
        - name: "การค้นหาตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "เพิ่มความแม่นยำในการค้นหาด้วยการพิจารณาความแตกต่างของตัวพิมพ์"

        # operation loop 3
        - name: "การจัดทำดัชนีเอกสาร"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "จัดทำดัชนีเอกสารเพียงครั้งเดียวและนำกลับมาใช้ใหม่สำหรับการค้นหาหลายครั้ง"

        # operation loop 4
        - name: "ตัวกรองการค้นหา"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "ใช้ตัวกรองเพื่อลดปริมาณข้อมูลที่ถูกประมวลผล"

        # operation loop 5
        - name: "ประโยคที่แน่นอน"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "ค้นหาประโยคหรือลำดับคำเฉพาะ"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหาในเอกสารหลากหลาย"
    exclude: "PDF"
    description: "GroupDocs.Search ทำงานร่วมกับไฟล์กว่า 70 รูปแบบ รวมถึงเอกสารสำนักงาน เพื่อให้การค้นหาที่รวดเร็วและแม่นยำพร้อมการสนับสนุนการจัดทำดัชนี."
    items: 
        # format loop 1
        - name: "ค้นหาในเอกสาร DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "ค้นหาในเอกสาร PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "ค้นหาในเอกสาร PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "ค้นหาในเอกสาร TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "ค้นหาในเอกสาร XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---