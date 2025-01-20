---
############################# Static ############################
layout: "family"
date:  2025-01-20T14:28:24
draft: false

product: "Search"
product_tag: "search"

lang: es

############################# Head ############################
head_title: "Búsqueda de Texto en Documentos e Indexación | API y Aplicación Web Gratuita"
head_description: "Realiza búsquedas de texto eficientes e indexación de datos en PDF, MS Office, OpenDocument y otros formatos de archivo populares utilizando nuestras API o la aplicación gratuita de búsqueda de documentos en línea."

############################# Header ############################
title: "Solución Integral de Búsqueda e Indexación de Documentos"
description:  |
  Realiza búsquedas de texto e indexación en PDF, Microsoft Office, OpenOffice y muchos otros formatos de archivo de documentos.

  Localiza rápidamente información en grandes colecciones de documentos con capacidades avanzadas de búsqueda de texto completo.

  Personaliza las características de búsqueda como sinónimos, búsqueda difusa y lematización para mejorar la precisión y los resultados.

############################# Supported Platforms ###############################
supported_platforms:
  enable: true
  head_title: "Elige tu plataforma"
  title: "Independencia de plataforma"
  description: "GroupDocs.Search es compatible con los siguientes sistemas operativos y marcos:"
  details_link_title: "Aprende más"

  items:
    # items loop
    - title: ".NET"
      description: GroupDocs.Search .NET 
      color: "blue"
      tag: "net"
      link: "/search/net/"
      features_link: "https://docs.groupdocs.com/search/net/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    .NET Framework 4.5 or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows Desktop <br> Windows Server <br> Linux
      
          # features loop
          - rows: "3"
            content: |
                    Microsoft Visual Studio
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Java"
      description: GroupDocs.Search Java
      color: "red"
      tag: "java"
      link: "/search/java/"
      features_link: "https://docs.groupdocs.com/search/java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Java SE 8 (1.8) or later
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                   NetBeans <br> IntelliJ IDEA <br> Eclipse 
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats
      

    # items loop
    - title: "Node.js"
      description: GroupDocs.Search Node.js
      color: "green"
      tag: "nodejs-java"
      link: "/search/nodejs-java/"
      features_link: "https://docs.groupdocs.com/search/nodejs-java/system-requirements/"
      features:
          # features loop
          - rows: "3"
            content: |
                    Node.js 16+ and J2SE 8.0 (1.8)+
      
          # features loop
          - rows: "4"
            content: |
                    Windows <br> Linux <br> Mac OS
      
          # features loop
          - rows: "3"
            content: |
                    Atom <br> Visual Studio Code <br> Cualquier otro editor de texto
      
          # features loop
          - rows: "1"
            content: |
                    70+ file formats


