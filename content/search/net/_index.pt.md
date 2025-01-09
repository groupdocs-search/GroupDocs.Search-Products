---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: pt
product: "Search"
product_tag: "search"
platform: "Net"
platform_tag: "net"

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
head_title: "Biblioteca de Pesquisa e Indexação de Documentos .NET para PDFs, Arquivos do Office e Mais"
head_description: "Solução poderosa .NET para pesquisa de texto e indexação em documentos como PDFs, Word, Excel, apresentações, e-mails e formatos da web."

############################# Header ############################
title: "Pesquisa e Indexação Avançada de Documentos com API .NET"
description: "Impulsione aplicativos .NET com capacidades de pesquisa de texto de ponta em formatos de documentos populares."
words:
  for: "para"

actions:
  main: "Baixe Nuget Gratuitamente"
  main_link: "https://www.nuget.org/packages/GroupDocs.Search"
  alt: "Licenciamento"
  alt_link: "https://purchase.groupdocs.com/pricing/search/net/"
  title: "Comece sua jornada hoje!"
  description: "Explore as capacidades do GroupDocs.Search gratuitamente ou obtenha uma licença para desbloquear seu potencial completo."

release:
  title: "Versão {0} lançada"
  notes: "Veja o que há de novo"
  downloads: "Downloads"

