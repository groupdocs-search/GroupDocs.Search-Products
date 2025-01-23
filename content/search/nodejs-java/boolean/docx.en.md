
---
############################# Static ############################
layout: "format"
date:  2025-01-23T10:13:32
draft: false
lang: en
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Generate barcode for DOCX using JavaScript Applications"
head_description: "Quickly generate and embed a barcode signature in a DOCX document with JavaScript using just a few lines of code. GroupDocs.Search supports signing across multiple file formats."

############################# Header ############################
title: "Generate and add Barcodes in DOCX effortlessly" 
description: "Employ GroupDocs.Search for Node.js via Java to incorporate barcodes into your business documents, placing them precisely where needed. Our solution offers extensive customization options to tailor barcode signatures to your requirements."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Download Now – It's Free!"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "An introduction to GroupDocs.Search for Node.js via Java"
    link: "/search/nodejs-java/"
    link_title: "Learn more"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) is a powerful document signing tool, supporting a diverse range of signature types including text, images, barcodes, digital certificates, and stamps. With compatibility across more than 60 file formats, such as PDFs, MS Office files, images, and ZIP archives, it allows for comprehensive document management. Signatures within documents can be searched, verified, altered, or removed as required.

############################# Steps ############################
steps:
    enable: true
    title: "How to generate and embed barcodes in DOCX file"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) enables the generation and placement of barcodes in a variety of popular formats on DOCX pages. With support for over 60 types of barcodes, Node.js via Java applications can be easily enhanced with barcode signing features by integrating our library.
      
      1. Provide the DOCX file or stream for processing.
      2. Pass the barcode text to a {{BarcodeSignOptions}} instance.
      3. Adjust barcode settings such as position, size, etc.
      4. Save the document with the newly added barcode.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copy"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Search result"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "click to copy"
        copy_done: "copied"
      links:
        #  loop
        - title: "More examples"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Documentation"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Instantiate a {{TextSignature}} object with the document path
        const signature = new signatureLib.Signature('input.docx');

        // Utilize {{BarcodeSignOptions}} to integrate a barcode into the document
        const options = new signatureLib.BarcodeSignOptions('Business data');

        // Configure the barcode type and additional parameters
        options.setEncodeType(signatureLib.BarcodeTypes.Code128);
        options.setLeft(100);
        options.setTop(100);
  
        // Save the signed document
        signature.sign('output.docx', options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Augment and secure your documents with advanced signature options"
  description: "The GroupDocs.Search for Node.js via Java library is designed to streamline the signing and subsequent management of popular document formats. Quickly and easily add, modify, verify, or remove a wide range of signatures."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Key Functionalities of GroupDocs.Search"
  features:
    # feature loop
    - title: "Dynamic document signing"
      content: "Sign any page of your documents using a variety of signature types, including text, images, barcodes, QR codes, and stamps. Additionally, you can embed hidden metadata, such as EXIF data in images, or secure the document against unauthorized edits using digital certificates."

    # feature loop
    - title: "Robust signature verification and search"
      content: "Our solution provides extensive tools for managing signed documents. Verify the authenticity of signatures to ensure document integrity, and utilize the search feature to list all signatures embedded within a document."

    # feature loop
    - title: "Easily edit signatures"
      content: "Most signatures added previously can be effortlessly modified. Update the text, reposition, or change the appearance of the signature to match your needs."

    # feature loop
    - title: "Streamlined signature removal"
      content: "With comprehensive support for CRUD operations, our tool allows for the efficient removal of signatures from your documents, ensuring that only the most relevant signatures remain."
      
  code_samples_ext:
    # code sample ext loop
    - title: "How to apply a barcode signature"
      content: |
        This example illustrates how to embed a customized barcode on DOCX document pages.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Provide the document to be signed
          const signature = new signatureLib.Signature('input.docx');

          // Utilize {{BarcodeSignOptions}} to integrate a barcode into the document
          const signOptions = new signatureLib.BarcodeSignOptions('Accepted');
          signOptions.setEncodeType(signatureLib.BarcodeTypes.Code39FullASCII);

          // Configure the barcode type and additional parameters
          signOptions.setVerticalAlignment(signatureLib.VerticalAlignment.Bottom);
          signOptions.setHorizontalAlignment(signatureLib.HorizontalAlignment.Left);

          // Define the barcode padding from the page edge
          const padding = new signatureLib.Padding();
          padding.setLeft(20);
          padding.setTop(180);
          signOptions.setMargin(padding);

          // Choose the bar color
          signOptions.setForeColor(signatureLib.Color.RED);

          // Specify the font style for the message
          const font = new signatureLib.SignatureFont();
          font.setSize(12);
          font.setFamilyName('Arial');
          signOptions.setFont(font);

          // Indicate the position of the message
          signOptions.setCodeTextAlignment(signatureLib.CodeTextAlignment.Above);

          // Sign and save the document
          signature.sign('output.docx', signOptions);

          ```
        platform: "nodejs-java"
        copy_title: "Copy"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "click to copy"
          copy_done: "copied"
        top_links:
          #  loop
          - title: "Download result"
            icon: "download"
            link: "/examples/search/formats/searchboolean.docx"
        links:
          #  loop
          - title: "More examples"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Documentation"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Ready to get started?"
  description: "Try GroupDocs.Search features for free or request a license"
  items:
    #  loop
    - title: "NPM download"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licensing"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Dive into our primary features"
    exclude: "boolean"
    description: "Experience a broad array of signature types and tools we provide"
    items: 
          
        # operation loop 1
        - name: "Search by condition"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Find information in documents using boolean conditions"

        # operation loop 2
        - name: "Case-sensitive search"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Improve search accuracy by considering case sensitivity"

        # operation loop 3
        - name: "Document indexing"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "Index documents once and reuse the index for multiple searches"

        # operation loop 4
        - name: "Search filters"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "Use filters to narrow down the data being processed"

        # operation loop 5
        - name: "Exact phrase"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Search for a specific sentence or phrase"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Sign across multiple document formats"
    exclude: "DOCX"
    description: "The Node.js via Java API empowers you to sign over 60 different formats. Whether adding signatures to specific pages or positioning them precisely, our tool makes it easy to apply various signature types."
    items: 
        # format loop 1
        - name: "Search in DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Microsoft Word Open XML Document"
          
        # format loop 2
        - name: "Search in PDF"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "Search in PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "PowerPoint Open XML Presentation"

        # format loop 4
        - name: "Search in TXT"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Text Document"
          
        # format loop 5
        - name: "Search in XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Microsoft Excel Open XML Spreadsheet"
  

---