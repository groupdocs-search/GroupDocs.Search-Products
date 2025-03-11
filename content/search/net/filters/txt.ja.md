
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:37
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "TXT ドキュメントでの検索 - .NET"
head_description: "GroupDocs.Search for .NET は、さまざまなビジネス文書フォーマットにわたって効率的なテキスト検索を実現する C# アプリケーションを強化します。"

############################# Header ############################
title: "ビジネス文書内のテキストを検索する" 
description: "GroupDocs.Search for .NET により、文書内で強力かつ柔軟なテキスト検索が可能になります。.NET アプリケーションに検索機能を統合してください。"
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search とは？"
    link: "/search/net/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) は、効率的なテキスト検索と文書インデックス作成のための強力なライブラリです。PDF、Word、Excel、PowerPoint などの業界標準の文書を含む 70 以上のファイルフォーマットに対応しています。迅速で正確な結果で検索パフォーマンスを向上させます。

############################# Steps ############################
steps:
    enable: true
    title: "TXT データの検索方法"
    content: |
      [GroupDocs.Search](/search/net/) は、TXT ドキュメント内での効率的なテキスト検索を実現し、.NET アプリケーションに最適です。
      
      1. 検索インデックスを保存するためのフォルダーを設定します。
      2. ファイルを含むフォルダーを選択します。
      3. TXT ドキュメントのみを処理するように検索オプションを構成します。
      4. 検索を実行し、結果を取得します。
   
    code:
      platform: "net"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらに例を見る"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // 再利用可能な検索インデックスを保存するパス
        Index index = new Index("c:/MyIndex");

        // ドキュメントを含むフォルダー
        index.Add("c:/MyDocuments");

        // 特定のファイルフォーマット内のみを検索
        SearchOptions options = new SearchOptions();
        options.SearchDocumentFilter = 
            SearchDocumentFilter.CreateFileExtension(".txt");

        // 検索結果を取得する
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度な検索機能"
  description: "GroupDocs.Search for .NET は、70 以上のファイルフォーマットにわたり洗練されたテキスト検索を実現します。インデックス作成により検索の効率が向上し、文書コンテンツを効果的に管理できます。"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search の主要機能"
  features:
    # feature loop
    - title: "高度なテキスト検索"
      content: "PDF、Word ファイル、プレゼンテーション、スプレッドシートを含む人気のあるビジネス文書から関連するテキストを抽出します。あいまい検索、同音異義語検出、ワイルドカードなどの複数の検索技術に対応しています。"

    # feature loop
    - title: "高速検索のための最適化されたインデックス作成"
      content: "検索速度を向上させるために検索インデックスを構築し、再利用します。大規模な文書コレクションを検索する際のパフォーマンスを最適化します。"

    # feature loop
    - title: "複数言語のサポート"
      content: "80 以上の言語で書かれた文書内で検索を実行できます。異なるキーボードレイアウトや単語のバリエーションを検出して、精度を向上させます。"

    # feature loop
    - title: "柔軟な検索設定"
      content: "フィルター、正規表現、ケースセンシティブ設定などのカスタマイズ可能なオプションで検索結果を絞り込みます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "処理するドキュメントのフィルタリング"
      content: |
        フィルターを使用して文書検索を絞り込む方法を学びます。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 特定のファイルフォーマットを除外するインデックスを設定します。
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            DocumentFilter.CreateFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = DocumentFilter.CreateNot(fileExtensionFilter);
          settings.DocumentFilter = invertedFilter;

          Index index = new Index("c:/MyIndex", settings);
              
          // ドキュメントディレクトリを指定します。
          index.Add("c:/MyDocuments");

          // 検索結果を取得します。
          SearchResult result = index.Search("Lorem");
          
          // 検索結果を処理して使用します。
          Console.WriteLine("Documents: " + result.DocumentCount);
          Console.WriteLine("Occurrences: " + result.OccurrenceCount);
          ```
        platform: "net"
        copy_title: "コピー"
        install:
          command: "dotnet add package GroupDocs.Search"
          copy_tip: "クリックしてコピー"
          copy_done: "コピーしました"
        top_links:
          #  loop
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchfilters.txt"
        links:
          #  loop
          - title: "さらに例を見る"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "ドキュメンテーション"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスをリクエストしてください"
  items:
    #  loop
    - title: "Nugetのダウンロード"
      link: "https://releases.groupdocs.com/search/net/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/search/net/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "主要機能"
    exclude: "filters"
    description: "正確かつ効率的なデータ検索を実行します。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ビジネス文書からデータを見つける"
    exclude: "TXT"
    description: "GroupDocs.Search は 70 以上のファイルフォーマットをサポートし、人気のオフィス文書の効率的な処理と検索を可能にします。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/filters/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/filters/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/filters/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/filters/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/filters/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---