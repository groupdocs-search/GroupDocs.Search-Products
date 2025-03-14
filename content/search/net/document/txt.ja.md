
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:49
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "TXT ドキュメントを .NET で検索する GroupDocs.Search"
head_description: "C# を使用して、さまざまなドキュメント形式で効率的なテキスト検索を行うために GroupDocs.Search for .NET を利用してください。"

############################# Header ############################
title: "高度なドキュメントテキスト検索" 
description: "GroupDocs.Search for .NET は人気のあるドキュメント形式でのテキスト検索を簡素化し、.NET アプリケーションで強力な検索クエリを作成できるようにします。"
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
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) は、ドキュメント内でのフルテキスト検索およびインデックス作成のために設計された強力なライブラリです。PDF、Word、PowerPoint、Excel、画像、ZIPファイルを含む70を超えるファイル形式をサポートし、迅速かつ正確な検索結果を保証します。

############################# Steps ############################
steps:
    enable: true
    title: "TXT ドキュメントでのテキスト検索の実行手順"
    content: |
      [GroupDocs.Search](/search/net/) により、TXT ドキュメント内での高度なコンテンツ検索操作を実施でき、.NET アプリケーションで精緻な検索結果を得ることができます。
      
      1. 検索インデックスを保存するフォルダーを設定します。
      2. TXT ファイルが含まれているフォルダーを選択します。
      3. 追加の検索オプションを設定します。
      4. 検索を実行し、結果を確認します。
   
    code:
      platform: "net"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "検索結果"
      install:
        command: "dotnet add package GroupDocs.Search"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらに例を見る"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/search/net/"
          
      content: |
        ```csharp {style=abap}
        // 検索インデックスのためのパスを定義する
        Index index = new Index("c:/MyIndex");

        // 検索するドキュメントが含まれているフォルダーを選択する
        index.Add("c:/MyDocuments");

        // 発音が似ている単語を見つけるために同音検索を有効にする
        SearchOptions options = new SearchOptions();
        options.UseHomophoneSearch = true;

        // 複雑な検索クエリを実行する
        SearchResult result = index.Search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度な検索およびインデックス作成機能"
  description: "GroupDocs.Search for .NET は70を超えるファイル形式でのテキスト検索およびインデックス作成を強化し、情報の取得および管理のための効果的なツールを提供します。"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Search の主な機能"
  features:
    # feature loop
    - title: "強力なテキスト検索"
      content: "PDF、Wordドキュメント、PowerPointプレゼンテーション、スプレッドシートを含む複数のドキュメントタイプでテキストを検索します。正確な一致、あいまい検索、ワイルドカードなどの機能を利用して、結果を絞り込みます。"

    # feature loop
    - title: "大規模データセット向けの高速インデックス作成"
      content: "情報の迅速な取得のために検索インデックスを作成および管理します。インデックス作成により、広範なドキュメントコレクションでの検索が最適化されます。"

    # feature loop
    - title: "多言語サポート"
      content: "80以上の言語で検索を実行し、異なるキーボードレイアウトや単語のバリエーションをサポートして精度を向上させます。"

    # feature loop
    - title: "カスタマイズ可能な検索設定"
      content: "大文字小文字の区別、日付範囲フィルタ、単語排除などのオプションを使用して、検索パラメータを微調整し、より良い結果を得ることができます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度な検索クエリの実行"
      content: |
        この例では、TXT ドキュメントに対して検索クエリを適用する方法を示します。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 検索インデックスのためのフォルダーを定義する
          Index index = new Index("c:/MyIndex");
              
          // ドキュメントファイルへのパスを指定する
          index.Add("c:/MyDocuments");

          // 保護されたドキュメント用のパスワードを提供する
          index.Dictionaries.DocumentPasswords.Add("protected.txt", "123456");

          // 類似単語を見つけるためにあいまい検索を有効にする
          SearchOptions options = new SearchOptions();
          options.FuzzySearch.Enabled = true;
          options.FuzzySearch.FuzzyAlgorithm = new SimilarityLevel(0.8);

          // 検索結果を取得する
          SearchResult result = index.Search("Loarem", options);
          
          // 検索結果を処理する
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
          - title: "結果をダウンロード"
            icon: "download"
            link: "/examples/search/formats/searchdocument.txt"
        links:
          #  loop
          - title: "さらに例を見る"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-.NET/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/search/net/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスを要求してください"
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
    title: "主な機能を探る"
    exclude: "document"
    description: "高度で高性能な検索機能を活用してください。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/net/boolean/txt/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/net/case-sensitive/txt/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/net/document/txt/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/net/filters/txt/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/net/phrase/txt/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ビジネスドキュメントを横断して検索"
    exclude: "TXT"
    description: "GroupDocs.Search は70を超えるファイル形式をサポートし、オフィスドキュメントを含め、インデックス作成機能を備えた迅速かつ効率的な検索を実現します。"
    items: 
        # format loop 1
        - name: "DOCXドキュメント内を検索"
          format: "DOCX"
          link: "/search/net/document/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFドキュメント内を検索"
          format: "PDF"
          link: "/search/net/document/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXドキュメント内を検索"
          format: "PPTX"
          link: "/search/net/document/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTドキュメント内を検索"
          format: "TXT"
          link: "/search/net/document/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXドキュメント内を検索"
          format: "XLSX"
          link: "/search/net/document/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---