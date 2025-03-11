
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:30
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: ".NET における TXT のブール演算子を使用した検索"
head_description: "GroupDocs.Search for .NET API は C# 開発者が AND、OR、NOT などのブール演算子を使用して文書内容を検索することを可能にします。"

############################# Header ############################
title: "ブール論理テキスト検索" 
description: "GroupDocs.Search for .NET は .NET アプリケーション内でブール演算子 (AND、OR、NOT) を使用して高度な検索クエリを作成することを容易にします。"
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
    title: "GroupDocs.Search とは？"
    link: "/search/net/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/) は、文書内のテキストを検索しインデックスを作成するための包括的なライブラリです。PDF、Word、PowerPoint、Excel、画像、ZIPファイルなど、70以上のファイル形式をサポートしており、大量の情報を効率的に処理できます。

############################# Steps ############################
steps:
    enable: true
    title: "TXT 文書内容をブール論理を使用して検索する方法"
    content: |
      [GroupDocs.Search](/search/net/) は TXT 文書内容を検索するプロセスを簡潔にします。.NET アプリケーションで結果を絞り込むためのブール論理検索条件を提供します。
      
      1. 検索インデックスを保存するフォルダーを指定します。
      2. TXT ファイルを含むフォルダーを選択します。
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
        // インデックスフォルダーのパスを設定
        Index index = new Index("c:/MyIndex");

        // 検索する文書を含むフォルダーを指定
        index.Add("c:/MyDocuments");

        // 複雑なクエリを使用して検索を実行
        SearchResult result = index.Search("lorem AND impsum");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書検索とインデックス作成の高度な機能を探る"
  description: "GroupDocs.Search for .NET ライブラリは70以上のファイル形式に対するテキスト検索とインデックス作成を簡素化します。高度な検索ツールで情報を簡単に見つけ、管理できます。"
  image: "/img/search/features_boolean.webp" # 500x500 px
  image_description: "GroupDocs.Search の主な機能"
  features:
    # feature loop
    - title: "強力なテキスト検索"
      content: "PDF、Word文書、PowerPointプレゼンテーション、スプレッドシートなど、さまざまなファイルタイプのテキストを検索します。正確な一致、ファジー検索、ワイルドカードなどの機能を用いて結果を絞り込むことができます。"

    # feature loop
    - title: "大規模データセットのインデックス作成"
      content: "迅速な検索のためのインデックスを作成・維持します。インデックス作成はデータを構造化し、広範な文書コレクションを検索しやすくします。"

    # feature loop
    - title: "複数言語をサポート"
      content: "80以上の言語で文書を検索でき、異なるキーボードレイアウトや形態素の単語形をサポートし、検索精度を向上させます。"

    # feature loop
    - title: "カスタマイズ可能な検索オプション"
      content: "大文字と小文字の区別、日付範囲フィルター、インデックス作成時に特定の単語やデータを除外する機能など、検索設定を調整できます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度なブール検索クエリの使用"
      content: |
        この例は、TXT 文書の検索に対するブールクエリの適用方法を示しています。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 検索インデックス用のフォルダーを設定
          Index index = new Index("c:/MyIndex");
              
          // 検索対象の文書のパスを指定
          index.Add("c:/MyDocuments");

          // ブール論理を使用して検索クエリを作成
          SearchQuery wordQuery1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wordQuery2 = SearchQuery.CreateWordQuery("ipsum");
          SearchQuery booleanQuery = SearchQuery.CreateAndQuery(wordQuery1, wordQuery2);

          // 検索結果を取得
          SearchResult result = index.Search(booleanQuery);
          
          // 検索結果を処理
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
            link: "/examples/search/formats/searchboolean.txt"
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
    title: "主要な機能を発見"
    exclude: "boolean"
    description: "高度かつ効率的な検索機能を探ります。"
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
    title: "人気の文書形式にまたがる検索"
    exclude: "TXT"
    description: "GroupDocs.Search は70以上のファイル形式をサポートしています。検索ルールをカスタマイズし、インデックス作成を活用して時間と労力を節約できます。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/net/boolean/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/net/boolean/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/net/boolean/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/net/boolean/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/net/boolean/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---