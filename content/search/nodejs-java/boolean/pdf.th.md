
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: th
format: Pdf
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "การค้นหา Boolean PDF ผ่าน Node.js"
head_description: "ใช้ API GroupDocs.Search for Node.js via Java เพื่อทำการค้นหาขั้นสูงในเนื้อหาของเอกสารด้วยตัวดำเนินการ boolean เช่น AND, OR และ NOT ที่ออกแบบมาสำหรับนักพัฒนา JavaScript."

############################# Header ############################
title: "ดำเนินการค้นหาตามหลักการ Boolean" 
description: "ด้วย GroupDocs.Search for Node.js via Java คุณสามารถสร้างคำค้นหาขั้นสูงโดยใช้ตัวดำเนินการ boolean (AND, OR, NOT) ได้อย่างราบรื่นในสภาพแวดล้อม Node.js ของคุณ."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดทันที"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search คืออะไร?"
    link: "/search/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) เป็นเครื่องมือที่ทรงพลังในการค้นหาและจัดทำดัชนีข้อความในเอกสาร รองรับรูปแบบมากกว่า 70 ประเภท เช่น PDF, Word, Excel, PowerPoint, รูปภาพ และไฟล์ ZIP ทำให้สามารถประมวลผลข้อมูลจำนวนมากได้อย่างมีประสิทธิภาพ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีค้นหาในเอกสาร PDF โดยใช้ตัวดำเนินการ boolean"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ช่วยให้คุณสามารถค้นหาเนื้อหาในไฟล์ PDF ได้อย่างมีประสิทธิภาพ ด้วยตรรกะ boolean คุณสามารถปรับปรุงคำค้นหาของคุณในแอปพลิเคชัน Node.js via Java เพื่อความแม่นยำที่ดียิ่งขึ้น.
      
      1. ตั้งค่าโฟลเดอร์เพื่อจัดเก็บดัชนีการค้นหา.
      2. เลือกโฟลเดอร์ที่มีไฟล์ PDF สำหรับการค้นหา.
      3. ดำเนินการตามคำค้นหาและดึงผลลัพธ์.
      4. ประมวลผลและวิเคราะห์ผลลัพธ์การค้นหา.
   
    code:
      platform: "nodejs-java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // กำหนดที่อยู่สำหรับโฟลเดอร์ดัชนี
        const index = new searchLib.Index("c:/MyIndex");

        // ระบุโฟลเดอร์ที่มีเอกสารสำหรับการค้นหา
        index.add("c:/MyDocuments");

        // ดำเนินการค้นหาโดยใช้ตรรกะที่ซับซ้อน
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เครื่องมือที่ทรงพลังสำหรับการค้นหาและจัดทำดัชนีเอกสาร"
  description: "GroupDocs.Search for Node.js via Java ช่วยให้การค้นหาและจัดทำดัชนีข้อความสำหรับไฟล์มากกว่า 70 ประเภท มีความรวดเร็วและแม่นยำในการค้นหาและจัดการข้อมูล."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาขข้อความที่พัฒนาแล้ว"
      content: "ค้นหาข้อความได้อย่างรวดเร็วในรูปแบบต่าง ๆ เช่น PDFs, เอกสาร Word, การนำเสนอ และสเปรดชีต ใช้ฟีเจอร์เช่น การจับคู่ที่แม่นยำ, การค้นหาด้วยอักขระแทน, และการค้นหาที่คลาดเคลื่อนเพื่อผลลัพธ์ที่แม่นยำ."

    # feature loop
    - title: "การจัดทำดัชนีข้อมูลอย่างมีประสิทธิภาพ"
      content: "สร้างและจัดการดัชนีเพื่อเพิ่มความเร็วในการค้นหาในคลังเอกสารขนาดใหญ่ การจัดทำดัชนีช่วยให้สามารถเข้าถึงข้อมูลของคุณได้อย่างรวดเร็วและเป็นระเบียบ."

    # feature loop
    - title: "การสนับสนุนหลายภาษา"
      content: "ค้นหาในเอกสารที่เขียนในมากกว่า 80 ภาษา การสนับสนุนทางรูปแบบและความเข้ากันได้ของการจัดเรียงแป้นพิมพ์ช่วยเพิ่มผลลัพธ์การค้นหาในภาษาต่าง ๆ."

    # feature loop
    - title: "การตั้งค่าการค้นหาที่มีความยืดหยุ่น"
      content: "ปรับแต่งการค้นหาของคุณโดยการเปิดใช้งานความไวต่อขนาดตัวอักษร, ใช้ตัวกรองวันที่, หรือข้ามคำและข้อมูลเฉพาะในระหว่างการจัดทำดัชนี."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ตัวอย่างการค้นหาด้วย boolean ขั้นสูง"
      content: |
        ตัวอย่างนี้แสดงวิธีสร้างคำค้นหาที่ใช้ boolean เพื่อค้นหาเนื้อหาในเอกสาร PDF.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // กำหนดโฟลเดอร์สำหรับดัชนีการค้นหา
          const index = new searchLib.Index("c:/MyIndex");
              
          // ระบุที่อยู่ของเอกสารที่ต้องการค้นหา
          index.add("c:/MyDocuments");

          // สร้างคำค้นหาโดยใช้ตัวดำเนินการ boolean
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // ดึงผลลัพธ์การค้นหา
          const result = index.search(booleanQuery);
          
          // ประมวลผลและใช้งานผลลัพธ์การค้นหา
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.pdf"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ทดลองคุณสมบัติของ GroupDocs.Search ฟรี หรือขอใบอนุญาต"
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
    title: "ความสามารถหลักของ GroupDocs.Search"
    exclude: "boolean"
    description: "ปลดล็อคคุณสมบัติการค้นหาขั้นสูงที่มีประสิทธิภาพและสามารถปรับแต่งได้."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pdf/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pdf/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหารูปแบบเอกสารยอดนิยม"
    exclude: "PDF"
    description: "GroupDocs.Search รองรับรูปแบบไฟล์มากกว่า 70 ประเภท มีกฎการค้นหาที่ยืดหยุ่นและการจัดทำดัชนีที่มีประสิทธิภาพเพื่อประหยัดเวลาและความพยายาม."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "รูปแบบเอกสารพกพา Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---