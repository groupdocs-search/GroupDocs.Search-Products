
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: th
format: Xlsx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "การค้นหาที่ไวต่อการพิมพ์ใน XLSX โดยใช้ .NET"
head_description: "API ของ GroupDocs.Search for .NET ช่วยให้นักพัฒนา C# สามารถทำการค้นหาที่ไวต่อการพิมพ์ในเอกสารต่างๆ ได้."

############################# Header ############################
title: "การค้นหาที่ไวต่อการพิมพ์" 
description: "GroupDocs.Search for .NET ช่วยให้คุณสร้างคำค้นหาที่ไวต่อการพิมพ์ในแอปพลิเคชัน .NET ของคุณได้."
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
       [GroupDocs.Search for .NET](/search/net/) เป็นห้องสมุดที่มีประสิทธิภาพสำหรับการค้นหาและการทำดัชนีข้อความในเอกสาร รองรับมากกว่า 70 รูปแบบไฟล์ รวมถึง PDF, Word, PowerPoint, Excel, รูปภาพ และไฟล์ ZIP เพื่อให้การจัดการข้อมูลขนาดใหญ่มีประสิทธิภาพ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการค้นหาที่ไวต่อการพิมพ์ในเอกสาร XLSX"
    content: |
      [GroupDocs.Search](/search/net/) ช่วยให้การค้นหาที่ไวต่อการพิมพ์ในเอกสาร XLSX เป็นไปอย่างราบรื่น ใช้เพื่อปรับผลลัพธ์ในแอปพลิเคชัน .NET.
      
      1. กำหนดโฟลเดอร์สำหรับจัดเก็บดัชนีการค้นหา.
      2. เลือกโฟลเดอร์ที่มีไฟล์ XLSX.
      3. ดำเนินการค้นหาและเรียกดูผลลัพธ์.
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
        // กำหนดเส้นทางไปยังโฟลเดอร์ดัชนี
        Index index = new Index("c:/MyIndex");

        // ระบุโฟลเดอร์ที่มีเอกสารที่จะค้นหา
        index.Add("c:/MyDocuments");

        // เปิดใช้งานการค้นหาที่ไวต่อการพิมพ์ในตัวเลือก
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // ดำเนินการค้นหา
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ฟีเจอร์ขั้นสูงสำหรับการค้นหาและการทำดัชนีเอกสาร"
  description: "ห้องสมุด GroupDocs.Search for .NET ช่วยให้การค้นหาและการทำดัชนีข้อความในรูปแบบไฟล์มากกว่า 70 รูปแบบเป็นไปอย่างง่ายดาย สามารถค้นหาและจัดการข้อมูลด้วยเครื่องมือค้นหาที่ทรงพลัง."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "ฟีเจอร์สำคัญของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความขั้นสูง"
      content: "ค้นหาข้อความในรูปแบบไฟล์ต่างๆ รวมถึง PDF, เอกสาร Word, สเปรดชีต และนำเสนอ โดยใช้ตัวเลือกเช่น การจับคู่ที่แน่นอน, การค้นหาแบบ fuzzy และอักขระแทนสำหรับผลลัพธ์ที่แม่นยำ."

    # feature loop
    - title: "ทำดัชนีชุดข้อมูลขนาดใหญ่"
      content: "สร้างและดูแลดัชนีเพื่อการค้นหาที่รวดเร็ว การจัดระเบียบดัชนีช่วยให้การค้นหาชุดเอกสารขนาดใหญ่เป็นไปอย่างมีประสิทธิภาพ."

    # feature loop
    - title: "รองรับหลายภาษา"
      content: "ค้นหาในเอกสารได้กว่า 80 ภาษา โดยมีการรองรับเลย์เอาต์แป้นพิมพ์และรูปแบบคำที่แตกต่างกันเพื่อผลลัพธ์ที่แม่นยำยิ่งขึ้น."

    # feature loop
    - title: "ตัวเลือกการค้นหาที่ปรับแต่งได้"
      content: "ปรับแต่งการตั้งค่าการค้นหาด้วยความไวต่อการพิมพ์, ตัวกรองช่วงวันที่ และความสามารถในการละเว้นคำหรือข้อมูลเฉพาะระหว่างการทำดัชนี."
      
  code_samples_ext:
    # code sample ext loop
    - title: "ใช้คำค้นหาที่ไวต่อการพิมพ์"
      content: |
        ตัวอย่างนี้แสดงให้เห็นถึงการใช้คำค้นหาที่ไวต่อการพิมพ์ในการค้นหาเอกสาร XLSX.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // กำหนดโฟลเดอร์สำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // ระบุเส้นทางไปยังเอกสารที่ต้องค้นหา
          index.Add("c:/MyDocuments");

          // สร้างคำค้นหาขึ้นมา
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // เปิดใช้งานตัวเลือกการค้นหาที่ไวต่อการพิมพ์
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // ค้นหาข้อความในเอกสาร
          SearchResult result = index.Search(wordQuery, options);
          
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
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
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
    title: "ค้นพบฟีเจอร์สำคัญ"
    exclude: "case-sensitive"
    description: "สำรวจฟังก์ชันการค้นหาที่มีประสิทธิภาพและขั้นสูง."
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
    title: "ค้นหารูปแบบเอกสารที่เป็นที่นิยม"
    exclude: "XLSX"
    description: "GroupDocs.Search รองรับมากกว่า 70 รูปแบบไฟล์ ปรับแต่งกฎการค้นหาและใช้การทำดัชนีเพื่อลดเวลาและความพยายาม."
    items: 
        # format loop 1
        - name: "การค้นหา DOCX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "การค้นหา PDF ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "การค้นหา PPTX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "การค้นหา TXT ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "การค้นหา XLSX ตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---