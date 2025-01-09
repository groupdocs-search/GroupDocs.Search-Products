---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: pt
product: "Search"
product_tag: "search"
platform: "Java"
platform_tag: "java"

############################# Drop-down ############################
supported_platforms:
  items:
    # supported_platforms loop
    - title: ".NET"
      tag: "net"
    # supported_platforms loop
    - title: "Java"
      tag: "java"
    # supported_platforms loop
    - title: "Node.js"
      tag: "nodejs-java"

############################# Head ############################
head_title: "Solução de Pesquisa e Indexação de Documentos Java para PDFs, Arquivos do Office e Conteúdo da Web"
head_description: "Pesquisa de texto poderosa e indexação para aplicativos Java. Busque e organize dados em PDFs, Word, Excel, apresentações, e-mails e formatos da web."

############################# Header ############################
title: "Pesquisa e Indexação Eficientes de Documentos com API Java"
description: "Capacite aplicativos Java com robustas funcionalidades de pesquisa de texto em todos os formatos de documentos populares."
words:
  for: "para"

actions:
  main: "Baixe Maven Gratuitamente"
  main_link: "https://releases.groupdocs.com/java/repo/com/groupdocs/groupdocs-search/"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/search/java/"
  title: "Comece sua jornada hoje!"
  description: "Explore as capacidades do GroupDocs.Search gratuitamente ou obtenha uma licença para desbloquear seu potencial completo."

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"

