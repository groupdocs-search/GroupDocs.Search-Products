
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: th
format: Pdf
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "ค้นหาวลีใน PDF ด้วย .NET"
head_description: "GroupDocs.Search for .NET เสริมสร้างแอปพลิเคชัน C# ด้วยความสามารถในการค้นหาวลีที่ทรงพลังสำหรับเนื้อหาของเอกสาร."

############################# Header ############################
title: "ค้นหาวลีในเอกสาร" 
description: "ค้นหาวลีที่เฉพาะเจาะจงได้อย่างรวดเร็วด้วย GroupDocs.Search for .NET บูรณาการฟังก์ชันการค้นหาที่มีประสิทธิภาพในแอปพลิเคชัน .NET ของคุณ."
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ดาวน์โหลด"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search ฟีเจอร์"
    link: "/search/net/"
    link_title: "เรียนรู้เพิ่มเติม"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) เป็นห้องสมุดที่ทรงพลังสำหรับการจัดทำดัชนีและค้นหาข้อความในเอกสาร รองรับกว่า 70 รูปแบบไฟล์ รวมถึง PDF เอกสาร Word แผ่น Excel รูปภาพ และไฟล์ ZIP ทำให้สามารถค้นหาได้อย่างรวดเร็วและแม่นยำ.

############################# Steps ############################
steps:
    enable: true
    title: "วิธีการค้นหาวลีในเอกสาร PDF"
    content: |
      [GroupDocs.Search](/search/net/) ช่วยให้ง่ายต่อการค้นหาในเอกสาร PDF ใช้ตัวเลือกต่างๆ เพื่อลดความไม่แน่นอนของผลลัพธ์การค้นหาในแอปพลิเคชัน .NET.
      
      1. ตั้งค่าโฟลเดอร์สำหรับดัชนีการค้นหา.
      2. ระบุโฟลเดอร์ที่มีไฟล์ PDF.
      3. กำหนดค่าการตั้งค่าการค้นหา.
      4. ดึงและประมวลผลผลลัพธ์การค้นหา.
   
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
        // เส้นทางในการจัดเก็บดัชนีการค้นหา
        Index index = new Index("c:/MyIndex");

        // โฟลเดอร์ที่มีเอกสาร
        index.Add("c:/MyDocuments");

        // กำหนดค่าตัวเลือกการค้นหา
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // ดำเนินการค้นหา
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "ค้นพบเครื่องมือค้นหาเอกสาร .NET"
  description: "GroupDocs.Search for .NET สามารถทำการค้นหาวลีในกว่า 70 รูปแบบไฟล์ ค้นหาและจัดการข้อมูลได้อย่างมีประสิทธิภาพด้วยความสามารถในการค้นหาขั้นสูง."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "ฟีเจอร์หลักของ GroupDocs.Search"
  features:
    # feature loop
    - title: "การค้นหาวลี"
      content: "ค้นหาวลีที่แน่นอนในเอกสารทางธุรกิจ รวมถึง PDF เอกสาร Word งานนำเสนอ และแผ่นงาน ใช้ตัวแทนไวลด์การ์ดและตัวเลือกอื่นๆ หากไม่ทราบวลีที่แน่นอน."

    # feature loop
    - title: "การจัดทำดัชนีข้อมูลที่มีประสิทธิภาพ"
      content: "สร้างและนำกลับมาใช้ดัชนีการค้นหาเพื่อเร่งความเร็วในการค้นหาเอกสาร การจัดทำดัชนีจะจัดระเบียบข้อมูลอย่างมีประสิทธิภาพ ทำให้การค้นหาวลีรวดเร็วยิ่งขึ้น."

    # feature loop
    - title: "การสนับสนุนหลายภาษา"
      content: "ค้นหาเอกสารในกว่า 80 ภาษา รองรับการตั้งค่าคีย์บอร์ดที่แตกต่างกันและรูปแบบทางสัณฐานสำหรับความแม่นยำในการค้นหาที่ดียิ่งขึ้น."

    # feature loop
    - title: "ตัวเลือกการค้นหาที่ยืดหยุ่น"
      content: "ปรับแต่งการค้นหาด้วยฟีเจอร์ต่างๆ เช่น ความไวต่อการพิมพ์ตัวพิมพ์ใหญ่ ความไม่แม่นยำ และการค้นหาเสียงพ้อง การกรองเอกสาร และอื่นๆ."
      
  code_samples_ext:
    # code sample ext loop
    - title: "การใช้เทคนิคการค้นหาขั้นสูง"
      content: |
        เรียนรู้วิธีสร้างคำค้นเพื่อค้นหาใน PDF.
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // ระบุโฟลเดอร์สำหรับดัชนีการค้นหา
          Index index = new Index("c:/MyIndex");
              
          // ตั้งค่าเส้นทางไปยังเอกสารสำหรับการค้นหา
          index.Add("c:/MyDocuments");

          // สร้างคำค้นสำหรับวลีเฉพาะ
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // ดึงผลลัพธ์การค้นหา
          SearchResult result = index.Search(query);
          
          // ประมวลผลและนำผลลัพธ์ไปใช้
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
            link: "/examples/search/formats/searchphrase.pdf"
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
    title: "ฟีเจอร์ขั้นสูง"
    exclude: "phrase"
    description: "ใช้ฟังก์ชันการค้นหาที่ยิ่งใหญ่และมีประสิทธิภาพ."
    items: 
          
        # operation loop 1
        - name: "ค้นหาตามเงื่อนไข"
          operation: "boolean"
          link: "/search/net/boolean/pdf/"
          description: "ค้นหาข้อมูลในเอกสารโดยใช้เงื่อนไขเชิงบูลีน"

        # operation loop 2
        - name: "การค้นหาตัวพิมพ์ใหญ่ตัวพิมพ์เล็ก"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/pdf/"
          description: "เพิ่มความแม่นยำในการค้นหาด้วยการพิจารณาความแตกต่างของตัวพิมพ์"

        # operation loop 3
        - name: "การจัดทำดัชนีเอกสาร"
          operation: "document"
          link: "/search/net/document/pdf/"
          description: "จัดทำดัชนีเอกสารเพียงครั้งเดียวและนำกลับมาใช้ใหม่สำหรับการค้นหาหลายครั้ง"

        # operation loop 4
        - name: "ตัวกรองการค้นหา"
          operation: "filters"
          link: "/search/net/filters/pdf/"
          description: "ใช้ตัวกรองเพื่อลดปริมาณข้อมูลที่ถูกประมวลผล"

        # operation loop 5
        - name: "ประโยคที่แน่นอน"
          operation: "phrase"
          link: "/search/net/phrase/pdf/"
          description: "ค้นหาประโยคหรือลำดับคำเฉพาะ"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "การค้นหาวลีในเอกสารทางธุรกิจ"
    exclude: "PDF"
    description: "GroupDocs.Search สนับสนุนการค้นหาใน 70+ รูปแบบเอกสาร ใช้ตัวเลือกขั้นสูงและการจัดทำดัชนีเพื่อลดความซับซ้อนในกระบวนการค้นหาของคุณ."
    items: 
        # format loop 1
        - name: "การค้นหาประโยคใน DOCX"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "เอกสาร Microsoft Word Open XML"
          
        # format loop 2
        - name: "การค้นหาประโยคใน PDF"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "รูปแบบเอกสารที่พกพาของ Adobe"
          
        # format loop 3
        - name: "การค้นหาประโยคใน PPTX"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "การนำเสนอ PowerPoint Open XML"

        # format loop 4
        - name: "การค้นหาประโยคใน TXT"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "เอกสารข้อความ"
          
        # format loop 5
        - name: "การค้นหาประโยคใน XLSX"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "สเปรดชีต Microsoft Excel Open XML"
  

---