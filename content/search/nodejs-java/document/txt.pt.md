
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:50
draft: false
lang: pt
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Encontre texto em TXT com GroupDocs.Search em Node.js"
head_description: "Utilize GroupDocs.Search for Node.js via Java com JavaScript para pesquisar texto de forma eficiente em vários formatos de documentos."

############################# Header ############################
title: "Solução de busca de documentos inteligente" 
description: "Localize texto em diferentes formatos de documentos usando GroupDocs.Search for Node.js via Java. Crie consultas de busca avançadas em suas aplicações Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Experimente Gratuitamente"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Introdução ao GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) é uma biblioteca de alto desempenho para busca de texto completo e indexação de documentos. Suporta mais de 70 tipos de arquivos, incluindo PDF, Word, PowerPoint, Excel, imagens e arquivos ZIP, garantindo resultados rápidos e precisos.

############################# Steps ############################
steps:
    enable: true
    title: "Realizar busca em arquivos TXT"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) permite executar buscas em arquivos TXT, refinando resultados em aplicações Node.js via Java.
      
      1. Defina uma pasta de armazenamento para o índice de busca.
      2. Selecione uma pasta com arquivos TXT.
      3. Defina parâmetros de busca adicionais.
      4. Execute a busca e analise os resultados.
   
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

        // Especifique o diretório para armazenamento do índice de busca
        const index = new searchLib.Index("c:/MyIndex");

        // Escolha a pasta que contém os documentos a serem pesquisados
        index.add("c:/MyDocuments");

        // Ative a busca por homônimos para palavras que soam semelhantes
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // Execute uma consulta de busca complexa
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades avançadas de busca e indexação"
  description: "GroupDocs.Search for Node.js via Java fornece ferramentas poderosas de pesquisa e indexação de texto em mais de 70 formatos de documentos, facilitando a localização e organização de informações."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Principais Benefícios do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de texto abrangente"
      content: "Localize texto em múltiplos tipos de documentos, incluindo PDFs, documentos do Word, apresentações do PowerPoint e planilhas. Use correspondências exatas, busca difusa e curingas para resultados refinados."

    # feature loop
    - title: "Indexação eficiente para grandes volumes de dados"
      content: "Acelere as buscas criando índices estruturados, facilitando a recuperação de informações de grandes coleções de documentos."

    # feature loop
    - title: "Suporte a mais de 80 idiomas"
      content: "Pesquise em documentos em diferentes idiomas, com reconhecimento automático de várias formas de palavras e layouts de teclado."

    # feature loop
    - title: "Configurações de pesquisa personalizadas"
      content: "Ajuste as opções de pesquisa, como sensibilidade ao caso, filtros de data e exclusões de palavras para obter resultados precisos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando busca para documentos TXT"
      content: |
        Este exemplo mostra como usar consultas de busca dentro de documentos TXT.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Defina o diretório para indexação de buscas
          const index = new searchLib.Index("c:/MyIndex");
              
          // Forneça o caminho do arquivo para armazenamento do documento
          index.add("c:/MyDocuments");

          // Insira a senha para arquivos protegidos
          index.getDictionaries().getDocumentPasswords().add("protected.txt", '123456');

          // Ative a busca difusa para detecção de palavras semelhantes
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // Extraia os resultados da busca
          const result = index.search("Loarem", options);
          
          // Procese e revise os resultados
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
            link: "/examples/search/formats/searchdocument.txt"
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
    title: "Explore recursos principais"
    exclude: "document"
    description: "Descubra recursos de busca de alta velocidade projetados para aumentar a eficiência e precisão."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Pesquise em uma variedade de documentos"
    exclude: "TXT"
    description: "GroupDocs.Search funciona com mais de 70 formatos de arquivo, incluindo documentos de escritório, garantindo buscas rápidas e precisas com suporte à indexação."
    items: 
        # format loop 1
        - name: "Buscar no documento DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Buscar no documento PDF"
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Buscar no documento PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Buscar no documento TXT"
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Buscar no documento XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---