code:
  title: "Encontre Texto em Arquivos Usando Java"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Java/"
  install_title : "Maven XML"
  install: |
    <dependency>
      <groupId>com.groupdocs</groupId>
      <artifactId>groupdocs-search</artifactId>
      <version>{0}</version>
    </dependency>
  content: |
    ```java {style=abap}  
    // Crie um índice para seus documentos
    Index index = new Index("c:/MyIndex");

    // Adicione documentos ao índice para buscas eficientes
    index.add("c:/MyDocuments");
    
    // Pesquise palavras ou frases específicas, como
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.search("?ffect & princip?(2~4)");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Visão Geral"
  description: "Descubra as poderosas capacidades de pesquisa de texto da biblioteca Java Java."
  features:
    # feature loop
    - title: "Operações de Indexação e Pesquisa em Java"
      content: "Com GroupDocs.Search for Java, você pode coletar, armazenar e analisar dados de maneira eficiente para criar índices detalhados para buscas mais rápidas e precisas."

    # feature loop
    - title: "Otimize a Busca Mesclando Índices"
      content: "Combine facilmente múltiplos índices com GroupDocs.Search for Java para simplificar as buscas. Reduza o impacto de índices delta menores consolidando-os em um único índice de alto desempenho."

    # feature loop
    - title: "Suporte a Layouts de Teclado Multilíngues"
      content: "Pesquise em diferentes idiomas e layouts de teclado com GroupDocs.Search for Java. Suporta 88 idiomas e 164 configurações de teclado para versatilidade incomparável."

    # feature loop
    - title: "Capacidades de Pesquisa Morfológicas"
      content: "Encontre diferentes formas de palavras, como substantivos singulares/plurais ou variações verbais usando GroupDocs.Search for Java. Personalize as opções de busca para inglês e outros idiomas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de Plataforma"
  description: "GroupDocs.Search for Java é compatível com principais sistemas operacionais e gerenciadores de pacotes."
  items:
    # platform loop
    - title: "Amazon"
      image: "amazon"
    # platform loop
    - title: "Docker"
      image: "docker"
    # platform loop
    - title: "Azure"
      image: "azure"
    # platform loop
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "Maven"
      image: "maven"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    Trabalhe com uma ampla gama de formatos de arquivo usando GroupDocs.Search for Java. [Veja a lista completa](https://docs.groupdocs.com/search/java/supported-document-formats/).
  groups:
    # group loop
    - color: "green"
      content: |
        ### Formatos de Escritório Populares
        * **Portátil:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **Texto:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### Formatos de Mídia
        * **Formatos de imagem populares:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **Imagens multi-página:** GIF, WEBP, TIFF
        * **Áudio:** MP3, WAV
        * **Vídeo:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### Outros
        * **Email:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **Web:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **Outros:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "Recursos do GroupDocs.Search for Java"
  description: "Gerencie o conteúdo de documentos de forma eficaz com capacidades de busca avançadas que suportam formatos como PDF, DOCX, XLSX, PPTX e mais."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parâmetros de Busca Personalizáveis"
      content: "Refine buscas usando faixas de data e filtros de sensibilidade a maiúsculas/minúsculas."

    # feature loop
    - icon: "detect"
      title: "Correção Ortográfica Aprimorada"
      content: "Pesquise de forma eficiente com correção ortográfica, caracteres curinga e ignorando caracteres especiais."

    # feature loop
    - icon: "collect"
      title: "Resultados de Busca Filtrados"
      content: "Aplique filtros para focar os resultados da busca com base em tipos específicos de documento ou critérios."

    # feature loop
    - icon: "get"
      title: "Importação e Exportação de Dados de Índice"
      content: "Importe facilmente dados para indexação ou exporte resultados para arquivos para uso posterior."

    # feature loop
    - icon: "remove"
      title: "Pule Arquivos Desnecessários"
      content: "Otimize a indexação excluindo arquivos ou palavras específicas."

    # feature loop
    - icon: "style"
      title: "Processamento de HTML e URL"
      content: "Extraia conteúdo HTML para arquivos e gere URLs para navegação através dos resultados da busca."

    # feature loop
    - icon: "detect"
      title: "Busca Rápida em Grandes Índices"
      content: "Acelere as operações de busca dividindo grandes índices em pedaços gerenciáveis."

    # feature loop
    - icon: "manipulate"
      title: "Indexação Baseada em Fluxos"
      content: "Indexe dados diretamente de fluxos ou estruturas de dados."

    # feature loop
    - icon: "compare"
      title: "Tratamento de Consultas Mal Escritas"
      content: "Detecte erros de digitação e sugira palavras alternativas para melhor precisão na busca."

    # feature loop
    - icon: "unreadable_characters"
      title: "Suporte Abrangente a Arquivos Compactados"
      content: "Indexe arquivos compactados aninhados e recupere listas detalhadas de arquivos dentro de arquivos ZIP."

    # feature loop
    - icon: "hidden_print"
      title: "Indexação que Economiza Espaço"
      content: "Compacte índices para economizar espaço em disco e processe arquivos protegidos por senha."

    # feature loop
    - icon: "style"
      title: "Suporte a Sinônimos Personalizados"
      content: "Expanda o dicionário de sinônimos para melhorar a precisão da busca com opções personalizadas."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemplos de código"
  description: "Experimente os recursos do GroupDocs.Search for Java com estes exemplos de código."
  items:
    # code sample loop
    - title: "Aumente a Precisão da Busca com Correspondência Difusa"
      content: |
        Explore a flexibilidade do GroupDocs.Search for Java para gerenciar conteúdo com capacidades avançadas de busca difusa. [Saiba mais](https://docs.groupdocs.com/search/java/search-results/).
        {{< landing/code title="Como processar o resultado da busca">}}
        ```java {style=abap}
        // Crie um índice
        Index index = new Index("C:/IndexFolder");
        index.add("C:/DocumentFolder");

        // Configure as opções de busca
        SearchOptions options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // Busque documentos contendo a palavra 'água' ou a frase 'Lorem ipsum'
        String query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.search(query, options);
        
        // Processe o resultado da busca
        System.out.println("Documents: " + result.getDocumentCount());
        System.out.println("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            System.out.println("Document: " + document.getDocumentInfo().getFilePath());
            System.out.println("Occurrences " + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Refine Resultados com Expressões Regulares"
      content: |
        Use expressões regulares no GroupDocs.Search for Java para criar resultados de busca precisos e detalhados. [Descubra técnicas avançadas](https://docs.groupdocs.com/search/java/regular-expression-search/).
        {{< landing/code title="Como buscar usando expressões regulares">}}
        ```java {style=abap}   
        // Crie um índice
        Index index = new Index("C:/IndexFolder");
        index.add("c:/DocumentFolder");
 
        // Busque a frase em formato de texto

        // O primeiro caractere ^ no início indica que esta é uma consulta de expressão regular
        String query = "^^(.)\\1{1,}";
        // Busque dois ou mais caracteres idênticos no começo de uma palavra
        SearchResult result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
