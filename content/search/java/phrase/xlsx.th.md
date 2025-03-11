
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: th
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "ค้นหาวลีใน XLSX โดยใช้ Java"
head_description: "GroupDocs.Search for Java เป็นการเสริมความสามารถให้กับแอปพลิเคชัน Java ด้วยฟีเจอร์การค้นหาวลีขั้นสูงสำหรับเนื้อหาของเอกสาร."

############################# Header ############################
title: "ค้นหาวลีในเอกสาร" 
description: "ค้นหาวลีที่เฉพาะเจาะจงได้อย่างรวดเร็วด้วย GroupDocs.Search for Java เพิ่มฟังก์ชันการค้นหาที่ทรงพลังให้กับแอปพลิเคชัน Java ของคุณ."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลด"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search ฟีเจอร์"
    link: "/search/java/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) เป็นห้องสมุดที่แข็งแกร่งสำหรับการสร้างดัชนีและค้นหาข้อความภายในเอกสาร รองรับกว่า 70 รูปแบบไฟล์ รวมถึง PDF, เอกสาร Word, แผ่นงาน Excel, รูปภาพ, และไฟล์ ZIP เพื่อให้ผลการค้นหาที่รวดเร็วและแม่นยำ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการค้นหาวลีในเอกสาร XLSX"
    content: |
      [GroupDocs.Search](/search/java/) ช่วยให้การค้นหาวลีในเอกสาร XLSX ง่ายขึ้น ใช้ตัวเลือกต่างๆ เพื่อปรับปรุงผลการค้นหาในแอปพลิเคชัน Java.
      
      1. สร้างไดเรกทอรีดัชนีการค้นหา.
      2. ระบุโฟลเดอร์ที่มีไฟล์ XLSX.
      3. ปรับค่าพารามิเตอร์การค้นหา.
      4. ดึงและวิเคราะห์ผลการค้นหา.
   
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
        // กำหนดเส้นทางดัชนีการค้นหา
        Index index = new Index("c:/MyIndex");

        // ระบุโฟลเดอร์ที่มีเอกสาร
        index.add("c:/MyDocuments");

        // กำหนดการตั้งค่าการค้นหา
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // ดำเนินการค้นหาคำถาม
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "สำรวจเอนจิ้นการค้นหาของเอกสาร Java"
  description: "GroupDocs.Search for Java อนุญาตให้ค้นหาวลีในรูปแบบไฟล์กว่า 70 รูปแบบ ค้นหาและจัดระเบียบข้อมูลได้อย่างมีประสิทธิภาพโดยใช้ฟีเจอร์การค้นหาที่ทันสมัย."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "ความสามารถหลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาวลี"
      content: "สามารถค้นหาวลีที่แน่นอนในเอกสารธุรกิจ เช่น PDF, ไฟล์ Word, งานนำเสนอ และแผ่นงาน ใช้เวิร์ดการ์ดและตัวเลือกอื่นๆ เมื่อไม่ทราบวลีที่แน่นอน."

    # feature loop
    - title: "การสร้างดัชนีข้อมูลที่ปรับให้เหมาะสม"
      content: "เร่งความเร็วในการค้นหาเอกสารโดยการสร้างและนำกลับมาใช้ดัชนีการค้นหา การสร้างดัชนีช่วยจัดระเบียบข้อมูลอย่างมีประสิทธิภาพเพื่อการค้นหาที่รวดเร็วและแม่นยำยิ่งขึ้น."

    # feature loop
    - title: "ความเข้ากันได้กับหลายภาษา"
      content: "ค้นหาเอกสารในกว่า 80 ภาษา รองรับการจัดเรียงแป้นพิมพ์ที่แตกต่างกันและการวิเคราะห์ทางสัณฐานวิทยาเพื่อปรับปรุงความแม่นยำในการค้นหา."

    # feature loop
    - title: "ตัวเลือกการค้นหาที่ทันสมัย"
      content: "ปรับแต่งการค้นหาด้วยความละเอียดของอักษร การค้นหาที่ไม่แน่นอน การจับคู่เสียงคล้ายกัน การกรองเอกสาร และฟีเจอร์ที่ทรงพลังอื่นๆ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้วิธีการค้นหาขั้นสูง"
      content: |
        เรียนรู้วิธีการสร้างคำถามสำหรับการค้นหาใน XLSX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // กำหนดไดเรกทอรีสำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // กำหนดเส้นทางไปยังเอกสารเป้าหมาย
          index.add("c:/MyDocuments");

          // สร้างคำถามการค้นหาสำหรับวลีเฉพาะ
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // ดึงผลการค้นหาทั้งหมด
          SearchResult result = index.search(query);
          
          // ประมวลผลและใช้ผลลัพธ์ที่ดึงมาได้
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "ความสามารถในการค้นหาขั้นสูง"
    exclude: "phrase"
    description: "ใช้ฟังก์ชันการค้นหาล้ำสมัยเพื่อการปรับปรุงความแม่นยำและประสิทธิภาพ."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหาวลีในเอกสารธุรกิจ"
    exclude: "XLSX"
    description: "GroupDocs.Search สนับสนุนการค้นหาวลีในรูปแบบเอกสารกว่า 70 รูปแบบ ใช้ตัวเลือกและการทำดัชนีที่ทันสมัยสำหรับการค้นหาที่มีประสิทธิภาพ."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "รูปแบบเอกสารพกพา Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---