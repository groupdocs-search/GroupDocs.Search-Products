
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: es
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Búsqueda boolean en TXT con Java"
head_description: "Con GroupDocs.Search for Java, los desarrolladores pueden realizar búsquedas de documentos utilizando operadores booleanos como AND, OR y NOT."

############################# Header ############################
title: "Búsqueda de texto booleano" 
description: "Utiliza GroupDocs.Search for Java para crear consultas de búsqueda booleanas avanzadas (AND, OR, NOT) en tus proyectos de Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar Gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Acerca de GroupDocs.Search"
    link: "/search/java/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) es una biblioteca versátil diseñada para la búsqueda de texto y la indexación de datos en documentos. Soporta más de 70 tipos de archivos, incluidos PDF, Word, Excel, presentaciones de PowerPoint, imágenes y archivos ZIP, lo que permite realizar búsquedas eficientes a través de grandes colecciones de datos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo realizar búsquedas booleanas en documentos TXT"
    content: |
      [GroupDocs.Search](/search/java/) permite realizar búsquedas de texto dentro de documentos TXT. Con soporte para condiciones booleanas, puedes mejorar la precisión de las búsquedas en aplicaciones de Java.
      
      1. Especifica la carpeta para almacenar el índice de búsqueda.
      2. Selecciona la carpeta que contiene documentos TXT.
      3. Ejecuta la consulta de búsqueda y recupera los resultados.
      4. Procesa los resultados obtenidos.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado de búsqueda"
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
        copy_tip: "haz clic para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Más ejemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentación"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Establece la ruta para la carpeta del índice
        Index index = new Index("c:/MyIndex");

        // Proporciona la ruta de la carpeta que contiene los documentos para la búsqueda
        index.add("c:/MyDocuments");

        // Ejecuta una búsqueda con una consulta compleja
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Herramientas poderosas para la búsqueda e indexación de documentos"
  description: "GroupDocs.Search for Java simplifica las búsquedas de texto y la indexación de datos para más de 70 formatos. Sus herramientas avanzadas te permiten encontrar y gestionar contenido sin esfuerzo."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto integral"
      content: "Busca en múltiples formatos como PDFs, documentos de Word, presentaciones, hojas de cálculo y más. Utiliza opciones como coincidencia exacta, búsqueda difusa y consultas con caracteres comodín para refinar los resultados."

    # feature loop
    - title: "Indexación de datos eficiente"
      content: "Crea y mantén índices para búsquedas de documentos más rápidas. Esta función organiza los datos de manera eficiente, facilitando el manejo de grandes colecciones de documentos."

    # feature loop
    - title: "Soporte multilingüe"
      content: "Busca en documentos escritos en más de 80 idiomas. Mejora la precisión aprovechando las formas morfológicas de las palabras y diferentes distribuciones de teclado."

    # feature loop
    - title: "Personalización flexible de la búsqueda"
      content: "Ajusta la configuración de búsqueda con características como sensibilidad a mayúsculas, filtros de rango de fechas y exclusiones para refinar tus resultados."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Uso de consultas complejas de búsqueda booleanas"
      content: |
        Este ejemplo demuestra cómo realizar búsquedas booleanas en archivos TXT.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Establece la carpeta para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Proporciona la ruta a los documentos a buscar
          index.add("c:/MyDocuments");

          // Construye la consulta utilizando lógica boolean
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Recupera los resultados de búsqueda
          SearchResult result = index.search(booleanQuery);
          
          // Procesa los resultados recuperados
          System.out.println("Documents: " + result.getDocumentCount());
          System.out.println("Occurrences: " + result.getDocumentCount());
          ```
        platform: "java"
        copy_title: "Copiar"
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
          copy_tip: "haz clic para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Descargar resultado"
            icon: "download"
            link: "/examples/search/formats/searchboolean.txt"
        links:
          #  loop
          - title: "Más ejemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentación"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "¿Listo para empezar?"
  description: "Prueba las funciones de GroupDocs.Search gratis o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licencias"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Características clave de un vistazo"
    exclude: "boolean"
    description: "Desbloquea poderosas y eficientes capacidades de búsqueda."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar formatos de documentos populares"
    exclude: "TXT"
    description: "GroupDocs.Search soporta más de 70 formatos de archivo, permitiéndote personalizar las reglas de búsqueda y utilizar la indexación para optimizar el rendimiento."
    items: 
        # format loop 1
        - name: "Búsqueda booleana en DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Búsqueda booleana en PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Búsqueda booleana en PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Búsqueda booleana en TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Búsqueda booleana en XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---