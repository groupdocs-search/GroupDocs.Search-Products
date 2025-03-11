
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: es
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Buscar en documentos DOCX utilizando Node.js"
head_description: "GroupDocs.Search for Node.js via Java agrega capacidades de búsqueda de texto rápidas y precisas a aplicaciones JavaScript, soportando múltiples formatos de documentos."

############################# Header ############################
title: "Encuentra texto en documentos empresariales" 
description: "GroupDocs.Search for Node.js via Java ofrece una funcionalidad de búsqueda poderosa y flexible para documentos. Integra la búsqueda de texto en aplicaciones Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) es una biblioteca robusta de búsqueda e indexación que permite la recuperación rápida de texto en documentos. Soporta más de 70 formatos de archivos, incluyendo PDFs, Word, Excel y PowerPoint, asegurando búsquedas precisas y eficientes.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo realizar una búsqueda en documentos DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) hace que buscar texto en documentos DOCX sea simple y eficiente para aplicaciones Node.js via Java.
      
      1. Crea un directorio para almacenar el índice de búsqueda.
      2. Elige la carpeta que contiene los documentos.
      3. Establece las opciones de búsqueda para incluir solo archivos DOCX.
      4. Ejecuta la búsqueda y recupera los resultados.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Define un directorio para almacenar el índice de búsqueda
        const index = new searchLib.Index("c:/MyIndex");

        // Especifica la carpeta que contiene documentos buscables
        index.add("c:/MyDocuments");

        // Restringe la búsqueda a formatos de archivo específicos
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".docx");

        // Recupera y procesa los resultados de búsqueda
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades avanzadas de búsqueda"
  description: "GroupDocs.Search for Node.js via Java mejora la eficiencia de búsqueda de documentos al indexar más de 70 formatos de archivos. Optimiza la recuperación de contenido con técnicas de búsqueda avanzadas."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto integral"
      content: "Extrae y localiza texto en formatos de documentos populares, como PDFs, archivos de Word, hojas de cálculo y presentaciones. Soporta búsqueda difusa, homófonos y consultas con comodines."

    # feature loop
    - title: "Indexación optimizada para rendimiento"
      content: "Acelera las búsquedas creando índices reutilizables. Mejora la velocidad y eficiencia al trabajar con grandes colecciones de documentos."

    # feature loop
    - title: "Soporte multilingüe"
      content: "Busca en documentos en más de 80 idiomas. Reconoce configuraciones de teclado y variaciones de palabras para mayor precisión."

    # feature loop
    - title: "Opciones de búsqueda personalizables"
      content: "Ajusta los resultados de búsqueda con filtros, expresiones regulares, sensibilidad a mayúsculas y minúsculas, y otras configuraciones flexibles."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrar documentos buscables"
      content: |
        Aprende a refinar las búsquedas de documentos usando filtros.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Configura un índice para excluir formatos de archivo no deseados
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Especifica el directorio que contiene los documentos
          index.add("c:/MyDocuments");

          // Procesa la salida de búsqueda para uso posterior
          const result = index.Search("Lorem", options);
          
          // Procesa la salida de búsqueda para uso posterior
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Copiar"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "¿Listo para comenzar?"
  description: "Prueba las características de GroupDocs.Search de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Funcionalidades clave"
    exclude: "filters"
    description: "Realiza búsquedas de texto rápidas y precisas en documentos."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar en diversos formatos de documentos"
    exclude: "DOCX"
    description: "GroupDocs.Search soporta más de 70 tipos de archivos, permitiendo una búsqueda eficiente de texto en diversos documentos de oficina y empresariales."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---