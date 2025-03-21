
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: th
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่ใน TXT ด้วย Node.js"
head_description: "API GroupDocs.Search for Node.js via Java ช่วยให้นักพัฒนาที่ใช้ JavaScript สามารถดำเนินการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่ในประเภทเอกสารต่างๆ ได้"

############################# Header ############################
title: "การค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่" 
description: "GroupDocs.Search for Node.js via Java ช่วยให้คุณสามารถนำฟังก์ชันการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่ไปใช้ในแอปพลิเคชัน Node.js ของคุณ"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "คืออะไร GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) เป็นไลบรารีที่มีพลังสำหรับการค้นหาและสร้างดัชนีข้อความในเอกสาร รองรับรูปแบบมากกว่า 70 รูปแบบ รวมถึง PDF, Word, Excel, PowerPoint, รูปภาพ และไฟล์ ZIP ทำให้จัดการข้อมูลจำนวนมากได้อย่างมีประสิทธิภาพ

############################# Steps ############################
steps:
    enable: true
    title: "ขั้นตอนในการดำเนินการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่ในไฟล์ TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ช่วยให้คุณสามารถดำเนินการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่ในไฟล์ TXT ได้อย่างมีประสิทธิภาพ ช่วยเพิ่มเวิร์กโฟลว์ใน Node.js via Java ของคุณ
      
      1. ตั้งค่าโฟลเดอร์เพื่อจัดเก็บดัชนีการค้นหา
      2. เลือกโฟลเดอร์ที่มีไฟล์ TXT
      3. ดำเนินการค้นหาและรับผลลัพธ์
      4. ประมวลผลและใช้ผลลัพธ์
   
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

        // ระบุเส้นทางสำหรับโฟลเดอร์ดัชนี
        const index = new searchLib.Index("c:/MyIndex");

        // ตั้งค่าโฟลเดอร์ที่มีเอกสารสำหรับการค้นหา
        index.add("c:/MyDocuments");

        // เปิดใช้งานการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่ในการตั้งค่า
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // ดำเนินการค้นหา
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ฟีเจอร์สำคัญสำหรับการค้นหาและสร้างดัชนีเอกสาร"
  description: "ด้วย GroupDocs.Search for Node.js via Java คุณสามารถค้นหาและสร้างดัชนีข้อความในรูปแบบไฟล์มากกว่า 70 รูปแบบได้อย่างมีประสิทธิภาพ จัดระเบียบข้อมูลได้อย่างง่ายดายด้วยเครื่องมือการค้นหาขั้นสูง"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อมูลแบบครบวงจร"
      content: "ค้นหาข้อความในประเภทเอกสารต่างๆ เช่น PDF, ไฟล์ Word, สเปรดชีต และนำเสนอ ใช้ตัวเลือกเช่น การจับคู่ที่แน่นอน การค้นหาที่คลุมเครือ และอักขระพิเศษเพื่อผลลัพธ์ที่แม่นยำ"

    # feature loop
    - title: "การสร้างดัชนีข้อมูลอย่างมีประสิทธิภาพ"
      content: "สร้างและจัดการดัชนีเพื่อเร่งความเร็วในการค้นหา การสร้างดัชนีช่วยให้คุณจัดระเบียบและค้นหาข้อมูลในคอลเลกชันเอกสารขนาดใหญ่ได้อย่างรวดเร็ว"

    # feature loop
    - title: "รองรับหลายภาษา"
      content: "ค้นหาเอกสารในกว่า 80 ภาษา รองรับรูปแบบแป้นพิมพ์ที่หลากหลายและความแปรปรวนของคำ เพื่อให้ผลการค้นหาที่แม่นยำ"

    # feature loop
    - title: "การตั้งค่าการค้นหาที่ปรับแต่งได้"
      content: "ปรับการตั้งค่าการค้นหา รวมถึงความไวต่อพิมพ์ใหญ่ ตัวกรองวันที่ และการยกเว้นคำหรือข้อมูลเฉพาะระหว่างการสร้างดัชนี"
      
  code_samples_ext:
    # code sample ext loop
    - title: "ตัวอย่าง: การดำเนินการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงวิธีการดำเนินการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่สำหรับเอกสาร TXT
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // กำหนดโฟลเดอร์สำหรับดัชนีการค้นหา
          const index = new searchLib.Index("c:/MyIndex");
              
          // ระบุเส้นทางไปยังโฟลเดอร์เอกสาร
          index.add("c:/MyDocuments");

          // ตั้งค่าคำค้นหาสำหรับการค้นหา
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // เปิดใช้งานการตั้งค่าการค้นหาที่คำนึงถึงความเป็นพิมพ์ใหญ่
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // ค้นหาข้อความในเอกสาร
          const result = index.search(wordQuery, options);
          
          // ประมวลผลและจัดการผลลัพธ์
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
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
    title: "ฟังก์ชันหลัก"
    exclude: "case-sensitive"
    description: "สำรวจฟีเจอร์ขั้นสูงสำหรับการค้นหาเอกสารอย่างรวดเร็วและแม่นยำ"
    items: 
          
        # operation loop 1
        - name: "ค้นหาตามเงื่อนไข"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "ค้นหาข้อมูลในเอกสารโดยใช้เงื่อนไขเชิงบูลีน"

        # operation loop 2
        - name: "การค้นหาตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "เพิ่มความแม่นยำในการค้นหาด้วยการพิจารณาความแตกต่างของตัวพิมพ์"

        # operation loop 3
        - name: "การจัดทำดัชนีเอกสาร"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "จัดทำดัชนีเอกสารเพียงครั้งเดียวและนำกลับมาใช้ใหม่สำหรับการค้นหาหลายครั้ง"

        # operation loop 4
        - name: "ตัวกรองการค้นหา"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "ใช้ตัวกรองเพื่อลดปริมาณข้อมูลที่ถูกประมวลผล"

        # operation loop 5
        - name: "ประโยคที่แน่นอน"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "ค้นหาประโยคหรือลำดับคำเฉพาะ"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รูปแบบเอกสารที่รองรับ"
    exclude: "TXT"
    description: "GroupDocs.Search รองรับรูปแบบเอกสารมากกว่า 70 รูปแบบ ปรับแต่งตัวเลือกการค้นหาของคุณและประหยัดเวลาในการจัดทำดัชนี"
    items: 
        # format loop 1
        - name: "การค้นหา DOCX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "การค้นหา PDF ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "การค้นหา PPTX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "การค้นหา TXT ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "การค้นหา XLSX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---