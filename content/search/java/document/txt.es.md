
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:34
draft: false
lang: es
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Encuentra texto en documentos TXT con GroupDocs.Search para Java"
head_description: "GroupDocs.Search for Java ayuda a los desarrolladores de Java a buscar rápidamente texto en varios formatos de documentos."

############################# Header ############################
title: "Búsqueda inteligente de texto en documentos" 
description: "Con GroupDocs.Search for Java, puedes buscar y extraer texto sin dificultades de múltiples tipos de documentos en tus aplicaciones de Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtén una prueba gratuita"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué hace GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Aprende más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) es una robusta biblioteca de búsqueda e indexación de documentos que soporta más de 70 formatos de archivo, incluidos PDF, Word, PowerPoint, Excel, imágenes y archivos ZIP. Permite capacidades de búsqueda rápidas, precisas y escalables para grandes colecciones de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Realizar búsquedas textuales en archivos TXT"
    content: |
      [GroupDocs.Search](/search/java/) facilita la búsqueda en archivos TXT utilizando lógica sofisticada e indexación, mejorando la precisión de búsqueda en aplicaciones Java.
      
      1. Configura un directorio para almacenar el índice de búsqueda.
      2. Selecciona una carpeta que contenga archivos TXT.
      3. Define opciones adicionales de búsqueda.
      4. Ejecuta la búsqueda y analiza los resultados.
   
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
        // Establecer el directorio para almacenar el índice de búsqueda
        Index index = new Index("c:/MyIndex");

        // Especificar la carpeta que contiene documentos buscables
        index.add("c:/MyDocuments");

        // Activar la búsqueda de homófonos para coincidir palabras con pronunciación similar
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Ejecutar una consulta de búsqueda avanzada
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades mejoradas de búsqueda e indexación"
  description: "GroupDocs.Search for Java simplifica la búsqueda de texto e indexación en más de 70 formatos de documentos, proporcionando herramientas eficientes para administrar y recuperar información rápidamente."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Características principales de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto exhaustiva"
      content: "Encuentra texto en múltiples formatos de documentos como PDFs, documentos de Word, presentaciones de PowerPoint y hojas de cálculo. Usa coincidencias exactas, búsqueda difusa y operadores comodín para resultados de búsqueda refinados."

    # feature loop
    - title: "Indexación optimizada para grandes datos"
      content: "Crea índices estructurados para acelerar las búsquedas, facilitando la navegación a través de extensos repositorios de documentos de manera eficiente."

    # feature loop
    - title: "Soporte para múltiples idiomas"
      content: "Realiza búsquedas en más de 80 idiomas con soporte integrado para diferentes distribuciones de teclado y variaciones de morfología de palabras, mejorando así la precisión."

    # feature loop
    - title: "Configuraciones de búsqueda flexibles"
      content: "Personaliza las búsquedas con opciones como sensibilidad a mayúsculas, filtrado basado en fechas y la capacidad de excluir palabras específicas para resultados precisos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementación de consultas de búsqueda avanzadas"
      content: |
        Este ejemplo ilustra cómo utilizar consultas de búsqueda para buscar dentro de documentos TXT de manera eficiente.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Definir el directorio para la indexación de búsqueda
          Index index = new Index("c:/MyIndex");
              
          // Proporcionar la ruta del archivo para los documentos
          index.add("c:/MyDocuments");

          // Ingresar la contraseña para documentos encriptados
          index.getDictionaries().getDocumentPasswords().add("protected.txt", "123456");

          // Activar la búsqueda difusa para detectar palabras similares
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Obtener los resultados de la búsqueda
          SearchResult result = index.Search("Loarem", options);
          
          // Procesar y analizar los resultados de la búsqueda
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "Descripción general de características clave"
    exclude: "document"
    description: "Descubre funcionalidades de búsqueda de texto de alto rendimiento diseñadas para eficiencia y precisión."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Encuentra información en documentos TXT con GroupDocs.Search"
    exclude: "TXT"
    description: "GroupDocs.Search soporta más de 70 formatos, incluidos archivos de oficina, habilitando búsquedas rápidas con características avanzadas de indexación."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---