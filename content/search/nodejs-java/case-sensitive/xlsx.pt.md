
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:48
draft: false
lang: pt
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Realize Pesquisas com Sensibilidade a Maiúsculas em XLSX com Node.js"
head_description: "A API GroupDocs.Search for Node.js via Java permite que desenvolvedores JavaScript executem pesquisas com sensibilidade a maiúsculas em diferentes tipos de documentos."

############################# Header ############################
title: "Pesquisa com Sensibilidade a Maiúsculas" 
description: "GroupDocs.Search for Node.js via Java permite implementar funcionalidades avançadas de pesquisa com sensibilidade a maiúsculas em suas aplicações Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar Gratuito"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) é uma biblioteca poderosa para pesquisar e indexar texto em documentos. Suporta mais de 70 formatos, incluindo PDFs, Word, Excel, PowerPoint, imagens e arquivos ZIP, permitindo o manuseio eficiente de grandes volumes de dados.

############################# Steps ############################
steps:
    enable: true
    title: "Etapas para Realizar Pesquisas com Sensibilidade a Maiúsculas em Arquivos XLSX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilita a realização de pesquisas com sensibilidade a maiúsculas em arquivos XLSX, aprimorando seus fluxos de trabalho Node.js via Java.
      
      1. Configure uma pasta para armazenar o índice de pesquisa.
      2. Selecione a pasta que contém arquivos XLSX.
      3. Execute a pesquisa e obtenha os resultados.
      4. Processar e utilizar os resultados.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado da busca"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // Especifique o caminho para a pasta do índice
        const index = new searchLib.Index("c:/MyIndex");

        // Defina a pasta que contém os documentos a serem pesquisados
        index.add("c:/MyDocuments");

        // Ative a pesquisa com sensibilidade a maiúsculas nas configurações
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // Execute a pesquisa
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Principais Funcionalidades para Pesquisa e Indexação de Documentos"
  description: "Com GroupDocs.Search for Node.js via Java, você pode pesquisar e indexar texto em mais de 70 formatos de arquivo. Acesse e organize informações de forma eficiente usando ferramentas de pesquisa avançadas."
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "Recursos Principais do GroupDocs.Search"
  features:
    # feature loop
    - title: "Pesquisa de Texto Abrangente"
      content: "Encontre texto em vários tipos de documentos, como PDFs, arquivos Word, planilhas e apresentações. Utilize opções como correspondências exatas, pesquisas aproximadas e curingas para resultados precisos."

    # feature loop
    - title: "Indexação de Dados Eficiente"
      content: "Crie e gerencie índices para agilizar as pesquisas. A indexação ajuda a organizar e localizar rapidamente dados em grandes coleções de documentos."

    # feature loop
    - title: "Suporte a Múltiplas Línguas"
      content: "Pesquise documentos em mais de 80 idiomas com suporte a diversos layouts de teclado e variações de palavras, garantindo resultados de pesquisa precisos."

    # feature loop
    - title: "Configurações de Pesquisa Personalizáveis"
      content: "Ajuste as configurações de pesquisa, incluindo sensibilidade a maiúsculas, filtros de data e exclusão de termos ou dados específicos durante a indexação."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemplo: Implementação de Pesquisa com Sensibilidade a Maiúsculas"
      content: |
        Este exemplo demonstra como realizar pesquisas com sensibilidade a maiúsculas para documentos XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Defina a pasta para o índice de pesquisa
          const index = new searchLib.Index("c:/MyIndex");
              
          // Forneça o caminho para a pasta de documentos
          index.add("c:/MyDocuments");

          // Configure uma consulta de pesquisa
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // Ative as configurações de pesquisa sensíveis a maiúsculas
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // Pesquise o texto nos documentos
          const result = index.search(wordQuery, options);
          
          // Processar e manipular os resultados
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "Copiar"
        install:
          command: "npm i @groupdocs/groupdocs.search"
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/search/formats/searchcase-sensitive.xlsx"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente as funcionalidades do GroupDocs.Search gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Download do NPM"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Funcionalidades Principais"
    exclude: "case-sensitive"
    description: "Explore recursos avançados para buscas rápidas e precisas em documentos."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Formatos de Documentos Compatíveis"
    exclude: "XLSX"
    description: "GroupDocs.Search suporta mais de 70 formatos de documentos. Personalize suas opções de pesquisa e economize tempo com a indexação."
    items: 
        # format loop 1
        - name: "Busca sensível a maiúsculas em DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Busca sensível a maiúsculas em PDF"
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Busca sensível a maiúsculas em PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Busca sensível a maiúsculas em TXT"
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Busca sensível a maiúsculas em XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---