
---
############################# Static ############################
layout: "format"
date:  2025-01-23T10:13:32
draft: false
lang: en
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Search Queries using Boolean Operators (AND, OR, NOT) via Java"
head_description: "Create and insert barcode signatures into XLSX documents in Java with ease. GroupDocs.Search enables versatile signature integration for multiple formats."

############################# Header ############################
title: "Generate barcode for XLSX" 
description: "Add barcodes of popular formats to any position in your business documents with GroupDocs.Search for Java. Our solution provides extensive options to customize barcode signatures."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download for Free"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "About GroupDocs.Search for Java"
    link: "/search/java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) is an advanced signing solution that supports a wide range of signature types. You can sign documents with text, images, barcodes, digital certificates, stamps, and more across 60+ file formats, including PDF, MS Office, images, ZIP files, and other popular business formats. Additionally, signatures in signed documents can be searched, verified, modified, or deleted at any time.

############################# Steps ############################
steps:
    enable: true
    title: "Steps to generate and add a barcode to XLSX file"
    content: |
      [GroupDocs.Search](/search/java/) can generate barcodes in various popular formats and place them on XLSX pages. With support for over 60 barcode types, Java applications can easily be enhanced with barcode signing capabilities by incorporating our library.
      
      1. Provide the XLSX file or stream to be processed.
      2. Pass the barcode text to the {{BarcodeSignOptions}} instance.
      3. Customize barcode options such as position, size, etc.
      4. Save the file with the newly added barcode.
   
    code:
      platform: "java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Search result"
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
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Create a new {{TextSignature}} instance with the document path
        Signature signature = new Signature("input.xlsx");

        // Use {{BarcodeSignOptions}} to add a barcode to the document
        BarcodeSignOptions options = new BarcodeSignOptions("Business data");

        // Set up the barcode type and other properties
        options.setEncodeType(BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);

        // Save the signed file
        signature.sign("output.xlsx", options);

        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Enhance or protect document content with signatures"
  description: "The GroupDocs.Search for Java library is designed for signing and further processing popular file formats. Quickly and easily add, modify, verify, or delete various types of signatures."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Features of GroupDocs.Search"
  features:
    # feature loop
    - title: "Document signing"
      content: "Sign any page of supported documents with text, images, barcodes, QR codes, or stamps. Add hidden metadata like EXIF in images or protect document content from unauthorized changes using digital certificates."

    # feature loop
    - title: "Signature search and verification"
      content: "There’s much more you can do with a signed document. We offer verification of signatures to ensure everything is in order. Additionally, you can retrieve a list of all document signatures through a search."

    # feature loop
    - title: "Modify signatures"
      content: "Most previously added signatures can be modified. Easily correct text, adjust position, or change color."

    # feature loop
    - title: "Delete signatures"
      content: "Our solution supports full CRUD operations for signatures. Many types of signatures can be deleted from a document when necessary."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to create a barcode signature"
      content: |
        This example demonstrates how to place a customized barcode on XLSX document pages.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Provide the document to be signed
          Signature signature = new Signature("input.xlsx");

          // Create signature options with the desired text
          BarcodeSignOptions signOptions = new BarcodeSignOptions("Accepted");
          signOptions.setEncodeType(BarcodeTypes.Code39FullASCII);

          // Set the relative barcode position on the page
          signOptions.setVerticalAlignment(VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(HorizontalAlignment.Left);

          // Set the barcode padding from the page edge
          Padding padding = new Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Set the color of the bars
          signOptions.setForeColor(Color.RED);

          // Define the message font style
          SignatureFont font = new SignatureFont();
          font.setSize(12);
          font.setFamilyName("Arial");
          signOptions.setFont(font);

          // Specify the message position
          signOptions.setCodeTextAlignment(CodeTextAlignment.Above);

          // Sign and save the document
          SignResult signResult = signature.sign("output.xlsx", signOptions);

          ```
        platform: "java"
        copy_title: "Copy"
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
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/search/formats/search_boolean.xlsx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"
  items:
    #  loop
    - title: "Maven download"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Discover our core capabilities"
    exclude: "boolean"
    description: "We proudly present an extensive variety of supported signatures and functions"
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/java/boolean/xlsx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/java/document/xlsx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/java/filters/xlsx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/java/phrase/xlsx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sign documents in other formats"
    exclude: "XLSX"
    description: "Over 60 formats can be signed using our Java API. Apply various signatures to any page or position within the document."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---