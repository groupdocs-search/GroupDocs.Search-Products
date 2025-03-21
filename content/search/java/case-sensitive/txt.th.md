
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: th
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ดำเนินการค้นหาแบบแยกตัวพิมพ์ใน TXT ด้วย Java"
head_description: "API GroupDocs.Search for Java ช่วยให้นักพัฒนา Java สามารถดำเนินการค้นหาแบบแยกตัวพิมพ์ในเอกสารหลายประเภทได้"

############################# Header ############################
title: "การค้นเอกสารแบบแยกตัวพิมพ์" 
description: "GroupDocs.Search for Java ช่วยให้คุณสามารถ Implement ฟังก์ชันการค้นหาแบบแยกตัวพิมพ์ในโปรเจค Java ของคุณได้"
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "รับฟรี"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "เรียนรู้เกี่ยวกับ GroupDocs.Search"
    link: "/search/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) เป็นเครื่องมือที่หลากหลายสำหรับการค้นหาและจัดทำดัชนีข้อความในเอกสารต่างๆ รองรับกว่า 70 รูปแบบรวมถึง PDFs, เอกสาร Word, งานนำเสนอ PowerPoint, แผ่น Excel, รูปภาพ และ ZIPs ซึ่งช่วยให้คุณจัดการกับชุดข้อมูลขนาดใหญ่ได้อย่างมีประสิทธิภาพ

############################# Steps ############################
steps:
    enable: true
    title: "คู่มือการค้นหาแบบแยกตัวพิมพ์ในไฟล์ TXT"
    content: |
      ด้วย [GroupDocs.Search](/search/java/) คุณสามารถดำเนินการค้นหาแบบแยกตัวพิมพ์ในเอกสาร TXT ได้ ซึ่งช่วยเสริมโปรเจค Java ของคุณ
      
      1. กำหนดโฟลเดอร์สำหรับการจัดเก็บดัชนีการค้นหา
      2. เลือกโฟลเดอร์ที่มีไฟล์ TXT
      3. ดำเนินการค้นหาที่แยกตัวพิมพ์และเก็บผลลัพธ์
      4. ประมวลผลและใช้ผลลัพธ์การค้นหา
   
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
        // กำหนดตำแหน่งสำหรับการจัดเก็บดัชนี
        Index index = new Index("c:/MyIndex");

        // ชี้ไปที่โฟลเดอร์ที่มีเอกสารที่จะค้นหา
        index.add("c:/MyDocuments");

        // เปิดใช้งานโหมดการแยกตัวพิมพ์ในการตั้งค่าการค้นหา
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // ดำเนินการค้นหา
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "เครื่องมือค้นหาและจัดทำดัชนีที่พัฒนาแล้ว"
  description: "ด้วย GroupDocs.Search for Java คุณสามารถปรับปรุงการค้นหาและการจัดทำดัชนีเอกสารสำหรับรูปแบบกว่า 70 รูปแบบ ทำให้ค้นหาข้อมูลและจัดระเบียบข้อมูลได้ง่ายขึ้น"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "จุดเด่นของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความที่ยืดหยุ่น"
      content: "ค้นหาผ่านเอกสารต่างๆ เช่น PDFs, เอกสาร Word, สเปรดชีต และงานนำเสนอ โดยใช้เครื่องมือต่างๆ เช่น การจับคู่แบบระบุ, การค้นหาที่ไม่ชัดเจน และการสนับสนุนอักขระตัวพิมพ์แทนเพื่อปรับผลลัพธ์ของคุณ"

    # feature loop
    - title: "การจัดการดัชนีที่มีประสิทธิภาพ"
      content: "จัดระเบียบและทำดัชนีชุดข้อมูลขนาดใหญ่เพื่อปรับปรุงความเร็วและประสิทธิภาพในการค้นหาเมื่อจัดการกับคอลเลกชันเอกสารขนาดใหญ่"

    # feature loop
    - title: "รองรับภาษาโลก"
      content: "ดำเนินการค้นหาในกว่า 80 ภาษา รองรับแป้นพิมพ์และความแตกต่างทางภาษาเพื่อความแม่นยำที่ดียิ่งขึ้น"

    # feature loop
    - title: "ตัวกรองการค้นหาที่ปรับแต่งได้"
      content: "ปรับเกณฑ์การค้นหาด้วยตัวเลือกต่างๆ เช่น ความไวต่อการพิมพ์, การกรองช่วงวันที่ และการยกเว้นคำหรือข้อมูลที่ไม่ต้องการในระหว่างการจัดทำดัชนี"
      
  code_samples_ext:
    # code sample ext loop
    - title: "ตัวอย่าง: คำค้นหาที่แยกตัวพิมพ์"
      content: |
        ตัวอย่างนี้แสดงวิธีการดำเนินการค้นหาแบบแยกตัวพิมพ์สำหรับเอกสาร TXT
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // กำหนดไดเร็กทอรีสำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // กำหนดตำแหน่งของโฟลเดอร์เอกสาร
          index.add("c:/MyDocuments");

          // ตั้งค่าคำค้นหา
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // เปิดใช้งานความไวต่อกรณีในตัวเลือกการค้นหา
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // ดำเนินการค้นหาเอกสาร
          SearchResult result = index.search(wordQuery, options);
          
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
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
    title: "ภาพรวมฟีเจอร์ที่สำคัญ"
    exclude: "case-sensitive"
    description: "ค้นพบความสามารถในการค้นหาที่แข็งแกร่งและมีประสิทธิภาพที่นำเสนอโดย GroupDocs.Search for Java"
    items: 
          
        # operation loop 1
        - name: "ค้นหาตามเงื่อนไข"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "ค้นหาข้อมูลในเอกสารโดยใช้เงื่อนไขเชิงบูลีน"

        # operation loop 2
        - name: "การค้นหาตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "เพิ่มความแม่นยำในการค้นหาด้วยการพิจารณาความแตกต่างของตัวพิมพ์"

        # operation loop 3
        - name: "การจัดทำดัชนีเอกสาร"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "จัดทำดัชนีเอกสารเพียงครั้งเดียวและนำกลับมาใช้ใหม่สำหรับการค้นหาหลายครั้ง"

        # operation loop 4
        - name: "ตัวกรองการค้นหา"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "ใช้ตัวกรองเพื่อลดปริมาณข้อมูลที่ถูกประมวลผล"

        # operation loop 5
        - name: "ประโยคที่แน่นอน"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "ค้นหาประโยคหรือลำดับคำเฉพาะ"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "รูปแบบไฟล์ที่รองรับสำหรับการค้นหา"
    exclude: "TXT"
    description: "GroupDocs.Search ทำงานร่วมกับรูปแบบเอกสารยอดนิยมกว่า 70 รูปแบบ เสนอการตั้งค่าการค้นหาที่ปรับแต่งได้และการจัดทำดัชนีที่มีประสิทธิภาพ"
    items: 
        # format loop 1
        - name: "การค้นหา DOCX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "การค้นหา PDF ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "การค้นหา PPTX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "การค้นหา TXT ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "การค้นหา XLSX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---