############################# Features ###############################
features:
  enable: true
  title: "Características Clave de GroupDocs.Search"
  description: "GroupDocs.Search proporciona herramientas poderosas para indexar y buscar texto en formatos de documentos populares. Simplifica y mejora la gestión de documentos con funcionalidad avanzada de búsqueda."

  items:
    # items loop
    - icon: "view"
      title: "Búsqueda de texto avanzada"
      content: "Realiza búsquedas de texto rápidas y precisas en documentos indexados."

    # items loop
    - icon: "manipulate"
      title: "Opciones de búsqueda personalizables"
      content: "Aprovecha características como búsqueda difusa, sinónimos y lematización para obtener resultados más precisos."

    # items loop
    - icon: "merge"
      title: "Soporte para múltiples formatos"
      content: "Indexa y busca contenido en Microsoft Office, PDF, OpenOffice y otros formatos comunes."

    # items loop
    - icon: "additional"
      title: "Indexación eficiente"
      content: "Construye y mantiene rápidamente índices para grandes colecciones de documentos."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Buscando texto en formatos de documentos populares"
  description: "GroupDocs.Search ejemplos de código"
  items:
    # code sample loop
    - title: "Búsqueda de Texto"
      content: |
       GroupDocs.Search es una herramienta potente para encontrar texto en documentos. Puedes buscar a través de múltiples documentos en varios formatos almacenados en una carpeta específica. Los resultados de la búsqueda se guardan en una carpeta separada, lo que te permite acceder y reutilizarlos sin tener que realizar la búsqueda nuevamente.
      samples:
        - language: "C#"
          color: "blue"
          content: |
            ```csharp {style=abap}   
            // Crea una instancia de la clase Index, especificando la carpeta para almacenar índices.
            Index index = new Index("\\Index Folder");

            //Especifica la ruta a los documentos donde se realizará la búsqueda.
            index.Add("\\Documents Folder");

            //Crea una instancia del objeto SearchOptions.
            SearchOptions options = new SearchOptions();

            //Realiza la búsqueda del texto deseado.
            SearchResult result = index.Search("ipsum dolor", options);

            //Maneja y procesa los resultados de búsqueda.
            if (result.DocumentCount > 0){
                Console.WriteLine("Documents: " + result.DocumentCount);
                for (int i = 0; i < result.DocumentCount; i++)
                {
                    FoundDocument document = result.GetFoundDocument(i);
                    Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
                    Console.WriteLine("Found: " + document.FoundFields.Length);
                }
            }

            ```
        - language: "Java"
          color: "red"
          content: |
            ```java {style=abap}   
            // Crea una instancia de la clase Index, especificando la carpeta para almacenar índices.
            Index index = new Index("\\Index Folder");

            //Especifica la ruta a los documentos donde se realizará la búsqueda.
            index.add("\\Documents Folder");

            //Crea una instancia del objeto SearchOptions.
            SearchOptions options = new SearchOptions();

            //Realiza la búsqueda del texto deseado.
            SearchResult result = index.search("ipsum dolor", options);

            //Maneja y procesa los resultados de búsqueda.
            if (result.getDocumentCount() > 0){
                System.out.println("Documents: " + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    FoundDocument document = result.getFoundDocument(i);
                    System.out.println("Document: " + document.getDocumentInfo().getFilePath());
                    System.out.println("Found: " + document.getFoundFields().length);
                }
            }

            ```
        - language: "TypeScript"
          color: "green"
          content: |
            ```javascript {style=abap}   
            const searchLib = require('@groupdocs/groupdocs.search');

            // Crea una instancia de la clase Index, especificando la carpeta para almacenar índices.
            const index = new searchLib.Index('\\Index Folder');

            //Especifica la ruta a los documentos donde se realizará la búsqueda.
            index.add('\\Documents Folder');

            //Crea una instancia del objeto SearchOptions.
            const options = new searchLib.SearchOptions();

            //Realiza la búsqueda del texto deseado.
            const result = index.search('ipsum dolor', options);

            //Maneja y procesa los resultados de búsqueda.
            if (result.getDocumentCount() > 0){
                console.log('Documents: ' + result.getDocumentCount());
                for (int i = 0; i < result.getDocumentCount(); i++)
                {
                    const document = result.getFoundDocument(i);
                    console.log('Document: ' + document.getDocumentInfo().getFilePath());
                    console.log('Found: ' + document.getFoundFields().length);
                }
            }

            ```


############################# Supported Formats ###############################
formats:
  enable: true
  title: "Soporta más de 70 formatos de archivo"
  description: "GroupDocs.Search soporta casi todos los formatos de archivo ampliamente utilizados"

############################# Metrics ###############################
metrics:
  enable: true
  title: "Estadísticas de Nuestro Producto"
  description: "Descubre métricas clave que muestran nuestro rendimiento, alcance y crecimiento."

  items:
    # items loop
    - number: "70+"
      title: "Formatos Soportados"
      content: "Proporcionamos compatibilidad con más de 70 formatos de documentos populares."

    # items loop
    - number: "500k"
      title: "Descargas de NuGet"
      content: "GroupDocs.Search para .NET ha sido descargado más de 500,000 veces en NuGet."

    # items loop
    - number: "12k"
      title: "Descargas de Maven"
      content: "Los desarrolladores de Java han descargado GroupDocs.Search más de 12,000 veces desde Maven."

    # items loop
    - number: "150+"
      title: "Clientes Satisfechos"
      content: "Desarrolladores y empresas líderes de todo el mundo confían en nuestros productos para soluciones innovadoras."


