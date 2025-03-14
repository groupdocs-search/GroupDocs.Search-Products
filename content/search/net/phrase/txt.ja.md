
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

############################# Head ############################
head_title: "TXT内のフレーズ検索 - GroupDocs.Search for .NET"
head_description: "GroupDocs.Search for .NETは、ドキュメントコンテンツの強力なフレーズ検索機能を持つC#アプリケーションを強化します。"

############################# Header ############################
title: "ドキュメント内のフレーズ検索" 
description: "GroupDocs.Search for .NETを使用して、特定のフレーズを迅速に見つけることができます。効率的な検索機能を.NETアプリケーションに統合しましょう。"
subtitle: "GroupDocs.Search for .NET" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ダウンロード"
      link: "https://releases.groupdocs.com/search/net/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchの機能"
    link: "/search/net/"
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for .NET](/search/net/)は、ドキュメント内のテキストをインデックス作成および検索するための強力なライブラリです。PDF、Word文書、Excelシート、画像、ZIPファイルなど、70以上のファイル形式をサポートし、迅速かつ正確な検索結果を提供します。

############################# Steps ############################
steps:
    enable: true
    title: "TXTドキュメントでフレーズを検索する方法"
    content: |
      [GroupDocs.Search](/search/net/)は、TXTドキュメントでの検索を簡素化します。.NETアプリケーションで検索結果を絞り込むために様々なオプションを使用してください。
      
      1. 検索インデックスフォルダーを設定します。
      2. TXTファイルを含むフォルダーを指定します。
      3. 検索設定を構成します。
      4. 検索結果を取得し、処理します。
   
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
        // 検索インデックスを保存するパス
        Index index = new Index("c:/MyIndex");

        // ドキュメントが含まれるフォルダー
        index.Add("c:/MyDocuments");

        // 検索オプションを設定する
        SearchQuery word1 = SearchQuery.CreateWordQuery("lorem");
        SearchQuery word2 = SearchQuery.CreateWordQuery("ipsum");
        SearchQuery word3 = SearchQuery.CreateWordQuery("dolor");

        SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, word2, word3);

        // 検索を実行する
        SearchResult result = index.Search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: ".NETのドキュメント検索エンジンを発見する"
  description: "GroupDocs.Search for .NETは、70以上のファイル形式にわたってフレーズ検索を可能にします。高度な検索機能を使ってデータを効率的に管理し、位置を特定します。"
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Searchの主要機能"
  features:
    # feature loop
    - title: "フレーズ検索"
      content: "PDF、Wordファイル、プレゼンテーション、スプレッドシートを含むビジネスドキュメント内で正確なフレーズを検索します。正確なフレーズが不明な場合は、ワイルドカードやその他のオプションを使用してください。"

    # feature loop
    - title: "効率的なデータインデックス作成"
      content: "検索インデックスを作成および再利用して、ドキュメント検索の速度を向上させます。インデクシングによりデータが効率的に構造化され、フレーズ検索が迅速になります。"

    # feature loop
    - title: "多言語サポート"
      content: "80以上の言語でドキュメントを検索できます。異なるキーボードレイアウトや形態的な単語形をサポートし、検索の精度を向上させます。"

    # feature loop
    - title: "柔軟な検索オプション"
      content: "大文字小文字の区別、ファジー検索、同音異義語検索、ドキュメントフィルタリングなどの機能で検索をカスタマイズできます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度な検索技術の使用"
      content: |
        TXT内で検索するためのクエリを作成する方法を学びます。
      code:
        title: "C#"
        content: |
          ```csharp {style=abap}
          // 検索インデックス用のフォルダーを指定する
          Index index = new Index("c:/MyIndex");
              
          // 検索用のドキュメントパスを設定する
          index.Add("c:/MyDocuments");

          // 特定のフレーズ用のクエリを作成する
          SearchQuery word1 = SearchQuery.CreateWordQuery("Lorem");
          SearchQuery wildcard = SearchQuery.CreateWildcardQuery(1, 7);
          SearchQuery word2 = SearchQuery.CreateWordQuery("dolor");

          SearchQuery query = SearchQuery.CreatePhraseSearchQuery(word1, wildcard, word2);

          // 検索結果を取得する
          SearchResult result = index.Search(query);
          
          // 結果を処理および利用する
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
            link: "/examples/search/formats/searchphrase.txt"
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
    title: "高度な機能"
    exclude: "phrase"
    description: "強力で効率的な検索機能を活用しましょう。"
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
    title: "ビジネスドキュメントにおけるフレーズ検索"
    exclude: "TXT"
    description: "GroupDocs.Searchは、70以上のドキュメント形式での検索をサポートします。高度なオプションとインデクシングを活用して、検索プロセスを効率化してください。"
    items: 
        # format loop 1
        - name: "DOCXのフレーズ検索"
          format: "DOCX"
          link: "/search/net/phrase/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFのフレーズ検索"
          format: "PDF"
          link: "/search/net/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXのフレーズ検索"
          format: "PPTX"
          link: "/search/net/phrase/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTのフレーズ検索"
          format: "TXT"
          link: "/search/net/phrase/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXのフレーズ検索"
          format: "XLSX"
          link: "/search/net/phrase/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---