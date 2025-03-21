
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: es
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Buscar en documentos PDF utilizando Java"
head_description: "GroupDocs.Search for Java agrega una poderosa búsqueda de texto a las aplicaciones Java, soportando varios formatos de documentos empresariales."

############################# Header ############################
title: "Encuentra texto en documentos empresariales" 
description: "GroupDocs.Search for Java te permite buscar texto en documentos utilizando consultas flexibles y precisas. Integra la funcionalidad de búsqueda en aplicaciones Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Descargar gratis"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "¿Qué es GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Saber más"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) es una biblioteca robusta para búsqueda rápida de texto e indexación de documentos. Soporta más de 70 formatos de archivo, incluyendo estándares de la industria como PDF, Word, Excel y PowerPoint. Mejora tus aplicaciones con capacidades de búsqueda precisas y de alta velocidad.

############################# Steps ############################
steps:
    enable: true
    title: "Cómo buscar en documentos PDF"
    content: |
      [GroupDocs.Search](/search/java/) permite búsquedas de texto rápidas y eficientes en documentos PDF, perfecto para aplicaciones Java.
      
      1. Especifica una carpeta para almacenar el índice de búsqueda.
      2. Selecciona la carpeta que contiene tus documentos.
      3. Configura las opciones de búsqueda para limitar los resultados a documentos PDF.
      4. Ejecuta la búsqueda y obtén los resultados.
   
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
        // Directorio para almacenar el índice de búsqueda reutilizable
        Index index = new Index("c:/MyIndex");

        // Carpeta que contiene los documentos
        index.add("c:/MyDocuments");

        // Filtra búsquedas por formato de documento
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.createFileExtension(".pdf");

        // Recupera los resultados de búsqueda
        SearchResult result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades de búsqueda mejoradas"
  description: "GroupDocs.Search for Java ofrece búsqueda avanzada de texto en más de 70 formatos de archivos. La indexación acelera las búsquedas y mejora la eficiencia en la gestión de documentos."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Características clave de GroupDocs.Search"
  features:
    # feature loop
    - title: "Búsqueda de texto poderosa"
      content: "Encuentra texto en formatos de documentos populares como PDFs, archivos de Word, presentaciones y hojas de cálculo. Soporta múltiples métodos de búsqueda, incluyendo búsqueda difusa, homófonos y comodines."

    # feature loop
    - title: "Indexación optimizada para mejor rendimiento"
      content: "Crea y reutiliza índices de búsqueda para mejorar la velocidad y eficiencia de búsqueda, especialmente en colecciones de documentos grandes."

    # feature loop
    - title: "Soporte de búsqueda multilingüe"
      content: "Busca dentro de documentos escritos en más de 80 idiomas. Detecta diferentes distribuciones de teclado y variaciones de palabras para mayor precisión."

    # feature loop
    - title: "Opciones de búsqueda personalizables"
      content: "Reduce los resultados de búsqueda con filtros, expresiones regulares y otras configuraciones de búsqueda avanzadas."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrar documentos antes de buscar"
      content: |
        Aprende a refinar búsquedas utilizando filtros
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Configura un índice que excluya ciertos formatos de archivo
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new Index("c:/MyIndex", settings);
              
          // Especifica la ruta de almacenamiento de documentos
          index.add("c:/MyDocuments");

          // Recupera los resultados de búsqueda
          SearchResult result = index.search("Lorem", options);
          
          // Procesa y utiliza los resultados de búsqueda
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
            link: "/examples/search/formats/searchfilters.pdf"
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
    title: "Características clave"
    exclude: "filters"
    description: "Realiza búsquedas de texto precisas y eficientes."
    items: 
          
        # operation loop 1
        - name: "Búsqueda por condición"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "Encuentra información en documentos usando condiciones booleanas"

        # operation loop 2
        - name: "Búsqueda sensible a mayúsculas y minúsculas"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "Mejora la precisión de la búsqueda considerando la sensibilidad de mayúsculas"

        # operation loop 3
        - name: "Indexación de documentos"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "Indexa documentos una vez y reutiliza el índice para múltiples búsquedas"

        # operation loop 4
        - name: "Filtros de búsqueda"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "Utiliza filtros para reducir los datos procesados"

        # operation loop 5
        - name: "Frase exacta"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "Busca una oración o frase específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar en documentos empresariales"
    exclude: "PDF"
    description: "GroupDocs.Search soporta más de 70 formatos de archivo, facilitando la búsqueda a través de documentos de oficina ampliamente utilizados."
    items: 
        # format loop 1
        - name: "Filtros de búsqueda para DOCX"
          format: "DOCX"
          link: "/search/java/filters/docx/"
          description: "Documento de Microsoft Word Open XML"
          
        # format loop 2
        - name: "Filtros de búsqueda para PDF"
          format: "PDF"
          link: "/search/java/filters/pdf/"
          description: "Formato de Documento Portátil de Adobe"
          
        # format loop 3
        - name: "Filtros de búsqueda para PPTX"
          format: "PPTX"
          link: "/search/java/filters/pptx/"
          description: "Presentación Open XML de PowerPoint"

        # format loop 4
        - name: "Filtros de búsqueda para TXT"
          format: "TXT"
          link: "/search/java/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Filtros de búsqueda para XLSX"
          format: "XLSX"
          link: "/search/java/filters/xlsx/"
          description: "Hoja de Cálculo Open XML de Microsoft Excel"
  

---