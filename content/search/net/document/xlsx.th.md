
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: th
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ค้นหาเอกสาร XLSX ใน .NET ด้วย GroupDocs.Search"
head_description: "ใช้ GroupDocs.Search for .NET เพื่อทำการค้นหาข้อความที่มีประสิทธิภาพในรูปแบบเอกสารต่างๆ โดยใช้ C#."

############################# Header ############################
title: "การค้นหาข้อความในเอกสารขั้นสูง" 
description: "GroupDocs.Search for .NET ทำให้การค้นหาข้อความในรูปแบบเอกสารยอดนิยมง่ายขึ้น ช่วยให้คุณสร้างการค้นหาที่ทรงพลังในแอปพลิเคชัน .NET ของคุณ."
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
       [GroupDocs.Search for .NET](/search/net/) เป็นห้องสมุดที่ทรงพลังสำหรับการค้นหาและจัดทำดัชนีข้อความในเอกสาร รองรับไฟล์กว่า 70 รูปแบบ รวมถึง PDF, Word, PowerPoint, Excel, รูปภาพ และไฟล์ ZIP เพื่อให้ผลลัพธ์การค้นหาที่รวดเร็วและแม่นยำ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการค้นหาข้อความในเอกสาร XLSX"
    content: |
      [GroupDocs.Search](/search/net/) ช่วยให้สามารถดำเนินการค้นหาขั้นสูงในเอกสาร XLSX ได้ โดยช่วยให้ได้ผลลัพธ์การค้นหาที่ปรับปรุงในแอปพลิเคชัน .NET.
      
      1. ตั้งค่าโฟลเดอร์สำหรับจัดเก็บดัชนีการค้นหา.
      2. เลือกโฟลเดอร์ที่มีไฟล์ XLSX.
      3. กำหนดค่าตัวเลือกการค้นหาเพิ่มเติม.
      4. เรียกใช้การค้นหาและตรวจสอบผลลัพธ์.
   
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
        // กำหนดเส้นทางสำหรับดัชนีการค้นหา
        Index index = new Index("c:/MyIndex");

        // เลือกโฟลเดอร์ที่มีเอกสารที่จะค้นหา
        index.Add("c:/MyDocuments");

        // เปิดใช้งานการค้นหาคำพ้องเสียงเพื่อค้นหาคำที่มีเสียงเหมือนกัน
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // ดำเนินการค้นหาที่ซับซ้อน
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ฟีเจอร์การค้นหาและการจัดทำดัชนีที่ล้ำสมัย"
  description: "GroupDocs.Search for .NET เพิ่มประสิทธิภาพการค้นหาและการจัดทำดัชนีในรูปแบบเอกสารกว่า 70 รูปแบบ มอบเครื่องมือที่มีประสิทธิภาพในการค้นหาและจัดการข้อมูล."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความที่ทรงพลัง"
      content: "ค้นหาข้อความในหลายประเภทเอกสาร รวมถึง PDF, เอกสาร Word, งานนำเสนอ PowerPoint และสเปรดชีต ใช้ฟีเจอร์เช่นการค้นหาแบบตรง, การค้นหาที่คลุมเครือ และอักขระแทนเพื่อปรับปรุงผลลัพธ์ของคุณ."

    # feature loop
    - title: "การจัดทำดัชนีที่รวดเร็วสำหรับชุดข้อมูลขนาดใหญ่"
      content: "สร้างและจัดการดัชนีการค้นหาสำหรับการดึงข้อมูลอย่างรวดเร็ว การจัดทำดัชนีช่วยเพิ่มประสิทธิภาพการค้นหาในคอลเลกชันเอกสารขนาดใหญ่."

    # feature loop
    - title: "การสนับสนุนหลายภาษา"
      content: "ทำการค้นหาในมากกว่า 80 ภาษา โดยรองรับรูปแบบคีย์บอร์ดที่แตกต่างกันและรูปแบบคำที่แตกต่างกันเพื่อปรับปรุงความแม่นยำ."

    # feature loop
    - title: "การตั้งค่าการค้นหาที่ปรับแต่งได้"
      content: "ปรับแต่งพารามิเตอร์การค้นหาด้วยตัวเลือก เช่น ความไวต่อพิมพ์ใหญ่พิมพ์เล็ก, ตัวกรองช่วงวัน และการตัดคำเพื่อผลลัพธ์ที่ดีกว่า."
      
  code_samples_ext:
    # code sample ext loop
    - title: "การดำเนินการค้นหาที่ซับซ้อน"
      content: |
        ตัวอย่างนี้แสดงวิธีการใช้คำค้นสำหรับเอกสาร XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // กำหนดโฟลเดอร์สำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // ระบุเส้นทางไปยังไฟล์เอกสาร
          index.Add("c:/MyDocuments");

          // กำหนดรหัสผ่านสำหรับเอกสารที่ป้องกัน
          index.Dictionaries.DocumentPasswords.Add("protected.xlsx", "123456");

          // เปิดใช้งานการค้นหาคลุมเครือเพื่อค้นหาคำที่คล้ายกัน
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // ดึงผลลัพธ์การค้นหา
          SearchResult result = index.Search("Loarem", options);
          
          // ประมวลผลเอาต์พุตการค้นหา
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
            link: "/examples/search/formats/searchdocument.xlsx"
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
    title: "สำรวจฟีเจอร์หลัก"
    exclude: "document"
    description: "ใช้ประโยชน์จากฟังก์ชันการค้นหาที่ล้ำสมัยและมีประสิทธิภาพสูง."
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
    title: "ค้นหาผ่านเอกสารทางธุรกิจของคุณ"
    exclude: "XLSX"
    description: "GroupDocs.Search รองรับรูปแบบเอกสารมากกว่า 70 รูปแบบ รวมถึงเอกสารสำนักงาน เพื่อให้การค้นหาที่รวดเร็วและมีประสิทธิภาพพร้อมความสามารถในการจัดทำดัชนี."
    items: 
        # format loop 1
        - name: "ค้นหาในเอกสาร DOCX"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "ค้นหาในเอกสาร PDF"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "ค้นหาในเอกสาร PPTX"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "ค้นหาในเอกสาร TXT"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "ค้นหาในเอกสาร XLSX"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---