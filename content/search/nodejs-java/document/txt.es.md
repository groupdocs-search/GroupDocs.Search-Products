
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: es
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Encuentra texto en TXT con GroupDocs.Search en Node.js"
head_description: "Utiliza GroupDocs.Search for Node.js via Java con JavaScript para buscar texto de manera eficiente en varios formatos de documentos."

############################# Header ############################
title: "Solución inteligente de búsqueda de documentos" 
description: "Localiza texto en diferentes formatos de documentos utilizando GroupDocs.Search for Node.js via Java. Crea consultas de búsqueda avanzadas dentro de tus aplicaciones Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Prueba Gratis"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introducción a GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) es una biblioteca de alto rendimiento para la búsqueda de texto completo e indexación de documentos. Soporta más de 70 tipos de archivos, incluyendo PDF, Word, PowerPoint, Excel, imágenes y archivos ZIP, asegurando resultados rápidos y precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Realiza búsqueda en archivos TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) te permite ejecutar búsquedas en archivos TXT, refinando resultados en aplicaciones Node.js via Java.
      
      1. Define una carpeta de almacenamiento para el índice de búsqueda.
      2. Selecciona una carpeta con archivos TXT.
      3. Establece parámetros de búsqueda adicionales.
      4. Ejecuta la búsqueda y analiza los resultados.
   
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

        // Especifica el directorio para el almacenamiento del índice de búsqueda
        const index = new searchLib.Index("c:/MyIndex");

        // Elige la carpeta que contiene los documentos a buscar
        index.add("c:/MyDocuments");

        // Habilita la búsqueda de homófonos para palabras que suenan similares
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Ejecuta una consulta de búsqueda compleja
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades avanzadas de búsqueda e indexación"
  description: "GroupDocs.Search for Node.js via Java proporciona potentes herramientas de búsqueda de texto e indexación a través de más de 70 formatos de documentos, facilitando la búsqueda y organización de información."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Beneficios clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto integral"
      content: "Localiza texto en múltiples tipos de documentos, incluyendo PDFs, documentos de Word, presentaciones de PowerPoint y hojas de cálculo. Utiliza coincidencias exactas, búsqueda difusa y comodines para resultados refinados."

    # feature loop
    - title: "Indexación eficiente para grandes volúmenes de datos"
      content: "Acelera las búsquedas creando índices estructurados, facilitando la recuperación de información de colecciones de documentos grandes."

    # feature loop
    - title: "Soporta más de 80 idiomas"
      content: "Realiza búsquedas en documentos en diferentes idiomas, con reconocimiento automático de diversas formas de palabras y distribuciones de teclado."

    # feature loop
    - title: "Configuraciones de búsqueda personalizadas"
      content: "Ajusta opciones de búsqueda como sensibilidad a mayúsculas, filtros de fecha y exclusiones de palabras para obtener resultados precisos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Uso de la búsqueda para documentos TXT"
      content: |
        Este ejemplo muestra cómo utilizar consultas de búsqueda dentro de documentos TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Establecer el directorio para la indexación de búsqueda
          const index = new searchLib.Index("c:/MyIndex");
              
          // Proporcionar la ruta del archivo para el almacenamiento del documento
          index.add("c:/MyDocuments");

          // Introducir la contraseña para archivos protegidos
          index.getDictionaries().getDocumentPasswords().add("protected.txt", '123456');

          // Habilitar búsqueda difusa para detección de palabras similares
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Extraer resultados de búsqueda
          const result = index.search("Loarem", options);
          
          // Procesar y revisar los resultados
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "Explora características clave"
    exclude: "document"
    description: "Descubre características de búsqueda de alta velocidad diseñadas para mejorar la eficiencia y precisión."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Busca en una variedad de documentos"
    exclude: "TXT"
    description: "GroupDocs.Search funciona con más de 70 formatos de archivo, incluyendo documentos de oficina, asegurando búsquedas rápidas y precisas con soporte de indexación."
    items: 
        # format loop 1
        - name: "Buscar en documento DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Buscar en documento PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Buscar en documento PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Buscar en documento TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Buscar en documento XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---