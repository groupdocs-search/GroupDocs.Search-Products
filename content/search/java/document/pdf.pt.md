
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: pt
format: Pdf
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Encontre texto em documentos PDF com GroupDocs.Search para Java"
head_description: "GroupDocs.Search for Java ajuda desenvolvedores Java a pesquisar rapidamente textos em vários formatos de documentos."

############################# Header ############################
title: "Pesquisa inteligente de texto em documentos" 
description: "Com GroupDocs.Search for Java, você pode buscar e extrair texto de vários tipos de documentos em suas aplicações Java de forma fluida."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Obtenha um Teste Gratuito"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "O que faz o GroupDocs.Search?"
    link: "/search/java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) é uma biblioteca robusta de pesquisa e indexação de documentos que suporta mais de 70 formatos de arquivo, incluindo PDF, Word, PowerPoint, Excel, imagens e arquivos ZIP. Ele permite capacidades de busca rápidas, precisas e escaláveis para grandes coleções de documentos.

############################# Steps ############################
steps:
    enable: true
    title: "Realizar buscas textuais em arquivos PDF"
    content: |
      [GroupDocs.Search](/search/java/) facilita a busca em arquivos PDF usando lógica sofisticada e indexação, melhorando a precisão das buscas nas aplicações Java.
      
      1. Configure um diretório para armazenar o índice de busca.
      2. Escolha uma pasta contendo arquivos PDF.
      3. Defina opções de busca adicionais.
      4. Execute a busca e analise os resultados.
   
    code:
      platform: "java"
      copy_title: "Copiar"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "Resultado da busca"
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
        copy_tip: "clique para copiar"
        copy_done: "copiado"
      links:
        #  loop
        - title: "Mais exemplos"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
        #  loop
        - title: "Documentação"
          link: "https://docs.groupdocs.com/search/java/"
          
      content: |
        ```java {style=abap}
        // Defina o diretório para armazenar o índice de busca
        Index index = new Index("c:/MyIndex");

        // Especifique a pasta contendo documentos pesquisáveis
        index.add("c:/MyDocuments");

        // Ative a busca de homófonos para corresponder palavras com pronúncias similares
        SearchOptions options = new SearchOptions();
        options.setUseHomophoneSearch(true);

        // Execute uma consulta de busca avançada
        SearchResult result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Capacidades aprimoradas de busca e indexação"
  description: "GroupDocs.Search for Java simplifica a busca e indexação de textos em mais de 70 formatos de documentos, oferecendo ferramentas eficientes para gerenciar e recuperar informações rapidamente."
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "Recursos principais do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de texto abrangente"
      content: "Encontre texto em vários formatos de documentos, como PDFs, documentos do Word, apresentações do PowerPoint e planilhas. Utilize correspondências exatas, busca aproximada e operadores de curinga para resultados de pesquisa refinados."

    # feature loop
    - title: "Indexação otimizada para grandes dados"
      content: "Crie índices estruturados para agilizar as pesquisas, facilitando a navegação por repositórios de documentos extensos de forma eficiente."

    # feature loop
    - title: "Suporte a múltiplas idiomas"
      content: "Realize buscas em mais de 80 idiomas com suporte embutido para diferentes layouts de teclado e variações de morfologia, melhorando a precisão."

    # feature loop
    - title: "Configurações de busca flexíveis"
      content: "Personalize as buscas com opções como sensibilidade a maiúsculas, filtragem por data e a capacidade de excluir palavras específicas para resultados precisos."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Implementando consultas de busca avançadas"
      content: |
        Este exemplo ilustra como usar consultas de busca para pesquisar dentro de documentos PDF de forma eficiente.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Defina o diretório para a indexação de busca
          Index index = new Index("c:/MyIndex");
              
          // Forneça o caminho do arquivo para os documentos
          index.add("c:/MyDocuments");

          // Insira a senha para documentos criptografados
          index.getDictionaries().getDocumentPasswords().add("protected.pdf", "123456");

          // Ative a busca aproximada para detectar palavras similares
          SearchOptions options = new SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new SimilarityLevel(0.8));

          // Busque resultados da pesquisa
          SearchResult result = index.Search("Loarem", options);
          
          // Processar e analisar os resultados da pesquisa
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
          copy_tip: "clique para copiar"
          copy_done: "copiado"
        top_links:
          #  loop
          - title: "Baixar resultado"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pdf"
        links:
          #  loop
          - title: "Mais exemplos"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
          #  loop
          - title: "Documentação"
            link: "https://docs.groupdocs.com/search/java/"
            

            


############################## Actions ############################

actions:
  enable: true
  title: "Pronto para começar?"
  description: "Experimente as funcionalidades do GroupDocs.Search gratuitamente ou solicite uma licença"
  items:
    #  loop
    - title: "Download do Maven"
      link: "https://releases.groupdocs.com/search/java/"
      color: "red"
        #  loop
    - title: "Licenciamento"
      link: "https://purchase.groupdocs.com/pricing/search/java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "Visão geral dos principais recursos"
    exclude: "document"
    description: "Descubra funcionalidades de busca de texto de alto desempenho, projetadas para eficiência e precisão."
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/java/boolean/pdf/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/pdf/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/java/document/pdf/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/java/filters/pdf/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/java/phrase/pdf/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Encontre informações em documentos PDF com GroupDocs.Search"
    exclude: "PDF"
    description: "GroupDocs.Search suporta mais de 70 formatos, incluindo arquivos de escritório, permitindo buscas rápidas com recursos avançados de indexação."
    items: 
        # format loop 1
        - name: "Buscar no documento DOCX"
          format: "DOCX"
          link: "/search/java/document/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Buscar no documento PDF"
          format: "PDF"
          link: "/search/java/document/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Buscar no documento PPTX"
          format: "PPTX"
          link: "/search/java/document/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Buscar no documento TXT"
          format: "TXT"
          link: "/search/java/document/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Buscar no documento XLSX"
          format: "XLSX"
          link: "/search/java/document/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---