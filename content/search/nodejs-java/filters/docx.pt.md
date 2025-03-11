
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:38
draft: false
lang: pt
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Pesquisar em documentos DOCX usando Node.js"
head_description: "GroupDocs.Search for Node.js via Java adiciona capacidades de busca de texto rápidas e precisas para aplicações JavaScript, suportando múltiplos formatos de documento."

############################# Header ############################
title: "Encontre texto em documentos de negócios" 
description: "GroupDocs.Search for Node.js via Java oferece funcionalidades de busca poderosas e flexíveis para documentos. Integre a busca de texto em aplicações Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar gratuitamente"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) é uma biblioteca robusta de busca e indexação que permite a recuperação rápida de texto em documentos. Suporta mais de 70 formatos de arquivo, incluindo PDFs, Word, Excel e PowerPoint, garantindo buscas precisas e eficientes.

############################# Steps ############################
steps:
    enable: true
    title: "Como realizar uma busca em documentos DOCX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) torna a busca de texto em documentos DOCX simples e eficiente para aplicações Node.js via Java.
      
      1. Crie um diretório para armazenar o índice de busca.
      2. Escolha a pasta que contém os documentos.
      3. Defina as opções de busca para incluir apenas arquivos DOCX.
      4. Execute a busca e recupere os resultados.
   
    code:
      platform: "nodejs-java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
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

        // Defina um diretório para armazenar o índice de busca
        const index = new searchLib.Index("c:/MyIndex");

        // Especifique a pasta que contém os documentos pesquisáveis
        index.add("c:/MyDocuments");

        // Restringa a busca a formatos de arquivo específicos
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".docx");

        // Recupere e processe os resultados da busca
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Recursos avançados de busca"
  description: "GroupDocs.Search for Node.js via Java aumenta a eficiência da busca em documentos indexando mais de 70 formatos de arquivo. Otimize a recuperação de conteúdo com técnicas de busca avançadas."
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "Principais recursos do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca abrangente de texto"
      content: "Extraia e localize texto em formatos de documento populares, como PDFs, arquivos do Word, planilhas e apresentações. Suporta busca difusa, homófonos e consultas com caracteres coringa."

    # feature loop
    - title: "Indexação otimizada para desempenho"
      content: "Acelere as buscas criando índices reutilizáveis. Melhora a velocidade e a eficiência ao lidar com grandes coleções de documentos."

    # feature loop
    - title: "Suporte a múltiplas línguas"
      content: "Busque em documentos em mais de 80 idiomas. Reconhece layouts de teclado e variações de palavras para melhor precisão."

    # feature loop
    - title: "Opções de busca personalizáveis"
      content: "Ajuste os resultados da busca com filtros, expressões regulares, sensibilidade a maiúsculas e minúsculas e outras configurações flexíveis."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Filtrar documentos pesquisáveis"
      content: |
        Aprenda a refinar buscas de documentos usando filtros.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Configure um índice para excluir formatos de arquivo indesejados
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // Especifique o diretório contendo os documentos
          index.add("c:/MyDocuments");

          // Processe a saída da busca para uso posterior
          const result = index.Search("Lorem", options);
          
          // Processe a saída da busca para uso posterior
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "Funcionalidades chave"
    exclude: "filters"
    description: "Realize buscas de texto rápidas e precisas em documentos."
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Buscar em diversos formatos de documento"
    exclude: "DOCX"
    description: "GroupDocs.Search suporta mais de 70 tipos de arquivo, permitindo busca eficiente de texto em vários documentos de escritório e negócios."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---