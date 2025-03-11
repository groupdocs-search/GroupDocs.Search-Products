
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:32
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "TXTにおける.NETの大文字小文字を区別する検索"
head_description: "GroupDocs.Search for .NET APIは、C#開発者がさまざまなドキュメントで大文字小文字を区別した検索を行うことを可能にします。"

############################# Header ############################
title: "大文字小文字を区別する検索" 
description: "GroupDocs.Search for .NETを使用すると、.NETアプリケーション内で高度な大文字小文字を区別した検索クエリを作成できます。"
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料ダウンロード"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchとは何ですか？"
    link: "/search/net/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/)は、文書内のテキスト検索およびインデックス作成を効率的に行うための強力なライブラリです。PDF、Word、PowerPoint、Excel、画像、ZIPファイルなど、70以上のファイル形式をサポートしており、大量データの取り扱いを確実にします。

############################# Steps ############################
steps:
    enable: true
    title: "TXT文書での大文字小文字を区別した検索の実行方法"
    content: |
      [GroupDocs.Search](/search/net/)は、TXT文書での大文字小文字を区別する検索を簡素化します。.NETアプリケーション内で結果を洗練させるために使用できます。
      
      1. 検索インデックスを格納するフォルダーを定義します。
      2. TXTファイルを含むフォルダーを選択します。
      3. 検索を実行し、結果を取得します。
      4. 結果を処理します。
   
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
        // インデックスフォルダーへのパスを設定します
        Index index = new Index("c:/MyIndex");

        // 検索するドキュメントを含むフォルダーを指定します
        index.Add("c:/MyDocuments");

        // オプションで大文字小文字を区別する検索を有効にします
        SearchOptions options = new SearchOptions();
        options.UseCaseSensitiveSearch = true;

        // 検索を実行します
        SearchResult result = index.Search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書検索およびインデックス作成のための高度な機能"
  description: "GroupDocs.Search for .NETライブラリは、70以上のファイル形式でのテキスト検索およびインデックス作成を簡素化します。強力な検索ツールを使って情報を効率的に特定し、管理できます。"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Searchの主な機能"
  features:
    # feature loop
    - title: "高度なテキスト検索"
      content: "PDF、Word文書、スプレッドシート、プレゼンテーションなど、さまざまなファイル形式でテキストを検索します。正確な結果を得るために、完全一致、ファジー検索、ワイルドカードなどのオプションを使用します。"

    # feature loop
    - title: "大規模データセットのインデックス作成"
      content: "より迅速な検索のためのインデックスを構築および管理します。組織的なインデックス作成により、膨大な文書コレクションの検索が簡素化されます。"

    # feature loop
    - title: "多言語サポート"
      content: "80以上の言語でドキュメントを検索し、さまざまなキーボードレイアウトや単語形態をサポートすることで、より正確な結果を得られます。"

    # feature loop
    - title: "カスタマイズ可能な検索オプション"
      content: "大文字小文字の区別、日付範囲フィルター、インデックス作成時に特定の単語やデータを除外する機能など、検索設定をカスタマイズできます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "大文字小文字を区別する検索クエリの使用"
      content: |
        この例では、TXT文書を検索するための大文字小文字を区別したクエリの使用方法を示しています。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 検索インデックスのフォルダーを設定します
          Index index = new Index("c:/MyIndex");
              
          // 検索対象の文書へのパスを指定します
          index.Add("c:/MyDocuments");

          // 検索クエリを作成します
          SearchQuery wordQuery = SearchQuery.CreateWordQuery("Lorem");

          // 大文字小文字を区別する検索オプションを有効にします
          SearchOptions options = new SearchOptions();
          options.UseCaseSensitiveSearch = true;

          // 文書内のテキストを検索します
          SearchResult result = index.Search(wordQuery, options);
          
          // 検索結果を処理します
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
            link: "/examples/search/formats/searchcase-sensitive.txt"
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
    title: "主な機能を発見する"
    exclude: "case-sensitive"
    description: "高度で効率的な検索機能を探求しましょう。"
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
    title: "人気の文書フォーマットを検索"
    exclude: "TXT"
    description: "GroupDocs.Searchは70以上のファイル形式をサポートします。検索ルールをカスタマイズし、インデックス作成を活用して時間と労力を節約しましょう。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/case-sensitive/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/case-sensitive/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/case-sensitive/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/case-sensitive/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/case-sensitive/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---