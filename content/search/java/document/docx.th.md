
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: th
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ค้นหาข้อความในเอกสาร DOCX ด้วย GroupDocs.Search สำหรับ Java"
head_description: "GroupDocs.Search for Java ช่วยให้นักพัฒนา Java สามารถค้นหาข้อความในรูปแบบเอกสารต่างๆ ได้อย่างรวดเร็ว"

############################# Header ############################
title: "การค้นหาข้อความในเอกสารที่ชาญฉลาด" 
description: "ด้วย GroupDocs.Search for Java คุณสามารถค้นหาและดึงข้อความจากประเภทเอกสารหลายประเภทในแอปพลิเคชัน Java ของคุณได้อย่างราบรื่น"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ทดลองใช้ฟรี"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search ทำอะไร?"
    link: "/search/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) เป็นไลบรารีค้นหาและจัดทำดัชนีเอกสารที่มีความแข็งแกร่ง รองรับกว่า 70 รูปแบบไฟล์ รวมถึง PDF, Word, PowerPoint, Excel, รูปภาพ และ ZIP archives โดยช่วยให้การค้นหาที่รวดเร็ว แม่นยำ และสามารถขยายได้สำหรับการเก็บเอกสารขนาดใหญ่

############################# Steps ############################
steps:
    enable: true
    title: "ดำเนินการค้นหาข้อความในไฟล์ DOCX"
    content: |
      [GroupDocs.Search](/search/java/) ทำให้การค้นหาไฟล์ DOCX เป็นเรื่องง่ายขึ้นด้วยตรรกะและการจัดทำดัชนีที่ซับซ้อน ช่วยเพิ่มความแม่นยำในการค้นหาในแอปพลิเคชัน Java
      
      1. ตั้งค่าไดเรกทอรีเพื่อเก็บดัชนีการค้นหา
      2. เลือกโฟลเดอร์ที่มีไฟล์ DOCX
      3. กำหนดตัวเลือกการค้นหาเพิ่มเติม
      4. ดำเนินการค้นหาและวิเคราะห์ผลลัพธ์
   
    code:
      platform: "java"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "ผลการค้นหา"
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
        - title: "เอกสารประกอบ"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // ตั้งค่าไดเรกทอรีสำหรับการเก็บดัชนีการค้นหา
        Index index = new Index("c:/MyIndex");

        // ระบุโฟลเดอร์ที่มีเอกสารที่ค้นหาได้
        index.add("c:/MyDocuments");

        // เปิดใช้งานการค้นหาคำที่ออกเสียงคล้ายกัน
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // ดำเนินการค้นหาคำสั่งขั้นสูง
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ความสามารถในการค้นหาและจัดทำดัชนีที่ได้รับการปรับปรุง"
  description: "GroupDocs.Search for Java ทำให้การค้นหาข้อความและการจัดทำดัชนีในรูปแบบเอกสาร 70+ รูปแบบ ง่ายขึ้น โดยมีเครื่องมือที่มีประสิทธิภาพในการจัดการและเรียกคืนข้อมูลอย่างรวดเร็ว"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "คุณสมบัติเสริมของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความอย่างครอบคลุม"
      content: "ค้นหาข้อความในรูปแบบเอกสารหลายประเภท เช่น PDFs, เอกสาร Word, งานนำเสนอ PowerPoint และสเปรดชีต โดยใช้การจับคู่ที่แม่นยำ, การค้นหาที่ใกล้เคียง, และตัวดำเนินการตัวแทนเพื่อผลลัพธ์การค้นหาที่เฉพาะเจาะจง"

    # feature loop
    - title: "การจัดทำดัชนีที่ดีที่สุดสำหรับข้อมูลขนาดใหญ่"
      content: "สร้างดัชนีที่มีโครงสร้างเพื่อเร่งความเร็วในการค้นหา ทำให้สามารถนำทางผ่านฐานข้อมูลเอกสารขนาดใหญ่ได้อย่างมีประสิทธิภาพ"

    # feature loop
    - title: "รองรับหลายภาษา"
      content: "ทำการค้นหาในกว่า 80 ภาษาโดยมีการสนับสนุนที่ติดตั้งสำหรับการจัดเรียงแป้นพิมพ์ที่แตกต่างกันและรูปแบบคำ, ซึ่งช่วยเพิ่มความแม่นยำ"

    # feature loop
    - title: "การตั้งค่าการค้นหาที่ยืดหยุ่น"
      content: "ปรับแต่งการค้นหาด้วยตัวเลือกต่างๆ เช่น ความไวต่ออักขระ, การกรองตามวันที่, และความสามารถในการยกเว้นคำเฉพาะเพื่อผลลัพธ์ที่แม่นยำ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้คำสั่งค้นหาขั้นสูง"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงวิธีการใช้คำสั่งค้นหาเพื่อค้นหาภายในเอกสาร DOCX อย่างมีประสิทธิภาพ
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // กำหนดไดเรกทอรีสำหรับการทำดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // ระบุเส้นทางไฟล์สำหรับเอกสาร
          index.add("c:/MyDocuments");

          // ระบุรหัสผ่านสำหรับเอกสารที่เข้ารหัส
          index.getDictionaries().getDocumentPasswords().add("protected.docx", "123456");

          // เปิดใช้งานการค้นหาที่ใกล้เคียงเพื่อค้นหาคำที่คล้ายกัน
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // ดึงข้อมูลผลลัพธ์การค้นหา
          SearchResult result = index.Search("Loarem", options);
          
          // ประมวลผลและวิเคราะห์ผลลัพธ์การค้นหา
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
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/search/formats/searchdocument.docx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "เอกสารประกอบ"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นแล้วหรือยัง?"
  description: "ทดลองฟีเจอร์ของ GroupDocs.Search ฟรีหรือขอใบอนุญาต"
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
    title: "ภาพรวมของคุณสมบัติหลัก"
    exclude: "document"
    description: "ค้นพบความสามารถในการค้นหาข้อความที่มีประสิทธิภาพสูงซึ่งออกแบบมาเพื่อประสิทธิภาพและความแม่นยำ"
    items: 
          
        # operation loop 1
        - name: "ค้นหาตามเงื่อนไข"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "ค้นหาข้อมูลในเอกสารโดยใช้เงื่อนไขเชิงบูลีน"

        # operation loop 2
        - name: "การค้นหาตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "เพิ่มความแม่นยำในการค้นหาด้วยการพิจารณาความแตกต่างของตัวพิมพ์"

        # operation loop 3
        - name: "การจัดทำดัชนีเอกสาร"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "จัดทำดัชนีเอกสารเพียงครั้งเดียวและนำกลับมาใช้ใหม่สำหรับการค้นหาหลายครั้ง"

        # operation loop 4
        - name: "ตัวกรองการค้นหา"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "ใช้ตัวกรองเพื่อลดปริมาณข้อมูลที่ถูกประมวลผล"

        # operation loop 5
        - name: "ประโยคที่แน่นอน"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "ค้นหาประโยคหรือลำดับคำเฉพาะ"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหาข้อมูลในเอกสาร DOCX ด้วย GroupDocs.Search"
    exclude: "DOCX"
    description: "GroupDocs.Search รองรับรูปแบบกว่า 70 รูปแบบ รวมถึงไฟล์สำนักงาน ช่วยให้การค้นหาเป็นไปได้อย่างรวดเร็วด้วยฟีเจอร์การจัดทำดัชนีขั้นสูง"
    items: 
        # format loop 1
        - name: "ค้นหาในเอกสาร DOCX"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "ค้นหาในเอกสาร PDF"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "ค้นหาในเอกสาร PPTX"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "ค้นหาในเอกสาร TXT"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "ค้นหาในเอกสาร XLSX"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---