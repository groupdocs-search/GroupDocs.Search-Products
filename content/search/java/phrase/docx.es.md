
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:39
draft: false
lang: es
format: Docx
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buscar frases en DOCX usando Java"
head_description: "GroupDocs.Search for Java mejora las aplicaciones Java con capacidades avanzadas de búsqueda de frases en el contenido de los documentos."

############################# Header ############################
title: "Encuentra frases en documentos" 
description: "Localiza rápidamente frases específicas con GroupDocs.Search for Java. Incorpora funcionalidades de búsqueda potentes en tus aplicaciones Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Funciones de GroupDocs.Search"
    link: "/search/java/"
    link_title: "Aprende más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) es una biblioteca robusta para indexar y buscar texto dentro de documentos. Soporta más de 70 formatos de archivo, incluyendo PDFs, documentos de Word, hojas de cálculo de Excel, imágenes y archivos ZIP, asegurando resultados de búsqueda rápidos y precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo encontrar frases en documentos DOCX"
    content: |
      [GroupDocs.Search](/search/java/) simplifica la búsqueda de frases en documentos DOCX. Utiliza diversas opciones para refinar los resultados de búsqueda en aplicaciones Java.
      
      1. Crea un directorio para el índice de búsqueda.
      2. Especifica la carpeta con archivos DOCX.
      3. Ajusta los parámetros de búsqueda.
      4. Recupera y analiza los resultados de búsqueda.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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
        // Define la ruta del índice de búsqueda
        Index index = new Index("c:/MyIndex");

        // Especifica la carpeta que contiene documentos
        index.add("c:/MyDocuments");

        // Establece preferencias de búsqueda
        SearchQuery word1 = SearchQuery.createWordQuery("lorem");
        SearchQuery word2 = SearchQuery.createWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.createWordQuery("dolor");

        SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, word2, word3);
        
        // Ejecuta la consulta de búsqueda
        SearchResult result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Explora el motor de búsqueda de documentos de Java"
  description: "GroupDocs.Search for Java permite búsquedas de frases en más de 70 formatos de archivo. Encuentra y organiza datos utilizando características de búsqueda avanzadas."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Capacidades clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de frases"
      content: "Localiza frases exactas en documentos de negocio, tales como PDFs, archivos de Word, presentaciones y hojas de cálculo. Utiliza comodines y otras opciones cuando la frase exacta no se conoce."

    # feature loop
    - title: "Indexación de datos optimizada"
      content: "Acelera las búsquedas en documentos creando y reutilizando índices de búsqueda. La indexación organiza datos de manera eficiente para búsquedas más rápidas y precisas."

    # feature loop
    - title: "Compatibilidad multilingüe"
      content: "Busca documentos en más de 80 idiomas. Soporta diferentes configuraciones de teclado y análisis morfológico para mejorar la precisión de búsqueda."

    # feature loop
    - title: "Opciones de búsqueda avanzadas"
      content: "Personaliza las búsquedas con sensibilidad a mayúsculas, búsqueda difusa, coincidencia de homófonos, filtrado de documentos y otras características potentes."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Utilizando métodos de búsqueda avanzados"
      content: |
        Aprende cómo construir consultas para buscar en DOCX.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Define el directorio para el índice de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Establece la ruta a los documentos de destino
          index.add("c:/MyDocuments");

          // Crea una consulta de búsqueda para una frase específica
          SearchQuery word1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.createWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.createWordQuery("dolor");

          SearchQuery query = SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Obtén los resultados de la búsqueda
          SearchResult result = index.search(query);
          
          // Procesa y utiliza los resultados recuperados
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchphrase.docx"
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
  title: "¿Listo para comenzar?"
  description: "Prueba las características de GroupDocs.Search de forma gratuita o solicita una licencia"
  items:
    #  loop
    - title: "Descarga de Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licenciamiento"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Capacidades de búsqueda avanzadas"
    exclude: "phrase"
    description: "Utiliza funcionalidades de búsqueda de vanguardia para mejorar la precisión y el rendimiento."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar frases en documentos de negocio"
    exclude: "DOCX"
    description: "GroupDocs.Search permite búsquedas de frases en más de 70 formatos de documentos. Aprovecha opciones avanzadas e indexación para búsquedas eficientes."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/phrase/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/phrase/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/phrase/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/phrase/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/phrase/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---