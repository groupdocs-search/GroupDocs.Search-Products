---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/net/phrase/chm/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MD EPUB  FB2 

############################# Head ############################
head_title: "¿Cómo agregar la búsqueda de frases en CHM Documentos en aplicaciones .NET?"
head_description: "GroupDocs.Search .NET API permite a las profesiones de software agregar búsqueda de frases y encontrar la frase exacta o la secuencia de palabras proporcionada en CHM documentos a través de .NET API."

############################# Header ############################
title: "¿Agregar búsqueda de frases o oraciones exactas en CHM Documentos dentro de aplicaciones .NET?"
description: "GroupDocs.Search .NET API permite a los programadores encontrar la secuencia de palabras proporcionada en CHM documentos a través de la búsqueda de frases o la búsqueda de oraciones exactas dentro de las aplicaciones .NET. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Cómo usar la búsqueda de frases o oraciones exactas en las aplicaciones .NET?"
    content: |
       La búsqueda de frases o frases exactas es un tipo de búsqueda que permite a los usuarios buscar documentos, sitios web o bases de datos que tengan una frase o frase exacta que contenga un orden específico y una combinación de palabras definidas por los consumidores. Es un término muy común en la terminología de los motores de búsqueda y permite a los usuarios buscar documentos para una secuencia específica de palabras en el texto de los documentos indexados. GroupDocs.Search for .NET es una API de búsqueda de texto y documentos de alto rendimiento muy útil que proporcionó una funcionalidad completa para desarrollar aplicaciones para la búsqueda e indexación de texto que admite algunos de los tipos de documentos más comunes, como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, Hojas de cálculo de Excel, presentaciones de PowerPoint, MSG de Outlook, PST, etc. Ha incluido compatibilidad con varias funciones relacionadas con la búsqueda de frases, como la consulta de búsqueda en forma de texto y objeto, el uso de comodines en la búsqueda de frases, etc.
############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Cómo realizar una búsqueda de frases en documentos CHM a través de .NET"
      content_left: |
       GroupDocs.Search .NET API permite a los desarrolladores de software agregar funcionalidades de búsqueda de frases dentro de su propia aplicación C# .NET. El siguiente ejemplo de código .NET demuestra cómo realizar la búsqueda de frases en texto y objetos con solo un par de líneas de código.

      title_right: "Búsqueda exacta de frases en CHM Documentos"
      content_right: |
         * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
         * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Busque la consulta de frase 'texto de frase' en forma de texto
         * Busque la frase 'texto de frase' en forma de objeto
         * Crear word1, word2 y crear la subconsulta 3 llamando al método [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
         * Combinar subconsultas para crear una nueva consulta de búsqueda llamando al método [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
         * Comience a buscar y muestre los resultados de búsqueda
         
        
      gisthash: "a5696884acf504acc319ba97465248cd"
      gistfile: "phrase_search_in_text_queries_dotnet.cs"

    - title_left: "Búsqueda de frases con comodines en CHM Documentos a través de .NET"
      content_left: |
        GroupDocs.Search for .NET permite a los programadores de software agregar funcionalidades de búsqueda de frases utilizando comodines dentro de la aplicación C# .NET. Los siguientes ejemplos de código .NET muestran cómo aplicar la búsqueda de frases con comodines en documentos CHM dentro de aplicaciones C#.

      title_right: "Aplicar la búsqueda de frases con comodines en el archivo CHM"
      content_right: |
        * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
        * Creación de índices en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Busque la consulta de frase 'texto de frase' en forma de texto
        * Busque la frase 'texto de frase' en forma de objeto
        * Creando word1 y Creando subconsulta 3 llamando al método [CreateWordQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordquery)
        * Crear wildcard2 llamando al método [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1)
        * Combinar subconsultas para crear una nueva consulta de búsqueda llamando al método [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
        * Comience a buscar y muestre los resultados de búsqueda
     
      gisthash: "3ff2bf9f8ba902d8d7ebead67a934654"
      gistfile: "use_wildcards_in_phrase_search_dotnet.cs"
      
    - title_left: "Combine la búsqueda de frases con otros tipos de búsquedas a través de .NET"
      content_left: |
        GroupDocs.Search .NET brinda a los programadores de software el poder de combinar la búsqueda de frases con otros tipos de búsquedas dentro de la aplicación .NET. Los siguientes ejemplos de código .NET muestran cómo aplicar comodines que representan palabras y caracteres en palabras.

      title_right: ".NET API para combinar la búsqueda de frases con otras búsquedas"
      content_right: |
        * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
        * Creación de índices en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Buscar la frase en forma de texto
        * Buscar la frase en forma de objeto
        * Definir patrón de palabra y añadir cadena.
        * Creando wordPattern1 y Creando word3 llamando al método [CreateWordPatternQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createwordpatternquery)
        * Crear wildcard2 llamando al método [CreateWildcardQuery](https://apireference.groupdocs.com/search/net/groupdocs.search.searchquery/createwildcardquery/methods/1)
        * Combinar subconsultas para crear una nueva consulta de búsqueda llamando al método [CreatePhraseSearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createphrasesearchquery)
        * Comience a buscar y muestre los resultados de búsqueda
     
      gisthash: "db5c32ed21237f3e1cd7cdbde0778c29"
      gistfile: "combine_phrase_search_with_others_dotnet.cs"

    - title_left: "Requisitos del sistema"
      content_left: |
       GroupDocs.Search for .NET es compatible con todas las principales plataformas y sistemas operativos. Para obtener una guía completa de requisitos del sistema, visite [requisitos del sistema](https://docs.groupdocs.com/search/net/system-requirements/) antes de ejecutar el código a continuación, asegúrese de tener los siguientes requisitos previos instalados en su sistema:
         * Sistemas Operativos: Microsoft Windows, Linux, Mac OS
         * Entorno de desarrollo: Visual Studio, Xamarin, MonoDevelop, etc.
         * Marcos: .NET Framework, .NET Standard, .NET Core, Mono
         * Obtenga la última versión de GroupDocs.Search para las API de .NET de [NuGet](https://www.nuget.org/packages/GroupDocs.search/)
        
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