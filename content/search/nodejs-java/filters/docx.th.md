
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: th
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ค้นหาในเอกสาร DOCX โดยใช้ Node.js"
head_description: "GroupDocs.Search for Node.js via Java เพิ่มความสามารถในการค้นหาข้อความที่รวดเร็วและแม่นยำให้กับแอปพลิเคชัน JavaScript รองรับหลายรูปแบบเอกสาร."

############################# Header ############################
title: "ค้นหาข้อความในเอกสารทางธุรกิจ" 
description: "GroupDocs.Search for Node.js via Java มอบฟังก์ชันการค้นหาที่ทรงพลังและยืดหยุ่นสำหรับเอกสาร รวมถึงการรวมการค้นหาข้อความเข้ากับแอปพลิเคชัน Node.js."
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
    title: "อะไรคือ GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) เป็นไลบรารีการค้นหาและการจัดทำดัชนีที่แข็งแกร่ง ช่วยให้สามารถดึงข้อมูลที่รวดเร็วในเอกสาร รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ รวมถึง PDF, Word, Excel และ PowerPoint เพื่อให้การค้นหาที่แม่นยำและมีประสิทธิภาพ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการค้นหาในเอกสาร DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ช่วยให้การค้นหาข้อความในเอกสาร DOCX เป็นเรื่องง่ายและมีประสิทธิภาพสำหรับแอปพลิเคชัน Node.js via Java.
      
      1. สร้างไดเรกทอรีสำหรับจัดเก็บดัชนีการค้นหา.
      2. เลือกโฟลเดอร์ที่มีเอกสาร.
      3. ตั้งค่าตัวเลือกการค้นหาเพื่อรวมเฉพาะไฟล์ DOCX.
      4. ดำเนินการค้นหาและดึงผลลัพธ์.
   
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

        // กำหนดไดเรกทอรีสำหรับจัดเก็บดัชนีการค้นหา
        const index = new searchLib.Index("c:/MyIndex");

        // ระบุโฟลเดอร์ที่มีเอกสารที่ค้นหาได้
        index.add("c:/MyDocuments");

        // จำกัดการค้นหาเฉพาะรูปแบบไฟล์ที่กำหนด
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".docx");

        // ดึงและประมวลผลผลลัพธ์การค้นหา
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ความสามารถการค้นหาขั้นสูง"
  description: "GroupDocs.Search for Node.js via Java ช่วยเพิ่มประสิทธิภาพในการค้นหาเอกสารโดยการจัดทำดัชนีรูปแบบไฟล์มากกว่า 70 รูปแบบ ปรับแต่งการเรียกคืนเนื้อหาด้วยเทคนิคการค้นหาขั้นสูง."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความที่ครอบคลุม"
      content: "ดึงและหาข้อความในรูปแบบเอกสารยอดนิยม เช่น PDF, ไฟล์ Word, สเปรดชีต และการนำเสนอ รองรับการค้นหาที่ไม่แน่นอน, เสียงพ้อง, และการค้นหาด้วยอักขระแทน."

    # feature loop
    - title: "การจัดทำดัชนีที่ปรับแต่งสำหรับประสิทธิภาพ"
      content: "เร่งการค้นหาด้วยการสร้างดัชนีที่สามารถนำกลับมาใช้ใหม่ได้ พร้อมเพิ่มความเร็วและประสิทธิภาพเมื่อทำงานกับคอลเลกชันเอกสารขนาดใหญ่."

    # feature loop
    - title: "การสนับสนุนหลายภาษา"
      content: "ค้นหาเอกสารในมากกว่า 80 ภาษา เครื่องมือรับรู้รูปแบบแป้นพิมพ์และความแตกต่างของคำเพื่อความแม่นยำที่ดียิ่งขึ้น."

    # feature loop
    - title: "ตัวเลือกการค้นหาที่ปรับแต่งได้"
      content: "ปรับแต่งผลลัพธ์การค้นหาด้วยฟิลเตอร์, การแสดงนิพจน์ปกติ, ความไวต่ออักษรตัวพิมพ์ใหญ่ และการตั้งค่าอื่น ๆ ที่ยืดหยุ่น."
      
  code_samples_ext:
    # code sample ext loop
    - title: "กรองเอกสารที่ค้นหาได้"
      content: |
        เรียนรู้วิธีปรับปรุงการค้นหาเอกสารโดยใช้ฟิลเตอร์.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // กำหนดค่าดัชนีเพื่อลบรูปแบบไฟล์ที่ไม่ต้องการ
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // ระบุไดเรกทอรีที่มีเอกสาร
          index.add("c:/MyDocuments");

          // ประมวลผลผลลัพธ์การค้นหาเพื่อใช้งานต่อไป
          const result = index.Search("Lorem", options);
          
          // ประมวลผลผลลัพธ์การค้นหาเพื่อใช้งานต่อไป
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
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "ฟังก์ชันหลัก"
    exclude: "filters"
    description: "ดำเนินการค้นหาข้อความที่รวดเร็วและแม่นยำทั่วทั้งเอกสาร."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหาในรูปแบบเอกสารที่หลากหลาย"
    exclude: "DOCX"
    description: "GroupDocs.Search รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ ทำให้สามารถค้นหาข้อความได้อย่างมีประสิทธิภาพในเอกสารทางธุรกิจและสำนักงานต่าง ๆ."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "รูปแบบเอกสารพกพา Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---