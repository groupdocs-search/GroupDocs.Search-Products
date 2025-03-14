
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: th
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ค้นหาในเอกสาร DOCX ด้วย Java"
head_description: "GroupDocs.Search for Java เพิ่มฟังก์ชันการค้นหาข้อความที่มีประสิทธิภาพในแอปพลิเคชัน Java รองรับรูปแบบเอกสารธุรกิจต่างๆ"

############################# Header ############################
title: "ค้นหาข้อความในเอกสารทางธุรกิจ" 
description: "GroupDocs.Search for Java ช่วยให้คุณค้นหาข้อความในเอกสารด้วยคำค้นที่ยืดหยุ่นและแม่นยำ รวมเข้ากับฟังก์ชันการค้นหาในแอปพลิเคชัน Java ได้อย่างราบรื่น"
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
    title: "GroupDocs.Search คืออะไร?"
    link: "/search/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) เป็นไลบรารีที่มีความสามารถในการค้นหาข้อความและการจัดทำดัชนีเอกสารอย่างรวดเร็ว รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ รวมถึงมาตรฐานในอุตสาหกรรมเช่น PDF, Word, Excel และ PowerPoint คุณสามารถเพิ่มความเร็วในการค้นหาที่แม่นยำให้กับแอปพลิเคชันของคุณได้

############################# Steps ############################
steps:
    enable: true
    title: "วิธีค้นหาในเอกสาร DOCX"
    content: |
      [GroupDocs.Search](/search/java/) ช่วยให้สามารถค้นหาข้อความได้อย่างรวดเร็วและมีประสิทธิภาพในเอกสาร DOCX ซึ่งเหมาะสำหรับแอปพลิเคชัน Java
      
      1. ระบุโฟลเดอร์เพื่อจัดเก็บดัชนีการค้นหา
      2. เลือกโฟลเดอร์ที่มีเอกสารของคุณ
      3. กำหนดค่าออปชั่นการค้นหาเพื่อจำกัดผลลัพธ์ให้อยู่ในเอกสาร DOCX
      4. ดำเนินการค้นหาและรับผลลัพธ์
   
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
        // ไดเรกทอรีสำหรับจัดเก็บดัชนีการค้นหาที่สามารถใช้ซ้ำได้
        Index index = new Index("c:/MyIndex");

        // โฟลเดอร์ที่มีเอกสาร
        index.add("c:/MyDocuments");

        // กรองการค้นหาตามรูปแบบเอกสาร
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".docx");

        // ดึงผลลัพธ์การค้นหา
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ความสามารถในการค้นหาที่พัฒนาเพิ่มขึ้น"
  description: "GroupDocs.Search for Java ให้การค้นหาข้อความขั้นสูงในมากกว่า 70 รูปแบบไฟล์ การจัดทำดัชนีช่วยเพิ่มความเร็วในการค้นหาและปรับปรุงประสิทธิภาพการจัดการเอกสาร"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "คุณสมบัติหลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความที่ทรงพลัง"
      content: "ค้นหาข้อความในรูปแบบเอกสารที่นิยมเช่น PDFs, ไฟล์ Word, งานนำเสนอ และสเปรดชีต รองรับวิธีการค้นหาหลายแบบรวมถึงการค้นหาแบบไม่สมบูรณ์, คำพ้องเสียง, และอักขระตัวแทน"

    # feature loop
    - title: "การจัดทำดัชนีที่ปรับให้เหมาะสมเพื่อประสิทธิภาพที่ดียิ่งขึ้น"
      content: "สร้างและนำกลับมาใช้ใหม่ในการจัดทำดัชนีการค้นหาเพื่อเพิ่มความเร็วและประสิทธิภาพในการค้นหา โดยเฉพาะในชุดเอกสารขนาดใหญ่"

    # feature loop
    - title: "การสนับสนุนการค้นหาหลายภาษา"
      content: "ค้นหาในเอกสารที่เขียนในมากกว่า 80 ภาษา โดยตรวจจับรูปแบบแป้นพิมพ์ที่แตกต่างกันและตัวแปรของคำเพื่อเพิ่มความแม่นยำ"

    # feature loop
    - title: "ตัวเลือกการค้นหาที่ปรับแต่งได้"
      content: "จำกัดผลลัพธ์การค้นหาด้วยตัวกรอง, นิพจน์ปกติ, และการตั้งค่าการค้นหาขั้นสูงอื่นๆ"
      
  code_samples_ext:
    # code sample ext loop
    - title: "กรองเอกสารก่อนการค้นหา"
      content: |
        เรียนรู้วิธีการปรับแต่งการค้นหาด้วยการกรอง
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // ตั้งค่าดัชนีที่ไม่รวมรูปแบบไฟล์บางรูปแบบ
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // ระบุเส้นทางการเก็บเอกสาร
          index.add("c:/MyDocuments");

          // ดึงผลลัพธ์การค้นหา
          SearchResult result = index.search("Lorem", options);
          
          // ประมวลผลและใช้ผลลัพธ์การค้นหา
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
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "คุณสมบัติหลัก"
    exclude: "filters"
    description: "ดำเนินการค้นหาข้อความที่แม่นยำและมีประสิทธิภาพ"
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
    title: "ค้นหาในเอกสารทางธุรกิจ"
    exclude: "DOCX"
    description: "GroupDocs.Search รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ ซึ่งทำให้ค้นหาเอกสารสำนักงานที่ใช้กันอย่างแพร่หลายได้ง่าย"
    items: 
        # format loop 1
        - name: "ตัวกรองการค้นหาสำหรับ DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "ตัวกรองการค้นหาสำหรับ PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "ตัวกรองการค้นหาสำหรับ PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "ตัวกรองการค้นหาสำหรับ TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "ตัวกรองการค้นหาสำหรับ XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---