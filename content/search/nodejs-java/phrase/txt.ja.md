
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:53
draft: false
lang: ja
format: Txt
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "TXT での検索フレーズ - Node.js"
head_description: "GroupDocs.Search for Node.js via Java は、JavaScript アプリケーションに効率的な文書検索のための強力なフレーズ検索機能を追加します。"

############################# Header ############################
title: "文書内のフレーズを見つける" 
description: "GroupDocs.Search for Node.js via Java を使用して特定のフレーズを迅速に特定します。あなたの Node.js アプリケーションに迅速かつ正確な検索機能を統合しましょう。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "ダウンロード"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search の機能"
    link: "/search/nodejs-java/"
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) は、文書内のテキストをインデックス化し検索するための高性能ライブラリです。70 以上のファイル形式をサポートしており、PDF、Word 文書、Excel スプレッドシート、画像、ZIP アーカイブなど、正確かつ迅速な検索結果を保証します。

############################# Steps ############################
steps:
    enable: true
    title: "TXT 文書内のフレーズを見つける方法"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) は、TXT 文書内でのフレーズ検索を可能にします。 Node.js via Java アプリケーションで異なる検索オプションを適用し、結果を絞り込むことができます。
      
      1. 検索インデックスフォルダーをセットアップします。
      2. TXT ファイルを含むフォルダーを定義します。
      3. 検索パラメーターを設定します。
      4. 検索結果を取得して処理します。
   
    code:
      platform: "nodejs-java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "検索結果"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらに例を見る"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "ドキュメント"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // 検索インデックスを保存するパスを指定します
        const index = new searchLib.Index("c:/MyIndex");

        // 文書を含むフォルダーを設定します
        index.add("c:/MyDocuments");

        // 検索設定を構成します
        const word1 = searchLib.SearchQuery.createWordQuery("lorem");
        const word2 = searchLib.SearchQuery.createWordQuery("ipsum");
        const word3 = searchLib.SearchQuery.createWordQuery("dolor");

        const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, word2, word3);

        // 検索クエリを実行します
        const result = index.search(query);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "Node.js 文書検索エンジンを発見する"
  description: "GroupDocs.Search for Node.js via Java は、70 以上のファイル形式にわたるフレーズ検索を可能にし、高度な検索機能を用いてデータの検索と整理を容易にします。"
  image: "/img/search/features_phrase.webp" # 500x500 px
  image_description: "GroupDocs.Search の主要機能"
  features:
    # feature loop
    - title: "フレーズ検索"
      content: "PDF、Word ファイル、プレゼンテーション、スプレッドシートなどのビジネス文書内で正確なフレーズを見つけます。フルフレーズが不明な場合は、ワイルドカードや柔軟な検索オプションを使用できます。"

    # feature loop
    - title: "最適化されたデータインデックス"
      content: "再利用可能なインデックスを作成することで、検索性能を向上させます。構造化インデックス化により、文書検索が加速され、精度が向上します。"

    # feature loop
    - title: "多言語互換性"
      content: "異なるキーボードレイアウトや形態素の単語変異をサポートし、80 以上の言語で文書を検索し、正確な結果を保証します。"

    # feature loop
    - title: "高度な検索オプション"
      content: "大文字小文字の区別、あいまい一致、同音異義語検出、文書フィルタリングなど、強力な機能を用いて検索をカスタマイズします。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "高度な検索技術の使用"
      content: |
        TXT での検索用クエリの構築方法を学びます。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 検索インデックスディレクトリを定義します
          const index = new searchLib.Index("c:/MyIndex");
              
          // ターゲット文書へのパスを設定します
          index.add("c:/MyDocuments");

          // 目的のフレーズに対するクエリを作成します
          const word1 = searchLib.SearchQuery.createWordQuery("Lorem");
          const wildcard = searchLib.SearchQuery.createWildcardQuery(1, 7);
          const word2 = searchLib.SearchQuery.createWordQuery("dolor");

          const query = searchLib.SearchQuery.createPhraseSearchQuery(word1, wildcard, word2);

          // 検索結果を取得します
          const result = index.search(query);
          
          // 結果を処理して使用します
          console.log('Documents: ' + result.getDocumentCount());
          console.log('Occurrences: ' + result.getOccurrenceCount());
          ```
        platform: "nodejs-java"
        copy_title: "コピー"
        install:
          command: "npm i @groupdocs/groupdocs.search"
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
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "ドキュメント"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスを要求してください"
  items:
    #  loop
    - title: "NPMのダウンロード"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      color: "red"
        #  loop
    - title: "ライセンス"
      link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
      color: "light"


############################# More Operations #####################
more_operations:
    enable: true
    title: "高度な検索機能"
    exclude: "phrase"
    description: "強力な検索機能を活用し、より迅速で正確な結果を得ます。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/txt/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/nodejs-java/document/txt/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/nodejs-java/filters/txt/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/txt/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "ビジネス文書内のフレーズを検索する"
    exclude: "TXT"
    description: "GroupDocs.Search は、70 以上の文書形式でフレーズ検索をサポートします。高度なオプションやインデックス化を利用して、検索プロセスを効率化してください。"
    items: 
        # format loop 1
        - name: "DOCXのフレーズ検索"
          format: "DOCX"
          link: "/search/nodejs-java/phrase/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFのフレーズ検索"
          format: "PDF"
          link: "/search/nodejs-java/phrase/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXのフレーズ検索"
          format: "PPTX"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTのフレーズ検索"
          format: "TXT"
          link: "/search/nodejs-java/phrase/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXのフレーズ検索"
          format: "XLSX"
          link: "/search/nodejs-java/phrase/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---