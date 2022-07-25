---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "es/search/net/boolean/mhtml/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE XHTML  MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Agregue operadores de búsqueda booleanos (AND, OR, NOT) en consultas de búsqueda a través de .NET"
head_description: "GroupDocs.Search .NET API permite a los desarrolladores de software agregar búsquedas booleanas o desarrollar nuevas consultas utilizando operadores booleanos Y, O NO, dentro de sus aplicaciones .NET."

############################# Header ############################
title: "Desarrolle consultas de búsqueda complejas utilizando operadores booleanos AND, OR, NOT en aplicaciones .NET"
description: "GroupDocs.Search .NET API permite a los programadores de computadoras desarrollar consultas de búsqueda complejas utilizando operadores booleanos (Y, O, NO) dentro de sus aplicaciones .NET. "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "¿Qué es la búsqueda booleana y cómo usar los operadores booleanos?"
    content: |
       La búsqueda booleana es un procedimiento de búsqueda muy útil que permite a los usuarios combinar diferentes palabras clave con el operador para limitar, ampliar y definir los resultados de la búsqueda. El operador booleano, como AND, OR, NOT y NEAR, etc. ayuda a los usuarios a obtener una gama más amplia de resultados o a reducir la cantidad de resultados de búsqueda no relacionados mediante la definición de limitaciones. GroupDocs.Search for .NET es una potente API de búsqueda de documentos de alto rendimiento que permite a los desarrolladores de software desarrollar aplicaciones que pueden realizar búsquedas de texto e indexación en algunos de los formatos de archivo de documentos más comunes como PDF, HTML, correo electrónico de Outlook, Microsoft Office Word, hojas de cálculo de Excel , presentaciones de PowerPoint, Outlook MSG, PST y muchos más. El operador booleano AND se puede usar para mostrar los resultados de todas las palabras que ha ingresado, el operador OR brinda resultados para cualquiera de las palabras que ha ingresado, el operador NOT se puede usar para mostrar los resultados de búsqueda sin ocurrencias, etc. Una gran característica es que puede reconocer consultas de búsqueda escritas en un idioma que no coincide con la distribución de su teclado.

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Use el operador booleano AND en consultas de búsqueda a través de .NET"
      content_left: |
       GroupDocs.Search .NET API brinda soporte completo para agregar capacidades de búsqueda booleana dentro de su aplicación .NET. El siguiente ejemplo de código C# muestra cómo crear un operador booleano "AND" en consultas de texto y formulario de objeto dentro de sus propias aplicaciones .NET.

      title_right: " Buscar documentos MHTML a través del operador booleano AND "
      content_right: |
         * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
         * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
         * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Creando la subconsulta 1 y Creando la subconsulta 2 llamando a la clase [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
         * Combinar subconsultas en una consulta llamando al método [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
         * Comience a buscar y muestre los resultados de búsqueda
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "Cómo usar el operador booleano O a través de .NET"
      content_left: |
       GroupDocs.Search for .NET es una potente API que permite a los programadores de software buscar en muchos formatos de documentos populares. Los siguientes ejemplos de código de C# .NET muestran cómo usar el operador booleano "OR" en consultas de texto y formulario de objeto dentro de aplicaciones de C#. 

      title_right: "Use el operador booleano OR para buscar archivos MHTML"
      content_right: |
        * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
        * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Creando la subconsulta 1 y Creando la subconsulta 2 llamando a la clase [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Combinar subconsultas en una consulta llamando al método [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Comience a buscar y muestre los resultados de búsqueda
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "Cree consultas de búsqueda complejas utilizando operadores booleanos"
      content_left: |
        GroupDocs.Search .NET permite a los programadores de computadoras combinar diferentes operadores booleanos para crear consultas de búsqueda complejas dentro de sus propias aplicaciones .NET. Los siguientes ejemplos de código .NET muestran cómo complejar las capacidades de búsqueda de documentos sin instalar ningún software o herramienta externa.

      title_right: "Busque documentos MHTML a través de consultas de búsqueda complejas"
      content_right: |
        * Primero debe especificar la ruta a la carpeta de índice y la carpeta de documentos.
        * Crear un índice en la carpeta especificada llamando a la instancia de la clase [Índice](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)
        * Indexación de documentos de la carpeta especificada llamando al método [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Comience a buscar y muestre la consulta de texto de los resultados de búsqueda
        * Búsqueda con consulta de objeto
        * Crear WordQuery y relativityWordQuery llamando a la clase [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Combinar subconsultas en una consulta llamando al método [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)
        * Crear einsteinWordQuery y albertWordQuery llamando a la clase [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)
        * Combinar subconsultas en una consulta llamando al método [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Combinar subconsultas en una consulta llamando al método [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery)
        * Comience a buscar y muestre los resultados de búsqueda
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

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