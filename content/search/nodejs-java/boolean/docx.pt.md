
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: pt
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "Busca booleana em DOCX via Node.js"
head_description: "Utilize a API GroupDocs.Search for Node.js via Java para realizar buscas avançadas no conteúdo de documentos com operadores booleanos como AND, OR e NOT, adaptada para desenvolvedores JavaScript."

############################# Header ############################
title: "Realize buscas com lógica booleana" 
description: "Com GroupDocs.Search for Node.js via Java, você pode criar consultas de busca avançadas usando operadores booleanos (AND, OR, NOT) de forma integrada no seu ambiente Node.js."
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixar Agora"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "O que é GroupDocs.Search?"
    link: "/search/nodejs-java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) é uma ferramenta robusta para buscar e indexar texto em documentos. Suporta mais de 70 formatos como PDF, Word, Excel, PowerPoint, imagens e arquivos ZIP, facilitando o processamento eficiente de grandes volumes de informações.

############################# Steps ############################
steps:
    enable: true
    title: "Como buscar em documentos DOCX usando operadores booleanos"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) permite que você busque conteúdo em arquivos DOCX de forma eficaz. Com a lógica booleana, você pode refinar suas consultas de busca em aplicações Node.js via Java para uma maior precisão.
      
      1. Configure a pasta para armazenar o índice de busca.
      2. Selecione a pasta contendo arquivos DOCX para a busca.
      3. Execute a consulta de busca e recupere os resultados.
      4. Processe e analise os resultados da busca.
   
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

        // Defina a localização da pasta do índice
        const index = new searchLib.Index("c:/MyIndex");

        // Especifique a pasta contendo os documentos para pesquisa
        index.add("c:/MyDocuments");

        // Execute uma consulta de busca com lógica avançada
        const result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ferramentas poderosas para pesquisa e indexação de documentos"
  description: "GroupDocs.Search for Node.js via Java otimiza a busca de texto e a indexação para mais de 70 tipos de arquivos, ajudando você a encontrar e gerenciar informações mais rápido e com precisão."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Recursos principais do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de texto aprimorada"
      content: "Encontre texto rapidamente em vários formatos, como PDFs, documentos Word, apresentações e planilhas. Utilize recursos como correspondências exatas, buscas por wildcards e busca difusa para resultados precisos."

    # feature loop
    - title: "Indexação de dados eficiente"
      content: "Crie e gerencie índices para acelerar buscas em grandes coleções de documentos. A indexação assegura acesso rápido e estruturado aos seus dados."

    # feature loop
    - title: "Suporte multilingue"
      content: "Busque em documentos escritos em mais de 80 idiomas. O suporte morfológico e a compatibilidade com layouts de teclado melhoram os resultados da busca em diferentes idiomas."

    # feature loop
    - title: "Configurações de busca flexíveis"
      content: "Personalize sua busca ativando a sensibilidade a maiúsculas e minúsculas, aplicando filtros de data ou ignorando palavras e dados específicos durante a indexação."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Exemplo de busca booleana avançada"
      content: |
        Este exemplo demonstra como criar consultas baseadas em Booleana para buscar conteúdo em documentos DOCX.
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // Defina a pasta para o índice de busca
          const index = new searchLib.Index("c:/MyIndex");
              
          // Forneça a localização dos documentos a serem pesquisados
          index.add("c:/MyDocuments");

          // Construa uma consulta usando operadores booleanos
          const wordQuery1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wordQuery2 = searchLib.SearchQuery.createWordQuery("ipsum");
          const booleanQuery = searchLib.SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Recupere os resultados da busca
          const result = index.search(booleanQuery);
          
          // Processe e utilize os resultados da busca
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
            link: "/examples/search/formats/searchboolean.docx"
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
    title: "Principais capacidades do GroupDocs.Search"
    exclude: "boolean"
    description: "Desbloqueie recursos de busca avançados, eficientes e personalizáveis."
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
    title: "Busque formatos de documentos populares"
    exclude: "DOCX"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo, proporcionando regras de busca flexíveis e indexação eficiente para economizar tempo e esforço."
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/boolean/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/boolean/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/boolean/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/boolean/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---