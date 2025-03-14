
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: pt
format: Xlsx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Pesquisar frases em XLSX usando Node.js"
head_description: "GroupDocs.Search for Node.js via Java adiciona uma poderosa funcionalidade de busca de frases a aplicativos JavaScript para uma pesquisa de documentos eficiente."

############################# Header ############################
title: "Encontre frases em documentos" 
description: "Localize rapidamente frases específicas com GroupDocs.Search for Node.js via Java. Integre capacidades de busca rápidas e precisas em seus aplicativos Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "Recursos do GroupDocs.Search"
    link: "/search/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) é uma biblioteca de alto desempenho para indexação e busca de texto em documentos. Suporta mais de 70 formatos de arquivo, incluindo PDFs, documentos Word, planilhas Excel, imagens e arquivos ZIP, garantindo resultados de busca precisos e rápidos.

############################# Steps ############################
steps:
    enable: true
    title: "Como encontrar frases em documentos XLSX"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) facilita a busca de frases em documentos XLSX. Aplique diferentes opções de busca para refinar os resultados em aplicativos Node.js via Java.
      
      1. Configure uma pasta para o índice de busca.
      2. Defina a pasta que contém os arquivos XLSX.
      3. Configure os parâmetros da busca.
      4. Recupere e processe os resultados da busca.
   
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

        // Especifique o caminho para armazenar o índice de busca
        const index = new searchLib.Index("c:/MyIndex");

        // Defina a pasta contendo os documentos
        index.add("c:/MyDocuments");

        // Configure as definições de busca
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // Execute a consulta de busca
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Descubra o mecanismo de busca de documentos Node.js"
  description: "GroupDocs.Search for Node.js via Java permite buscas de frases em mais de 70 formatos de arquivo, facilitando a localização e organização de dados com recursos avançados de pesquisa."
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "Principais capacidades do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca por frase"
      content: "Encontre frases exatas em documentos comerciais como PDFs, arquivos Word, apresentações e planilhas. Utilize curingas e opções de busca flexíveis quando a frase completa for desconhecida."

    # feature loop
    - title: "Indexação de dados otimizada"
      content: "Aumente o desempenho da busca criando índices reutilizáveis. A indexação estruturada acelera as buscas em documentos e melhora a precisão."

    # feature loop
    - title: "Compatibilidade multilingue"
      content: "Pesquise documentos em mais de 80 idiomas com suporte para diferentes layouts de teclado e variações morfológicas das palavras, garantindo resultados precisos."

    # feature loop
    - title: "Opções de busca avançadas"
      content: "Personalize buscas com sensibilidade a maiúsculas, correspondência difusa, detecção de homófonos, filtragem de documentos e outros recursos poderosos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando técnicas de busca avançadas"
      content: |
        Aprenda a construir consultas para busca em XLSX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Defina o diretório do índice de busca
          const index = new searchLib.Index("c:/MyIndex");
              
          // Defina o caminho para os documentos de destino
          index.add("c:/MyDocuments");

          // Crie uma consulta para a frase desejada
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // Recupere os resultados da busca
          const result = index.search(query);
          
          // Processe e utilize os resultados
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
            link: "/examples/search/formats/searchphrase.xlsx"
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
    title: "Recursos de busca avançados"
    exclude: "phrase"
    description: "Aproveite recursos de busca poderosos para resultados mais rápidos e precisos."
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
    title: "Pesquise frases em documentos comerciais"
    exclude: "XLSX"
    description: "GroupDocs.Search suporta busca de frases em mais de 70 formatos de documento. Utilize opções avançadas e indexação para otimizar o processo de busca."
    items: 
        # format loop 1
        - name: "Busca de frases em DOCX"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Busca de frases em PDF"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Busca de frases em PPTX"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Busca de frases em TXT"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Busca de frases em XLSX"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---