---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/java/case-sensitive/pptm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "API de Java para realizar búsquedas de texto con distinción entre mayúsculas y minúsculas en documentos PPTM"
head_description: "GroupDocs.Search Java API permite a los programadores realizar búsquedas de texto que distinguen entre mayúsculas y minúsculas y descubrir la estructura exacta de las palabras en documentos PPTM a través de Java."

############################# Header ############################
title: "Realizar búsquedas con distinción entre mayúsculas y minúsculas a través de PPTM documentos en aplicaciones Java"
description: "GroupDocs.Search Java API permite a los desarrolladores de software aplicar búsquedas de texto con distinción entre mayúsculas y minúsculas a través de varios tipos de documentos como PDF, HTML, DOCX, PPTX, XLSX y más en aplicaciones Java."

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo realizar búsquedas con distinción entre mayúsculas y minúsculas en aplicaciones Java?"
    content: |
      La sensibilidad a mayúsculas y minúsculas es una técnica de búsqueda muy útil que describe la capacidad de un programa para diferenciar entre letras mayúsculas (mayúsculas) y minúsculas (pequeñas) en búsquedas web, de bases de datos o de documentos. Es muy importante recordar que, de forma predeterminada, el motor de búsqueda no distingue entre mayúsculas y minúsculas, lo que significa que la búsqueda de la palabra Computadora dará tanto fragmentos con un nombre clave como texto con las palabras Computadora y computadora. Supongamos que necesitamos reducir los resultados de la búsqueda a los que tienen la letra mayúscula 'Computadora', lo que significa que necesitamos una búsqueda que distinga entre mayúsculas y minúsculas. GroupDocs.Search para Java es una API eficaz de búsqueda e indexación de documentos que permite a los desarrolladores de software desarrollar aplicaciones que pueden realizar la búsqueda e indexación de texto para algunos de los tipos de documentos más populares como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel, Presentaciones de PowerPoint, Outlook MSG, PST y muchos más. Además, puede identificar consultas de búsqueda escritas en un idioma que no coincide con la distribución de su teclado.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Búsqueda sensible a mayúsculas y minúsculas en PPTM Documentos a través de Java"
      content_left: |
       GroupDocs.Search Java API ha incorporado soporte completo para funciones de búsqueda básicas y avanzadas que permiten a los desarrolladores de software realizar búsquedas que distinguen entre mayúsculas y minúsculas dentro de sus aplicaciones Java con solo un par de líneas de código.
       
        El siguiente ejemplo de código Java muestra cómo lograr una búsqueda que distingue entre mayúsculas y minúsculas con una consulta en el texto en archivos PPTM con solo un par de líneas de código.

      title_right: "Realice una búsqueda que distingue entre mayúsculas y minúsculas en PPTM Files"
      content_right: |
         * Identifique la ruta a la carpeta de índice, así como a la carpeta de documentos.
         * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
         * Indexación de documentos de la carpeta especificada llamando a la instancia de la clase [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
         * Iniciar una nueva instancia de la clase [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
         * Habilitación de la opción de búsqueda entre mayúsculas y minúsculas llamando al método [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
         * Definir consulta de búsqueda y comenzar a buscar
         
        
      gisthash: "f5cba2431bcb82d746d2a002b1947d21"
      gistfile: "case-sensitive_in_text_queries_java.java"

    - title_left: "Realice búsquedas sensibles a mayúsculas y minúsculas en forma de objeto a través de Java"
      content_left: |
        GroupDocs.Search Java brinda a los desarrolladores de software el poder de incluir funciones de búsqueda para varios formatos de documentos dentro de sus propias aplicaciones. El siguiente ejemplo de código Java demuestra cómo realizar búsquedas que distinguen entre mayúsculas y minúsculas con una consulta en forma de objeto a través de documentos PPTM. 

      title_right: "Aplicar búsqueda con distinción entre mayúsculas y minúsculas en PPTM Documentos"
      content_right: |
        * Identifique la ruta a la carpeta de índice, así como a la carpeta de documentos.
        * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String))
        * Indexación de documentos de la carpeta especificada llamando a la instancia de la clase [Add](https://apireference.groupdocs.com/search/net/groupdocs.search.index/add/methods/1)
        * Iniciar una nueva instancia de la clase [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
        * Habilitación de la opción de búsqueda entre mayúsculas y minúsculas llamando al método [UseCaseSensitiveSearch](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/usecasesensitivesearch)
        * Crear una consulta de búsqueda en un objeto llamando al método [createWordQuery](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchQuery#createWordQuery(java.lang.String))
        * Definir consulta de búsqueda y comenzar a buscar
     
      gisthash: "9e2aee884e199033f89c2c21cde108b7"
      gistfile: "case-sensitive_search_in_object_form_java.java"

    - title_left: "Requisitos del sistema"
      content_left: |
        GroupDocs.Search for Java es compatible con todas las principales plataformas y sistemas operativos. Para obtener una guía completa de requisitos del sistema, visite [requisitos del sistema](https://docs.groupdocs.com/search/java/system-requirements/) antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema:
          * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
          * Compatibilidad con versiones de Java: J2SE 7.0 (1.7), J2SE 8.0 (1.8) o superior
          * Obtenga la última versión de GroupDocs.Search para las API de Java de GroupDocs [Repository](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/)
        
      title_right: "Por qué usar GroupDocs.Search"
      content_right: |
        * Creación de índices de búsqueda tanto en memoria como en disco.
        * Capacidad de indexación de un archivo, secuencia o estructura.
        * Soporte de indexación de documentos protegidos por contraseña.
        * Soporte para la fusión de varios índices.
        * Documento de filtro durante la indexación de búsqueda.
        * Compatibilidad con el corrector ortográfico durante la búsqueda.
        * Los caracteres combinados son totalmente compatibles
        * La combinación de diferentes tipos de búsqueda en una consulta de búsqueda.
        * Compatibilidad con búsquedas de palabras simples y expresiones regulares
        * Totalmente compatible con el reemplazo de alias en las consultas de búsqueda.

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---