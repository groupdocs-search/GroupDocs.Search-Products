
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:45
draft: false
lang: pt
format: Txt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Head ############################
head_title: "Pesquisa Booleana em TXT com Java"
head_description: "Com GroupDocs.Search for Java, desenvolvedores podem realizar buscas em documentos utilizando operadores booleanos como AND, OR e NOT."

############################# Header ############################
title: "Pesquisa de texto booleana" 
description: "Utilize GroupDocs.Search for Java para criar consultas avançadas de busca booleana (AND, OR, NOT) em seus projetos Java."
subtitle: "GroupDocs.Search for Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "Baixe Gratuitamente"
      link: "https://releases.groupdocs.com/search/java/"
      
############################# About ############################
about:
    enable: true
    title: "Sobre GroupDocs.Search"
    link: "/search/java/"
    link_title: "Saiba mais"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Java](/search/java/) é uma biblioteca versátil projetada para busca de texto e indexação de dados em documentos. Ela suporta mais de 70 tipos de arquivos, incluindo PDF, Word, Excel, PowerPoint, imagens e arquivos ZIP, permitindo buscas eficientes em grandes coleções de dados.

############################# Steps ############################
steps:
    enable: true
    title: "Como realizar buscas booleanas em documentos TXT"
    content: |
      [GroupDocs.Search](/search/java/) permite buscas de texto dentro de documentos TXT. Com suporte a condições booleanas, você pode aumentar a precisão da busca em aplicações Java.
      
      1. Especifique a pasta para armazenar o índice de busca.
      2. Selecione a pasta que contém documentos TXT.
      3. Execute a consulta de busca e recupere os resultados.
      4. Processar os resultados obtidos.
   
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
        // Defina o caminho para a pasta do índice
        Index index = new Index("c:/MyIndex");

        // Forneça o caminho da pasta que contém documentos para a busca
        index.add("c:/MyDocuments");

        // Execute uma busca com uma consulta complexa
        SearchResult result = index.search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Ferramentas poderosas para busca e indexação de documentos"
  description: "GroupDocs.Search for Java simplifica buscas de texto e indexação de dados para mais de 70 formatos. Suas ferramentas avançadas permitem encontrar e gerenciar conteúdos de forma eficiente."
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "Principais recursos do GroupDocs.Search"
  features:
    # feature loop
    - title: "Busca de texto abrangente"
      content: "Pesquise entre múltiplos formatos como PDFs, documentos do Word, apresentações, planilhas e mais. Utilize opções como correspondência exata, busca difusa e consultas com caracteres curinga para refinar os resultados."

    # feature loop
    - title: "Indexação de dados eficiente"
      content: "Crie e mantenha índices para buscas de documentos mais rápidas. Este recurso organiza os dados de forma eficiente, facilitando o manuseio de grandes coleções de documentos."

    # feature loop
    - title: "Suporte a múltiplas línguas"
      content: "Pesquise em documentos escritos em mais de 80 idiomas. Aumente a precisão aproveitando formas morfológicas de palavras e diferentes layouts de teclado."

    # feature loop
    - title: "Personalização flexível da busca"
      content: "Ajuste as configurações de busca com recursos como sensibilidade a maiúsculas, filtros de intervalo de datas e exclusões para refinar seus resultados."
      
  code_samples_ext:
    # code sample ext loop
    - title: "Usando consultas de busca booleana complexas"
      content: |
        Este exemplo demonstra como realizar buscas booleanas em arquivos TXT.
      code:
        title: "Java"
        content: |
          ```java {style=abap}
          // Defina a pasta para o índice de busca
          Index index = new Index("c:/MyIndex");
              
          // Forneça o caminho para os documentos a serem pesquisados
          index.add("c:/MyDocuments");

          // Construa a consulta utilizando lógica booleana
          SearchQuery wordQuery1 = SearchQuery.createWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.createWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.createAndQuery(wordQuery1, wordQuery2);

          // Recupere os resultados da busca
          SearchResult result = index.search(booleanQuery);
          
          // Processar os resultados recuperados
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "Principais recursos em um relance"
    exclude: "boolean"
    description: "Desbloqueie capacidades de busca poderosas e eficientes"
    items: 
          
        # operation loop 1
        - name: "Busca por condição"
          operation: "boolean"
          link: "/search/java/boolean/txt/"
          description: "Encontre informações em documentos usando condições booleanas"

        # operation loop 2
        - name: "Busca sensível a maiúsculas"
          operation: "case-sensitive"
          link: "/search/java/case-sensitive/txt/"
          description: "Aprimore a precisão da busca considerando a sensibilidade a maiúsculas"

        # operation loop 3
        - name: "Indexação de documentos"
          operation: "document"
          link: "/search/java/document/txt/"
          description: "Indexe documentos uma vez e reutilize o índice para múltiplas buscas"

        # operation loop 4
        - name: "Filtros de busca"
          operation: "filters"
          link: "/search/java/filters/txt/"
          description: "Use filtros para restringir os dados processados"

        # operation loop 5
        - name: "Frase exata"
          operation: "phrase"
          link: "/search/java/phrase/txt/"
          description: "Busque por uma frase ou sentença específica"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "Pesquise formatos de documentos populares"
    exclude: "TXT"
    description: "GroupDocs.Search suporta mais de 70 formatos de arquivo, permitindo que você personalize regras de busca e utilize indexação para otimizar o desempenho."
    items: 
        # format loop 1
        - name: "Busca booleana em DOCX"
          format: "DOCX"
          link: "/search/java/boolean/docx/"
          description: "Documento Microsoft Word Open XML"
          
        # format loop 2
        - name: "Busca booleana em PDF"
          format: "PDF"
          link: "/search/java/boolean/pdf/"
          description: "Formato de Documento Portátil Adobe"
          
        # format loop 3
        - name: "Busca booleana em PPTX"
          format: "PPTX"
          link: "/search/java/boolean/pptx/"
          description: "Apresentação PowerPoint Open XML"

        # format loop 4
        - name: "Busca booleana em TXT"
          format: "TXT"
          link: "/search/java/boolean/txt/"
          description: "Documento de Texto"
          
        # format loop 5
        - name: "Busca booleana em XLSX"
          format: "XLSX"
          link: "/search/java/boolean/xlsx/"
          description: "Planilha Microsoft Excel Open XML"
  

---