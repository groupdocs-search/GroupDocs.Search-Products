
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: th
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ค้นหา XLSX ใน .NET ด้วยการใช้ตัวดำเนินการ Boolean"
head_description: "API GroupDocs.Search for .NET ช่วยให้นักพัฒนา C# สามารถค้นหาสาระในเอกสารโดยใช้ตัวดำเนินการ Boolean เช่น AND, OR และ NOT."

############################# Header ############################
title: "การค้นหาข้อความด้วยตรรกศาสตร์ Boolean" 
description: "GroupDocs.Search for .NET ทำให้การสร้างคำค้นที่ซับซ้อนด้วยตัวดำเนินการ Boolean (AND, OR, NOT) ภายในแอพพลิเคชัน .NET ของคุณเป็นเรื่องที่ตรงไปตรงมา."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลดฟรี"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search คืออะไร?"
    link: "/search/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) คือห้องสมุดที่ครอบคลุมสำหรับการค้นหาและสร้างดัชนีข้อความในเอกสาร มันรองรับรูปแบบไฟล์มากกว่า 70 ประเภท เช่น PDF, Word, PowerPoint, Excel, ภาพถ่าย และไฟล์ ZIP ทำให้สามารถประมวลผลข้อมูลจำนวนมากได้อย่างมีประสิทธิภาพ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีค้นหาสาระในเอกสาร XLSX ด้วยตรรกศาสตร์ Boolean"
    content: |
      [GroupDocs.Search](/search/net/) ทำให้การค้นหาสาระในเอกสาร XLSX เป็นเรื่องที่ตรงไปตรงมา มันให้เงื่อนไขการค้นหาด้วยตรรกศาสตร์ Boolean เพื่อกรองผลลัพธ์ในแอพพลิเคชันต่าง ๆ ของ .NET.
      
      1. ระบุโฟลเดอร์เพื่อจัดเก็บดัชนีการค้นหา.
      2. เลือกโฟลเดอร์ที่มีไฟล์ XLSX.
      3. ดำเนินการค้นหาและเรียกคืนผลลัพธ์.
      4. ประมวลผลผลลัพธ์.
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "ผลการค้นหา"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "เอกสารประกอบ"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // ตั้งค่าพาธไปยังโฟลเดอร์ดัชนี
        Index index = new Index("c:/MyIndex");

        // ระบุโฟลเดอร์ที่มีเอกสารที่จะค้นหา
        index.Add("c:/MyDocuments");

        // ดำเนินการค้นหาด้วยการใช้คำค้นที่ซับซ้อน
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "สำรวจฟีเจอร์ขั้นสูงสำหรับการค้นหาและสร้างดัชนีเอกสาร"
  description: "ห้องสมุด GroupDocs.Search for .NET ทำให้การค้นหาและสร้างดัชนีข้อความสำหรับรูปแบบไฟล์มากกว่า 70 ประเภทเป็นเรื่องที่ไม่ซับซ้อน สามารถค้นหาและจัดการข้อมูลได้อย่างมีประสิทธิภาพด้วยเครื่องมือค้นหาขั้นสูง."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความที่ทรงพลัง"
      content: "ค้นหาข้อความในประเภทไฟล์ต่าง ๆ รวมถึง PDFs, เอกสาร Word, การนำเสนอ PowerPoint และสเปรดชีต ใช้ฟีเจอร์เช่นการจับคู่ที่แน่นอน, การค้นหาที่คลุมเครือ, และตัวอักขระพิเศษเพื่อปรับปรุงผลลัพธ์."

    # feature loop
    - title: "สร้างดัชนีข้อมูลชุดใหญ่"
      content: "สร้างและดูแลดัชนีเพื่อการค้นหาที่รวดเร็วขึ้น การสร้างดัชนีช่วยจัดระเบียบข้อมูลทำให้การค้นหาคอลเลคชันเอกสารขนาดใหญ่ทำได้ง่ายขึ้น."

    # feature loop
    - title: "รองรับหลายภาษา"
      content: "ค้นหาเอกสารในภาษามากกว่า 80 ภาษา โดยการสนับสนุนเลย์เอาต์คีย์บอร์ดที่แตกต่างกันและรูปแบบคำทางสัณฐานเพื่อเพิ่มความแม่นยำในการค้นหา."

    # feature loop
    - title: "ตัวเลือกการค้นหาที่ปรับแต่งได้"
      content: "ปรับแต่งการตั้งค่าการค้นหาด้วยฟีเจอร์เช่น ความละเอียดของตัวพิมพ์, ตัวกรองช่วงวันที่, และความสามารถในการยกเว้นคำหรือข้อมูลเฉพาะขณะสร้างดัชนี."
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้คำค้น Boolean ที่ทันสมัย"
      content: |
        ตัวอย่างนี้แสดงวิธีการใช้คำค้น Boolean สำหรับการค้นหาเอกสาร XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // ตั้งค่าโฟลเดอร์สำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // ระบุพาธไปยังเอกสารที่จะถูกค้นหา
          index.Add("c:/MyDocuments");

          // สร้างคำค้นด้วยตรรกศาสตร์ Boolean
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // เรียกคืนผลลัพธ์การค้นหา
          SearchResult result = index.Search(booleanQuery);
          
          // ประมวลผลผลลัพธ์การค้นหา
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "คัดลอก"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "คลิกเพื่อคัดลอก"
          copy_done: "คัดลอกแล้ว"
        top_links:
          #  loop
          - title: "ดาวน์โหลดผลลัพธ์"
            icon: "download"
            link: "/examples/search/formats/searchboolean.xlsx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "เอกสารประกอบ"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมที่จะเริ่มต้นแล้วหรือยัง?"
  description: "ทดลองฟีเจอร์ของ GroupDocs.Search ฟรีหรือขอใบอนุญาต"
  items:
    #  loop
    - title: "ดาวน์โหลด Nuget"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "การอนุญาต"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "ค้นพบฟีเจอร์หลัก"
    exclude: "boolean"
    description: "สำรวจฟังก์ชันการค้นหาที่มีประสิทธิภาพและทันสมัย."
    items: 
          
        # operation loop 1
        - name: "ค้นหาตามเงื่อนไข"
          operation: "boolean"
          link: "/search/net/boolean/xlsx/"
          description: "ค้นหาข้อมูลในเอกสารโดยใช้เงื่อนไขเชิงบูลีน"

        # operation loop 2
        - name: "การค้นหาตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/xlsx/"
          description: "เพิ่มความแม่นยำในการค้นหาด้วยการพิจารณาความแตกต่างของตัวพิมพ์"

        # operation loop 3
        - name: "การจัดทำดัชนีเอกสาร"
          operation: "document"
          link: "/search/net/document/xlsx/"
          description: "จัดทำดัชนีเอกสารเพียงครั้งเดียวและนำกลับมาใช้ใหม่สำหรับการค้นหาหลายครั้ง"

        # operation loop 4
        - name: "ตัวกรองการค้นหา"
          operation: "filters"
          link: "/search/net/filters/xlsx/"
          description: "ใช้ตัวกรองเพื่อลดปริมาณข้อมูลที่ถูกประมวลผล"

        # operation loop 5
        - name: "ประโยคที่แน่นอน"
          operation: "phrase"
          link: "/search/net/phrase/xlsx/"
          description: "ค้นหาประโยคหรือลำดับคำเฉพาะ"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหาในรูปแบบเอกสารยอดนิยม"
    exclude: "XLSX"
    description: "GroupDocs.Search รองรับรูปแบบไฟล์มากกว่า 70 ประเภท ปรับแต่งกฎการค้นหาและใช้การสร้างดัชนีเพื่อประหยัดเวลาและความพยายาม."
    items: 
        # format loop 1
        - name: "ค้นหาตามเงื่อนไขใน DOCX"
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "ค้นหาตามเงื่อนไขใน PDF"
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "ค้นหาตามเงื่อนไขใน PPTX"
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "ค้นหาตามเงื่อนไขใน TXT"
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "ค้นหาตามเงื่อนไขใน XLSX"
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---