code:
  title: "Pesquise Texto em Arquivos de Diretório"
  more: "Mais exemplos"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
  install: "dotnet add package GroupDocs.Search"
  content: |
    ```csharp {style=abap}   
    // Crie um índice para seus documentos
    Index index = new Index("c:/MyIndex");

    // Adicione documentos ao índice para buscas eficientes
    index.Add("c:/MyDocuments");
    
    // Pesquise palavras ou frases específicas, como
    // 'affect', 'effect', 'principles', 'principally'
    SearchResult results = 
        index.Search("'"?ffect & princip?(2~4)"'");
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search Visão Geral"
  description: "Explore a biblioteca .NET C# para pesquisa de texto robusta e indexação."
  features:
    # feature loop
    - title: "Recursos de Indexação e Pesquisa .NET"
      content: "Indexe, armazene e processe dados de documentos de maneira eficiente com GroupDocs.Search for .NET para operações de pesquisa altamente precisas e rápidas."

    # feature loop
    - title: "Combine Índices para Melhor Velocidade de Pesquisa"
      content: "GroupDocs.Search for .NET permite que você mescle múltiplos índices para otimizar o desempenho. Reduza o impacto de índices delta, combinando-os em um índice abrangente para buscas mais suaves."

    # feature loop
    - title: "Pesquise em Diferentes Layouts de Teclado"
      content: "Trate facilmente consultas de busca em 88 idiomas e 164 layouts de teclado com o reconhecimento inteligente do GroupDocs.Search for .NET."

    # feature loop
    - title: "Pesquisas de Palavras Morfológicas"
      content: "GroupDocs.Search for .NET suporta buscas por variações de palavras como substantivos singulares/plurais e diferentes formas verbais, personalizáveis para vários idiomas."

############################# Platforms ############################
platforms:
  enable: true
  title: "Independência de Plataforma"
  description: "GroupDocs.Search for .NET funciona perfeitamente em sistemas operacionais e gerenciadores de pacotes principais."
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
    - title: "VS Code"
      image: "vs_code"
    # platform loop
    - title: "ReSharper"
      image: "resharper"
    # platform loop
    - title: "macOS"
      image: "finder"
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NuGet"
      image: "nuget"

############################# File formats ############################
formats:
  enable: true
  title: "Formatos de arquivo suportados"
  description: |
    Processe uma extensa gama de formatos de arquivo com GroupDocs.Search for .NET. [Veja todos os formatos suportados](https://docs.groupdocs.com/search/net/supported-document-formats/).
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
  title: "Recursos Chave do GroupDocs.Search for .NET"
  description: "Simplifique a gestão de documentos com capacidades de busca avançadas em formatos populares como PDF, DOCX, XLSX, PPTX e mais."

  items:
    # feature loop
    - icon: "document_info"
      title: "Parâmetros de Busca Flexíveis"
      content: "Use filtros como faixas de data e sensibilidade a maiúsculas/minúsculas para refinar sua pesquisa."

    # feature loop
    - icon: "detect"
      title: "Correção Ortográfica Inteligente"
      content: "Pesquise frases com correção ortográfica, caracteres curinga e ignore caracteres especiais."

    # feature loop
    - icon: "collect"
      title: "Resultados de Busca Filtrados"
      content: "Personalize e filtre os resultados da busca por tipo de documento ou critérios."

    # feature loop
    - icon: "get"
      title: "Importação e Exportação de Índices"
      content: "Importe dados, modifique configurações de indexação e exporte resultados indexados."

    # feature loop
    - icon: "remove"
      title: "Exclua Dados Irrelevantes"
      content: "Otimize a indexação pulando arquivos ou palavras específicas."

    # feature loop
    - icon: "style"
      title: "Extração de URL"
      content: "Converta texto formatado em HTML em arquivos e gere links para resultados de busca."

    # feature loop
    - icon: "detect"
      title: "Busca em Alta Velocidade"
      content: "Divida grandes índices em partes menores para processamento mais rápido."

    # feature loop
    - icon: "manipulate"
      title: "Manipulação de Dados Aprimorada"
      content: "Indexe documentos diretamente de fluxos de dados e estruturas."

    # feature loop
    - icon: "compare"
      title: "Detecção de Erros de Digitação"
      content: "Sugira palavras alternativas e rastreie ocorrências para melhorar a precisão."

    # feature loop
    - icon: "unreadable_characters"
      title: "Suporte a Arquivos Compactados"
      content: "Indexe arquivos ZIP aninhados e recupere detalhes de arquivos dentro deles."

    # feature loop
    - icon: "hidden_print"
      title: "Indexação Eficiente"
      content: "Economize espaço em disco com indexação compacta e processe documentos protegidos por senha."

    # feature loop
    - icon: "style"
      title: "Sinônimos Personalizados"
      content: "Adicione e gerencie sinônimos para resultados de busca adaptáveis."

############################# Code samples ############################
code_samples:
  enable: true
  title: "Exemplos de código"
  description: "Descubra as poderosas capacidades do GroupDocs.Search for .NET com exemplos práticos."
  items:
    # code sample loop
    - title: "Aumente a Produtividade com Busca Difusa"
      content: |
        Use GroupDocs.Search for .NET para controle de conteúdo flexível e preciso através de algoritmos de busca avançados. [Explore mais](https://docs.groupdocs.com/search/net/search-results/).
        {{< landing/code title="Como processar o resultado da busca">}}
        ```csharp {style=abap}
        // Crie um índice
        Index index = new Index("C:/IndexFolder");
        index.Add("C:/DocumentFolder");

        // Configure as opções de busca
        SearchOptions options = new SearchOptions();
        options.FuzzySearch.Enabled = true;
        options.FuzzySearch.FuzzyAlgorithm = new TableDiscreteFunction(3);

        // Busque documentos contendo a palavra 'água' ou a frase 'Lorem ipsum'
        string query = "water OR \"Lorem ipsum\"";
        SearchResult result = index.Search(query, options);
        
        // Processe o resultado da busca
        Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
        Console.WriteLine("Occurrences: " + document.OccurrenceCount);
        for (int i = 0; i < result.DocumentCount; i++) {
            FoundDocument document = result.GetFoundDocument(i);
            Console.WriteLine("Document: " + document.DocumentInfo.FilePath);
            Console.WriteLine("Occurrences: " + document.OccurrenceCount);
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "Busca Avançada com Expressões Regulares"
      content: |
        GroupDocs.Search for .NET suporta expressões regulares para buscas precisas. [Aprenda técnicas avançadas](https://docs.groupdocs.com/search/net/regular-expression-search/).
        {{< landing/code title="Como buscar usando expressões regulares">}}
        ```csharp {style=abap}   
        // Crie um índice
        Index index = new Index("c:/IndexFolder");
        index.Add("c:/DocumentFolder");
 
        // Busque a frase em formato de texto

        // O primeiro caractere ^ no início indica que esta é uma consulta de expressão regular
        string query = "^^(.)\\1{1,}";
        // Busque dois ou mais caracteres idênticos no começo de uma palavra
        SearchResult result = index.Search(query);
 
        ```
        {{< /landing/code >}}

---