############################# Customers ###############################
customers:
  enable: true
  title: "Nuestros Clientes Satisfechos"
  description: "Las bibliotecas de GroupDocs son confiables para las principales marcas y organizaciones en todo el mundo."

  items:
    # items loop
    - title: "BenQ Corporation"
      logo: "benq"
      
    # items loop
    - title: "Nasdaq Stock Market"
      logo: "nasdaq"
      
    # items loop
    - title: "AT&T Inc."
      logo: "att"
      
    # items loop
    - title: "Customer logo AstraZeneca"
      logo: "astrazeneca"
      
    # items loop
    - title: "Central Bank of Argentina"
      logo: "argentinacentralbank"
      
    # items loop
    - title: "Roche Holding AG"
      logo: "roche"
      
    # items loop
    - title: "Capita"
      logo: "capita"
      
    # items loop
    - title: "Axa S.A."
      logo: "axa"
      
    # items loop
    - title: "Instructure Inc."
      logo: "instructure"
      
    # items loop
    - title: "Wipro"
      logo: "wipro"


############################# Actions ###############################
actions:
  enable: true
  title: "¡Comienza Tu Aventura Hoy!"
  description: "Experimenta GroupDocs.Search de forma gratuita en tu plataforma preferida."

  items:
    # items loop
    - title: ".NET"
      color: "blue"
      link: "/search/net/"

    # items loop
    - title: "Java"
      color: "red"
      link: "/search/java/"

    # items loop
    - title: "Node.js via Java"
      color: "green"
      link: "/search/nodejs-java/"

############################# FAQ ###############################
faq:
  enable: true
  title: "Preguntas Frecuentes"
  description: "Encuentra respuestas a preguntas comunes sobre GroupDocs.Search."

  items:
    # items loop
    - question: "¿GroupDocs.Search requiere herramientas externas para buscar documentos?"
      answer: "No, GroupDocs.Search funciona como una solución independiente y no necesita herramientas o software adicionales como Adobe Acrobat o Microsoft Office para realizar búsquedas."

    # items loop
    - question: "¿Puedo probar GroupDocs.Search antes de comprar?"
      answer: "¡Sí, puedes! GroupDocs.Search ofrece una prueba gratuita. Puedes explorar sus características, aunque la versión de prueba puede incluir limitaciones como marcas de agua o funcionalidad restringida. Para desbloquear todas las funciones, puedes solicitar una licencia temporal gratuita de 30 días. Aprende más en la página de [licencia temporal](https://purchase.groupdocs.com/temporary-license/)."

    # items loop
    - question: "¿Cuáles son las opciones de licenciamiento disponibles?"
      answer: "Ofrecemos varios modelos de licenciamiento para GroupDocs.Search, adaptados a diferentes necesidades. Elige una licencia según el tamaño de tu equipo, escenario de uso o si necesitas el SDK/API para distribución al cliente. Para un uso flexible, considera una licencia medida donde pagas según el uso real. Aprende más sobre tus opciones en la página de [precios](https://purchase.groupdocs.com/pricing/search/net/)."

############################# App links ###############################
app_links:
  enable: true
  title: "GroupDocs.Search Aplicaciones Web"
  description: "Explora GroupDocs.Search con nuestra aplicación web gratuita. Realiza búsquedas de texto e indexación en más de 70 formatos de archivo populares directamente en tu navegador, completamente gratis."

  items:
    # items loop
    - title: "GroupDocs.Search Total"
      content: "Busca dentro de PDF, Excel, Word, PowerPoint y otros tipos de archivos directamente desde tu navegador web."
      icon: "groupdocs_watermark-app"
      link: "https://products.groupdocs.app/search/total"

    # items loop
    - title: "GroupDocs.Search Word"
      content: "Carga DOCX para realizar búsquedas de texto avanzadas sin necesidad de instalar software."
      icon: "groupdocs_words-app"
      link: "https://products.groupdocs.app/search/docx"

    # items loop
    - title: "GroupDocs.Search PDF"
      content: "Prueba las capacidades de indexación y recuperación de PDFs en varios formatos de forma gratuita."
      icon: "groupdocs_pdf-app"
      link: "https://products.groupdocs.app/search/pdf"


---