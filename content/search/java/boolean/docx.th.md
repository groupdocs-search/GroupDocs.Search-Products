
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:29
draft: false
lang: th
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "การค้นหาทางตรรกะใน DOCX ด้วย Java"
head_description: "ด้วย GroupDocs.Search for Java นักพัฒนาสามารถดำเนินการค้นหาเอกสารโดยใช้ตัวดำเนินการทางตรรกะเช่น AND, OR และ NOT ได้"

############################# Header ############################
title: "การค้นหาข้อความทางตรรกะ" 
description: "ใช้ GroupDocs.Search for Java สร้างคำค้นทางตรรกะ (AND, OR, NOT) ขั้นสูงในโครงการ Java ของคุณ"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "เกี่ยวกับ GroupDocs.Search"
    link: "/search/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) เป็นไลบรารีที่หลากหลายออกแบบมาสำหรับการค้นหาข้อความและการจัดดัชนีข้อมูลในเอกสาร รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ รวมถึง PDF, Word, Excel, PowerPoint, รูปภาพ และ ZIP archives ช่วยให้ค้นหาข้อมูลในคลังข้อมูลขนาดใหญ่ได้อย่างมีประสิทธิภาพ

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการดำเนินการค้นหาทางตรรกะในเอกสาร DOCX"
    content: |
      [GroupDocs.Search](/search/java/) ช่วยให้ค้นหาข้อความในเอกสาร DOCX ได้ โดยรองรับเงื่อนไขทางตรรกะ คุณสามารถเพิ่มความแม่นยำในการค้นหาในแอปพลิเคชัน Java
      
      1. ระบุโฟลเดอร์สำหรับจัดเก็บดัชนีการค้นหา
      2. เลือกโฟลเดอร์ที่มีเอกสาร DOCX
      3. ดำเนินการค้นหาและดึงผลลัพธ์
      4. ประมวลผลผลลัพธ์ที่ได้รับ
   
    code:
      platform: "java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command_title: "Maven XML"
        command: |
          <dependencies>
            <dependency>
              <groupId>com.groupdocs</groupId>
              <artifactId>groupdocs-search</artifactId>
              <version>{0}</version>
            </dependency>
          </dependencies>

          <repositories>
            <repository>
              <id>repository.groupdocs.com</id>
              <name>GroupDocs Repository</name>
              <url>https://repository.groupdocs.com/repo/</url>
            </repository>
          </repositories>
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // กำหนดเส้นทางสำหรับโฟลเดอร์ดัชนี
        Index index = new Index("c:/MyIndex");

        // ระบุเส้นทางของโฟลเดอร์ที่มีเอกสารสำหรับการค้นหา
        index.add("c:/MyDocuments");

        // ดำเนินการค้นหาด้วยคำถามที่ซับซ้อน
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เครื่องมือทรงพลังสำหรับการค้นหาและการจัดดัชนีเอกสาร"
  description: "GroupDocs.Search for Java ทำให้การค้นหาข้อความและการจัดดัชนีข้อมูลในรูปแบบมากกว่า 70 รูปแบบง่ายขึ้น เครื่องมือขั้นสูงช่วยให้คุณค้นหาและจัดการเนื้อหาได้อย่างมีประสิทธิภาพ"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความที่ครอบคลุม"
      content: "ค้นหาข้ามรูปแบบหลายอย่างเช่น PDFs, เอกสาร Word, งานนำเสนอ, สเปรดชีต และอื่น ๆ ใช้ตัวเลือกเช่นการจับคู่ที่แน่นอน, การค้นหาที่ไม่แน่นอน, และคำถามที่ใช้ตัวแทนในการปรับแต่งผลลัพท์"

    # feature loop
    - title: "การจัดดัชนีข้อมูลที่มีประสิทธิภาพ"
      content: "สร้างและดูแลดัชนีเพื่อการค้นหาเอกสารที่รวดเร็วขึ้น ฟีเจอร์นี้ช่วยจัดระเบียบข้อมูลอย่างมีประสิทธิภาพ ทำให้จัดการคอลเลคชันเอกสารขนาดใหญ่ได้ง่าย"

    # feature loop
    - title: "การสนับสนุนหลายภาษา"
      content: "ค้นหาในเอกสารที่เขียนด้วยภาษามากกว่า 80 ภาษา เพิ่มความแม่นยำโดยการใช้รูปแบบคำทาง Morphological และรูปแบบแป้นพิมพ์ที่แตกต่างกัน"

    # feature loop
    - title: "การปรับแต่งการค้นหาที่ยืดหยุ่น"
      content: "ปรับการตั้งค่าการค้นหาด้วยฟีเจอร์ต่าง ๆ เช่น การไวต่อการพิมพ์ตัวพิมพ์ใหญ่, การกรองช่วงวันที่, และการยกเว้นเพื่อลดความซับซ้อนของผลลัพธ์"
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้คำถามค้นหาทางตรรกะที่ซับซ้อน"
      content: |
        ตัวอย่างนี้แสดงวิธีการดำเนินการค้นหาทางตรรกะในไฟล์ DOCX
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // กำหนดโฟลเดอร์สำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // ระบุเส้นทางไปยังเอกสารที่ต้องค้นหา
          index.add("c:/MyDocuments");

          // สร้างคำถามโดยใช้ตรรกะทางตรรกะ
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // ดึงผลลัพธ์การค้นหา
          SearchResult result = index.search(booleanQuery);
          
          // ประมวลผลผลลัพธ์ที่ดึงมา
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "คัดลอก"
        install:
          command_title: "Maven XML"
          command: |
            <dependencies>
              <dependency>
                <groupId>com.groupdocs</groupId>
                <artifactId>groupdocs-search</artifactId>
                <version>{0}</version>
              </dependency>
            </dependencies>
            <repositories>
              <repository>
                <id>repository.groupdocs.com</id>
                <name>GroupDocs Repository</name>
                <url>https://repository.groupdocs.com/repo/</url>
              </repository>
            </repositories>
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ทดลองคุณสมบัติของ GroupDocs.Search ฟรี หรือขอใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "การอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "คุณสมบัติหลักในภาพรวม"
    exclude: "boolean"
    description: "เปิดใช้งานความสามารถในการค้นหาที่ทรงพลังและมีประสิทธิภาพ"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหารูปแบบเอกสารที่เป็นที่นิยม"
    exclude: "DOCX"
    description: "GroupDocs.Search รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ ช่วยให้คุณสามารถปรับกฎการค้นหาและใช้การจัดดัชนีเพื่อเพิ่มประสิทธิภาพ"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "รูปแบบเอกสารพกพา Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---