
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: es
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Realiza búsquedas sensibles a mayúsculas en PPTX con Node.js"
head_description: "La API GroupDocs.Search for Node.js via Java permite a los desarrolladores JavaScript ejecutar búsquedas sensibles a mayúsculas en diferentes tipos de documentos."

############################# Header ############################
title: "Búsqueda Sensible a Mayúsculas" 
description: "GroupDocs.Search for Node.js via Java te permite implementar funcionalidad avanzada de búsqueda sensible a mayúsculas en tus aplicaciones Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) es una potente biblioteca para buscar e indexar texto en documentos. Soporta más de 70 formatos, incluyendo PDF, Word, Excel, PowerPoint, imágenes y archivos ZIP, lo que permite manejar eficientemente grandes cantidades de datos.

############################# Steps ############################
steps:
    enable: true
    title: "Pasos para Realizar Búsquedas Sensibles a Mayúsculas en Archivos PPTX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilita la realización de búsquedas sensibles a mayúsculas en archivos PPTX, mejorando tus flujos de trabajo en Node.js via Java.
      
      1. Configura una carpeta para almacenar el índice de búsqueda.
      2. Selecciona la carpeta que contiene archivos PPTX.
      3. Ejecuta la búsqueda y obtén los resultados.
      4. Procesa y utiliza los resultados.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado de búsqueda"
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

        // Especifica la ruta para la carpeta del índice
        const index = new searchLib.Index("c:/MyIndex");

        // Establece la carpeta que contiene los documentos a buscar
        index.add("c:/MyDocuments");

        // Habilita la búsqueda sensible a mayúsculas en la configuración
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Ejecuta la búsqueda
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Características Clave para Búsqueda e Indexación de Documentos"
  description: "Con GroupDocs.Search for Node.js via Java, puedes buscar e indexar texto en más de 70 formatos de archivo. Accede y organiza información de manera efectiva utilizando herramientas de búsqueda avanzadas."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Características Principales de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de Texto Integral"
      content: "Encuentra texto en varios tipos de documentos como PDFs, archivos de Word, hojas de cálculo y presentaciones. Utiliza opciones como coincidencias exactas, búsquedas difusas y comodines para obtener resultados precisos."

    # feature loop
    - title: "Indexación de Datos Eficiente"
      content: "Crea y gestiona índices para acelerar las búsquedas. La indexación te ayuda a organizar y localizar rápidamente datos en grandes colecciones de documentos."

    # feature loop
    - title: "Soporte para Múltiples Idiomas"
      content: "Busca documentos en más de 80 idiomas con soporte para diversas configuraciones de teclado y variaciones de palabras, garantizando resultados de búsqueda precisos."

    # feature loop
    - title: "Configuraciones de Búsqueda Personalizables"
      content: "Ajusta la configuración de búsqueda, incluyendo sensibilidad a mayúsculas, filtros de fecha y exclusión de términos o datos específicos durante la indexación."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ejemplo: Implementación de Búsqueda Sensible a Mayúsculas"
      content: |
        Este ejemplo demuestra cómo realizar búsquedas sensibles a mayúsculas para documentos PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Define la carpeta para el índice de búsqueda
          const index = new searchLib.Index("c:/MyIndex");
              
          // Proporciona la ruta a la carpeta de documentos
          index.add("c:/MyDocuments");

          // Configura una consulta de búsqueda
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Activa la configuración de búsqueda sensible a mayúsculas
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Busca el texto en los documentos
          const result = index.search(wordQuery, options);
          
          // Procesa y maneja los resultados
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
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Search gratis o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Funcionalidades Clave"
    exclude: "case-sensitive"
    description: "Explora características avanzadas para una búsqueda de documentos rápida y precisa."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formatos de Documento Compatibles"
    exclude: "PPTX"
    description: "GroupDocs.Search es compatible con más de 70 formatos de documento. Personaliza tus opciones de búsqueda y ahorra tiempo con la indexación."
    items: 
        # format loop 1
        - name: "Búsqueda sensible a mayúsculas y minúsculas en DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas en PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Búsqueda sensible a mayúsculas y minúsculas en PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Búsqueda sensible a mayúsculas y minúsculas en TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Búsqueda sensible a mayúsculas y minúsculas en XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---