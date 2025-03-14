
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:47
draft: false
lang: es
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Realiza Búsquedas Sensibles a Mayúsculas en DOCX con Java"
head_description: "La API GroupDocs.Search for Java ayuda a los desarrolladores de Java a realizar búsquedas sensibles a mayúsculas en múltiples tipos de documentos."

############################# Header ############################
title: "Búsqueda de Documentos Sensible a Mayúsculas" 
description: "GroupDocs.Search for Java te permite implementar una funcionalidad precisa de búsqueda sensible a mayúsculas en tus proyectos de Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obténlo Gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Conoce GroupDocs.Search"
    link: "/search/java/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) es una herramienta versátil para la búsqueda y el indexado de texto en diversos documentos. Soporta más de 70 formatos como PDFs, archivos de Word, presentaciones de PowerPoint, hojas de Excel, imágenes y archivos ZIP, lo que te permite manejar eficientemente conjuntos de datos extensos.

############################# Steps ############################
steps:
    enable: true
    title: "Guía para Búsqueda Sensible a Mayúsculas en Archivos DOCX"
    content: |
      Usando [GroupDocs.Search](/search/java/), puedes realizar búsquedas sensibles a mayúsculas en documentos DOCX, mejorando tus proyectos de Java.
      
      1. Establece la carpeta para almacenar el índice de búsqueda.
      2. Selecciona la carpeta que contiene archivos DOCX.
      3. Ejecuta la búsqueda sensible a mayúsculas y recoge los resultados.
      4. Procesa y utiliza los resultados de búsqueda.
   
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
        // Define la ubicación para el almacenamiento del índice
        Index index = new Index("c:/MyIndex");

        // Indica la carpeta que contiene los documentos a buscar
        index.add("c:/MyDocuments");

        // Activa el modo sensible a mayúsculas en la configuración de búsqueda
        SearchOptions options = new SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Ejecuta la búsqueda
        SearchResult result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Herramientas Mejoradas de Búsqueda e Indexado"
  description: "Con GroupDocs.Search for Java, puedes optimizar la búsqueda de documentos e indexado para más de 70 formatos, facilitando la localización y organización de información."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Características Destacadas de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de Texto Flexible"
      content: "Realiza búsquedas en documentos como PDFs, archivos de Word, hojas de cálculo y presentaciones. Utiliza herramientas como coincidencia exacta, búsqueda difusa y soporte para caracteres comodín para refinar tus resultados."

    # feature loop
    - title: "Gestión Eficiente de Índices"
      content: "Organiza e indexa grandes conjuntos de datos para mejorar la velocidad y el rendimiento de búsqueda al manejar colecciones de documentos grandes."

    # feature loop
    - title: "Soporte para Idiomas Globales"
      content: "Realiza búsquedas en más de 80 idiomas, adaptándose a diferentes disposiciones de teclado y variaciones lingüísticas para una mejor precisión."

    # feature loop
    - title: "Filtros de Búsqueda Personalizables"
      content: "Ajusta los criterios de búsqueda con opciones como sensibilidad a mayúsculas, filtrado por rangos de fechas y exclusión de palabras o datos no deseados durante el indexado."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Ejemplo: Consultas de Búsqueda Sensible a Mayúsculas"
      content: |
        Este ejemplo demuestra cómo implementar búsquedas sensibles a mayúsculas para documentos DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Define el directorio para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Especifica la ubicación de la carpeta de documentos
          index.add("c:/MyDocuments");

          // Configura una consulta de búsqueda
          SearchQuery wordQuery = SearchQuery.createWordQuery("Lorem");

          // Activa la sensibilidad a mayúsculas en las opciones de búsqueda
          SearchOptions options = new SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Realiza la búsqueda de documentos
          SearchResult result = index.search(wordQuery, options);
          
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
            link: "/examples/search/formats/searchcase-sensitive.docx"
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
    title: "Resumen de Características Clave"
    exclude: "case-sensitive"
    description: "Descubre las capacidades de búsqueda robustas y efectivas que ofrece GroupDocs.Search for Java."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formatos de Archivo Soportados para Búsqueda"
    exclude: "DOCX"
    description: "GroupDocs.Search trabaja con más de 70 formatos de documentos populares, ofreciendo configuraciones de búsqueda personalizables e indexado eficiente."
    items: 
        # format loop 1
        - name: "Búsqueda sensible a mayúsculas y minúsculas en DOCX"
          format: "DOCX"
          link: "/search/java/case-sensitive/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas en PDF"
          format: "PDF"
          link: "/search/java/case-sensitive/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Búsqueda sensible a mayúsculas y minúsculas en PPTX"
          format: "PPTX"
          link: "/search/java/case-sensitive/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Búsqueda sensible a mayúsculas y minúsculas en TXT"
          format: "TXT"
          link: "/search/java/case-sensitive/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Búsqueda sensible a mayúsculas y minúsculas en XLSX"
          format: "XLSX"
          link: "/search/java/case-sensitive/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---