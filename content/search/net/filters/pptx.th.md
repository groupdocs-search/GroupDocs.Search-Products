
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: th
format: Pptx
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ค้นหาในเอกสาร PPTX ด้วย .NET"
head_description: "GroupDocs.Search for .NET เพิ่มประสิทธิภาพให้กับแอปพลิเคชัน C# ด้วยการค้นหาข้อความที่มีประสิทธิภาพในรูปแบบเอกสารธุรกิจต่าง ๆ"

############################# Header ############################
title: "ค้นหาข้อความในเอกสารธุรกิจ" 
description: "GroupDocs.Search for .NET ช่วยให้คุณค้นหาข้อความในเอกสารได้อย่างมีประสิทธิภาพและยืดหยุ่น สามารถรวมฟังก์ชันการค้นหาเข้าในแอปพลิเคชัน .NET ได้อย่างง่ายดาย"
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
       [GroupDocs.Search for .NET](/search/net/) เป็นไลบรารีที่มีประสิทธิภาพสำหรับการค้นหาข้อความและการทำดัชนีเอกสารอย่างมีประสิทธิภาพ รองรับรูปแบบไฟล์มากกว่า 70 รูปแบบ รวมถึงเอกสารมาตรฐานในอุตสาหกรรม เช่น PDF, Word, Excel และ PowerPoint ปรับปรุงประสิทธิภาพการค้นหาด้วยผลลัพธ์ที่รวดเร็วและแม่นยำ

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการค้นหาข้อมูลในเอกสาร PPTX"
    content: |
      [GroupDocs.Search](/search/net/) ช่วยให้การค้นหาข้อความในเอกสาร PPTX มีประสิทธิภาพ ทำให้เหมาะสำหรับแอปพลิเคชัน .NET
      
      1. ตั้งค่าโฟลเดอร์สำหรับจัดเก็บดัชนีการค้นหา
      2. เลือกโฟลเดอร์ที่มีไฟล์ของคุณ
      3. กำหนดค่าเลือกตัวเลือกการค้นหาเพื่อประมวลผลเฉพาะเอกสาร PPTX
      4. ดำเนินการค้นหาและเรียกคืนผลลัพธ์
   
    code:
      platform: "net"
      copy_title: "คัดลอก"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "คลิกเพื่อคัดลอก"
        copy_done: "คัดลอกแล้ว"
      links:
        #  loop
        - title: "ตัวอย่างเพิ่มเติม"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "เอกสาร"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // เส้นทางในการจัดเก็บดัชนีการค้นหาที่สามารถนำกลับมาใช้ใหม่ได้
        Index index = new Index("c:/MyIndex");

        // โฟลเดอร์ที่มีเอกสาร
        index.Add("c:/MyDocuments");

        // ค้นหาเฉพาะในรูปแบบไฟล์ที่กำหนด
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".pptx");

        // เรียกคืนผลลัพธ์การค้นหา
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ฟังก์ชันการค้นหาขั้นสูง"
  description: "GroupDocs.Search for .NET ช่วยให้สามารถค้นหาข้อความที่ซับซ้อนได้ในกว่า 70 รูปแบบไฟล์ การทำดัชนีช่วยเพิ่มประสิทธิภาพในการค้นหาและจัดการเนื้อหาเอกสารได้อย่างมีประสิทธิภาพ"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาข้อความขั้นสูง"
      content: "ดึงข้อมูลข้อความที่เกี่ยวข้องจากเอกสารธุรกิจยอดนิยม รวมถึง PDFs, ไฟล์ Word, งานนำเสนอ และสเปรดชีต รองรับเทคนิคการค้นหาหลายรูปแบบ เช่น การค้นหาหมายเหตุ, การตรวจจับเสียงที่คล้ายกัน และอักขระตัวแทน"

    # feature loop
    - title: "การทำดัชนีที่ปรับให้เหมาะสมเพื่อค้นหาที่รวดเร็วขึ้น"
      content: "สร้างและนำดัชนีการค้นหามาใช้ใหม่เพื่อเพิ่มความเร็วในการค้นหา การทำดัชนีช่วยเพิ่มประสิทธิภาพเมื่อค้นหาผ่านคอลเล็กชันเอกสารขนาดใหญ่"

    # feature loop
    - title: "รองรับหลายภาษา"
      content: "ดำเนินการค้นหาในเอกสารที่เขียนในกว่า 80 ภาษา ตรวจจับรูปแบบคีย์บอร์ดที่แตกต่างกันและความแปรปรวนของคำเพื่อเพิ่มความแม่นยำ"

    # feature loop
    - title: "การตั้งค่าการค้นหาที่ยืดหยุ่น"
      content: "ปรับแต่งผลลัพธ์การค้นหาด้วยตัวเลือกที่กำหนดเอง รวมถึงการกรอง, นิพจน์ปกติ, และการตั้งค่าความไวต่อกรณี"
      
  code_samples_ext:
    # code sample ext loop
    - title: "กรองเอกสารที่จะประมวลผล"
      content: |
        เรียนรู้วิธีการจำกัดการค้นหาเอกสารด้วยการกรอง
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // ตั้งค่าดัชนีที่ไม่รวมรูปแบบไฟล์บางประเภท
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // ระบุไดเรกทอรีเอกสาร
          index.Add("c:/MyDocuments");

          // เรียกคืนผลลัพธ์การค้นหา
          SearchResult result = index.Search("Lorem");
          
          // ประมวลผลและใช้ผลลัพธ์การค้นหา
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.pptx"
        links:
          #  loop
          - title: "ตัวอย่างเพิ่มเติม"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "เอกสาร"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "พร้อมเริ่มต้นแล้วหรือยัง?"
  description: "ทดลองคุณสมบัติของ GroupDocs.Search ฟรี หรือขอใบอนุญาต"
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
    title: "ฟังก์ชันหลัก"
    exclude: "filters"
    description: "ดำเนินการค้นข้อมูลที่แม่นยำและมีประสิทธิภาพ"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ค้นหาข้อมูลในเอกสารธุรกิจของคุณ"
    exclude: "PPTX"
    description: "GroupDocs.Search รองรับ 70+ รูปแบบไฟล์ ช่วยให้การประมวลผลและค้นหาเอกสารสำนักงานยอดนิยมมีประสิทธิภาพ"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "รูปแบบเอกสารพกพา Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---