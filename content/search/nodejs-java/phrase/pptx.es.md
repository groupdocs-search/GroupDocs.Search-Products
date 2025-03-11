
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:40
draft: false
lang: es
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Buscar frases en PPTX utilizando Node.js"
head_description: "GroupDocs.Search for Node.js via Java añade una potente funcionalidad de búsqueda de frases a las aplicaciones de JavaScript para una búsqueda eficiente de documentos."

############################# Header ############################
title: "Encuentra frases en documentos" 
description: "Localiza rápidamente frases específicas con GroupDocs.Search for Node.js via Java. Integra capacidades de búsqueda rápidas y precisas en tus aplicaciones de Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Características de GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Aprende más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) es una biblioteca de alto rendimiento para indexar y buscar texto en documentos. Soporta más de 70 formatos de archivo, incluyendo PDFs, documentos de Word, hojas de cálculo de Excel, imágenes y archivos ZIP, asegurando resultados de búsqueda precisos y rápidos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo encontrar frases en documentos PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilita la búsqueda de frases en documentos PPTX. Aplica diferentes opciones de búsqueda para refinar los resultados en aplicaciones de Node.js via Java.
      
      1. Configura una carpeta para el índice de búsqueda.
      2. Define la carpeta que contiene archivos PPTX.
      3. Configura los parámetros de búsqueda.
      4. Recupera y procesa los resultados de búsqueda.
   
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

        // Especifica el camino para almacenar el índice de búsqueda
        const index = new searchLib.Index("c:/MyIndex");

        // Configura la carpeta que contiene los documentos
        index.add("c:/MyDocuments");

        // Configura los parámetros de búsqueda
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Ejecuta la consulta de búsqueda
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Descubre el motor de búsqueda de documentos Node.js"
  description: "GroupDocs.Search for Node.js via Java permite búsquedas de frases en más de 70 formatos de archivo, facilitando la organización y búsqueda de datos con características de búsqueda avanzadas."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Principales capacidades de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de frases"
      content: "Encuentra frases exactas en documentos de negocios como PDFs, archivos de Word, presentaciones y hojas de cálculo. Utiliza comodines y opciones de búsqueda flexibles cuando la frase completa es desconocida."

    # feature loop
    - title: "Indexación de datos optimizada"
      content: "Aumenta el rendimiento de búsqueda creando índices reutilizables. La indexación estructurada acelera las búsquedas de documentos y mejora la precisión."

    # feature loop
    - title: "Compatibilidad multilenguaje"
      content: "Busca documentos en más de 80 idiomas con soporte para diferentes distribuciones de teclado y variaciones morfológicas, asegurando resultados precisos."

    # feature loop
    - title: "Opciones de búsqueda avanzadas"
      content: "Personaliza las búsquedas con sensibilidad a mayúsculas, coincidencia difusa, detección de homófonos, filtrado de documentos y otras potentes características."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Uso de técnicas de búsqueda avanzadas"
      content: |
        Aprende a construir consultas para buscar en PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Define el directorio del índice de búsqueda
          const index = new searchLib.Index("c:/MyIndex");
              
          // Establece el camino hacia los documentos objetivo
          index.add("c:/MyDocuments");

          // Crea una consulta para la frase deseada
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Recupera los resultados de búsqueda
          const result = index.search(query);
          
          // Procesa y utiliza los resultados
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
            link: "/examples/search/formats/searchphrase.pptx"
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
    title: "Capacidades de búsqueda avanzadas"
    exclude: "phrase"
    description: "Aprovecha las potentes características de búsqueda para obtener resultados más rápidos y precisos."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar frases en documentos de negocios"
    exclude: "PPTX"
    description: "GroupDocs.Search soporta búsquedas de frases en más de 70 formatos de documentos. Utiliza opciones avanzadas e indexación para agilizar el proceso de búsqueda."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---