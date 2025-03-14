
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:46
draft: false
lang: es
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Búsqueda booleana de PPTX a través de Node.js"
head_description: "Utiliza la API GroupDocs.Search for Node.js via Java para realizar búsquedas avanzadas en el contenido de documentos con operadores booleanos como AND, OR y NOT, diseñada para desarrolladores de JavaScript."

############################# Header ############################
title: "Realiza búsquedas con lógica booleana" 
description: "Con GroupDocs.Search for Node.js via Java, puedes crear consultas de búsqueda avanzadas utilizando operadores booleanos (AND, OR, NOT) sin problemas dentro de tu entorno Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Ahora"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) es una herramienta robusta para buscar e indexar texto dentro de documentos. Soporta más de 70 formatos como PDF, Word, Excel, PowerPoint, imágenes y archivos ZIP, lo que permite procesar grandes volúmenes de información de manera eficiente.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo buscar en documentos PPTX usando operadores booleanos"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) te permite buscar contenido en archivos PPTX de manera efectiva. Con lógica booleana, puedes refinar tus consultas de búsqueda en aplicaciones Node.js via Java para una mayor precisión.
      
      1. Configura la carpeta para almacenar el índice de búsqueda.
      2. Selecciona la carpeta que contiene los archivos PPTX para la búsqueda.
      3. Ejecuta la consulta de búsqueda y recupera los resultados.
      4. Procesa y analiza los resultados de búsqueda.
   
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

        // Establecer la ubicación de la carpeta del índice
        const index = new searchLib.Index("c:/MyIndex");

        // Especificar la carpeta que contiene los documentos para buscar
        index.add("c:/MyDocuments");

        // Ejecutar una consulta de búsqueda con lógica avanzada
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Herramientas poderosas para búsqueda e indexación de documentos"
  description: "GroupDocs.Search for Node.js via Java simplifica la búsqueda de texto y la indexación para más de 70 tipos de archivos, ayudándote a encontrar y gestionar información más rápido y con precisión."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto mejorada"
      content: "Encuentra texto rápidamente en varios formatos como PDFs, documentos de Word, presentaciones y hojas de cálculo. Utiliza características como coincidencias exactas, búsquedas con comodines y búsqueda difusa para obtener resultados precisos."

    # feature loop
    - title: "Indexación de datos eficiente"
      content: "Crea y gestiona índices para acelerar las búsquedas en grandes colecciones de documentos. La indexación asegura un acceso rápido y estructurado a tus datos."

    # feature loop
    - title: "Soporte multilingüe"
      content: "Realiza búsquedas en documentos escritos en más de 80 idiomas. El soporte morfológico y la compatibilidad con diferentes distribuciones de teclado mejoran los resultados de búsqueda en distintos idiomas."

    # feature loop
    - title: "Configuraciones de búsqueda flexibles"
      content: "Personaliza tu búsqueda habilitando la sensibilidad a mayúsculas, aplicando filtros de fecha o excluyendo palabras y datos específicos durante la indexación."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ejemplo de búsqueda booleana avanzada"
      content: |
        Este ejemplo demuestra cómo crear consultas basadas en Booleanas para buscar contenido en documentos PPTX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Definir la carpeta para el índice de búsqueda
          const index = new searchLib.Index("c:/MyIndex");
              
          // Proporcionar la ubicación de los documentos a buscar
          index.add("c:/MyDocuments");

          // Construir una consulta utilizando operadores booleanos
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Recuperar los resultados de búsqueda
          const result = index.search(booleanQuery);
          
          // Procesar y utilizar los resultados de búsqueda
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
            link: "/examples/search/formats/searchboolean.pptx"
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
    title: "Capacidades clave de GroupDocs.Search"
    exclude: "boolean"
    description: "Desbloquea funciones de búsqueda avanzadas, eficientes y personalizables."
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
    title: "Buscar formatos de documento populares"
    exclude: "PPTX"
    description: "GroupDocs.Search soporta más de 70 formatos de archivo, ofreciendo reglas de búsqueda flexibles e indexación eficiente para ahorrar tiempo y esfuerzo."
    items: 
        # format loop 1
        - name: "Búsqueda booleana en DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Búsqueda booleana en PDF"
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Búsqueda booleana en PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Búsqueda booleana en TXT"
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Búsqueda booleana en XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---