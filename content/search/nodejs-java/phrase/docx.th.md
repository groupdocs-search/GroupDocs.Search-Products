
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:41
draft: false
lang: th
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "ค้นหาวลีใน DOCX โดยใช้ Node.js"
head_description: "GroupDocs.Search for Node.js via Java เพิ่มฟังก์ชันการค้นหาวลีที่ทรงพลังให้กับแอพพลิเคชัน JavaScript สำหรับการค้นเอกสารอย่างมีประสิทธิภาพ."

############################# Header ############################
title: "ค้นหาวลีในเอกสาร" 
description: "ค้นหาวลีเฉพาะได้อย่างรวดเร็วด้วย GroupDocs.Search for Node.js via Java. บูรณาการความสามารถในการค้นหาที่รวดเร็วและแม่นยำเข้าสู่แอพพลิเคชัน Node.js ของคุณ."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลด"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "ฟีเจอร์ของ GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) เป็นไลบรารีประสิทธิภาพสูงสำหรับการจัดทำดัชนีและค้นหาข้อความในเอกสาร. รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ รวมถึง PDF, เอกสาร Word, สเปรดชีต Excel, รูปภาพ และ ZIP archives เพื่อให้ผลการค้นหาที่แม่นยำและรวดเร็ว.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีค้นหาวลีในเอกสาร DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) ทำให้การค้นหาวลีในเอกสาร DOCX เป็นเรื่องที่สามารถทำได้ง่าย. ใช้ตัวเลือกการค้นหาต่าง ๆ เพื่อปรับผลลัพธ์ในแอพพลิเคชัน Node.js via Java.
      
      1. ตั้งค่าธรรมเนียมสำหรับดัชนีการค้นหา.
      2. กำหนดโฟลเดอร์ที่บรรจุไฟล์ DOCX.
      3. กำหนดค่าพารามิเตอร์การค้นหา.
      4. ดึงและประมวลผลผลการค้นหา.
   
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

        // ระบุเส้นทางในการจัดเก็บดัชนีการค้นหา
        const index = new searchLib.Index("c:/MyIndex");

        // ตั้งค่าโฟลเดอร์ที่บรรจุเอกสาร
        index.add("c:/MyDocuments");

        // กำหนดการตั้งค่าการค้นหา
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // รันคำขอการค้นหา
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ค้นพบเอนจินค้นหาเอกสาร Node.js"
  description: "GroupDocs.Search for Node.js via Java ช่วยให้สามารถค้นหาวลีในรูปแบบไฟล์มากกว่า 70 รูปแบบ ทำให้การค้นหาและจัดระเบียบข้อมูลทำได้ง่ายด้วยฟีเจอร์การค้นขั้นสูง."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "ความสามารถหลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาวลี"
      content: "ค้นหาวลีที่แน่นอนในเอกสารธุรกิจ เช่น PDF, ไฟล์ Word, การนำเสนอ, และสเปรดชีต. ใช้เครื่องหมายแทนและตัวเลือกการค้นหาแบบยืดหยุ่นเมื่อไม่ทราบวลีทั้งหมด."

    # feature loop
    - title: "การจัดทำดัชนีข้อมูลที่ปรับแต่งแล้ว"
      content: "เพิ่มประสิทธิภาพการค้นหาด้วยการสร้างดัชนีที่นำกลับมาใช้ใหม่ได้. การจัดทำดัชนีแบบมีโครงสร้างช่วยเร่งการค้นหาเอกสารและปรับปรุงความแม่นยำ."

    # feature loop
    - title: "การรองรับหลายภาษา"
      content: "ค้นหาเอกสารในภาษามากกว่า 80 ภาษา โดยรองรับการจัดเรียงแป้นพิมพ์ที่แตกต่างกันและรูปแบบคำที่จัดรูปแบบได้ ซึ่งรับประกันผลลัพธ์ที่แม่นยำ."

    # feature loop
    - title: "ตัวเลือกการค้นหาขั้นสูง"
      content: "กำหนดค่าการค้นหาด้วยความไวต่อขนาด, การจับคู่ใกล้เคียง, การตรวจจับคำพ้อง, การกรองเอกสาร และฟีเจอร์ที่ทรงพลังอื่น ๆ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้เทคนิคการค้นหาขั้นสูง"
      content: |
        เรียนรู้วิธีสร้างคำขอสำหรับการค้นหาใน DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // กำหนดไดเรกทอรีดัชนีการค้นหา
          const index = new searchLib.Index("c:/MyIndex");
              
          // ตั้งค่าเส้นทางไปยังเอกสารเป้าหมาย
          index.add("c:/MyDocuments");

          // สร้างคำขอสำหรับวลีที่ต้องการ
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // ดึงผลการค้นหา
          const result = index.search(query);
          
          // ประมวลผลและใช้ผลลัพธ์
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
            link: "/examples/search/formats/searchphrase.docx"
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
    title: "ความสามารถในการค้นหาขั้นสูง"
    exclude: "phrase"
    description: "ใช้ฟีเจอร์การค้นหาที่ทรงพลังเพื่อผลลัพธ์ที่รวดเร็วยิ่งขึ้นและแม่นยำกว่า."
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
    title: "ค้นหาวลีในเอกสารธุรกิจ"
    exclude: "DOCX"
    description: "GroupDocs.Search สนับสนุนการค้นหาวลีในรูปแบบเอกสารมากกว่า 70 รูปแบบ. ใช้ตัวเลือกขั้นสูงและการจัดทำดัชนีเพื่อทำให้กระบวนการค้นหาเป็นไปอย่างราบรื่น."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "รูปแบบเอกสารพกพา Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---