
---
############################# Static ############################
layout: "format"
date:  2025-03-14T11:10:51
draft: false
lang: ja
format: Docx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "DOCX ドキュメント内の検索 - Node.js 用"
head_description: "GroupDocs.Search for Node.js via Java は、複数のドキュメント形式をサポートし、JavaScript アプリケーションに迅速かつ正確なテキスト検索機能を追加します。"

############################# Header ############################
title: "ビジネス文書内のテキストを見つける" 
description: "GroupDocs.Search for Node.js via Java は、ドキュメント向けに強力かつ柔軟な検索機能を提供します。Node.js アプリケーションにテキスト検索を統合することができます。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料でダウンロード"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Search とは？"
    link: "/search/nodejs-java/"
    link_title: "さらに詳しく"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) は、文書内の迅速なテキスト検索を可能にする堅牢な検索およびインデックス作成ライブラリです。PDF、Word、Excel、PowerPointを含む70以上のファイル形式をサポートしており、正確かつ効率的な検索を実現します。

############################# Steps ############################
steps:
    enable: true
    title: "DOCX ドキュメントでの検索方法"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) は、Node.js via Java アプリケーション向けに DOCX ドキュメント内のテキスト検索を簡単かつ効率的に行えます。
      
      1. 検索インデックスを保存するディレクトリを作成します。
      2. 文書を含むフォルダを選択します。
      3. DOCX ファイルのみを含むように検索オプションを設定します。
      4. 検索を実行し、結果を取得します。
   
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

        // 検索インデックスを保存するディレクトリを定義します
        const index = new searchLib.Index("c:/MyIndex");

        // 検索可能なドキュメントを含むフォルダを指定します
        index.add("c:/MyDocuments");

        // 特定のファイル形式に検索を制限します
        const options = new searchLib.SearchOptions();
        options.SearchDocumentFilter = 
            searchLib.SearchDocumentFilter.createFileExtension(".docx");

        // 検索結果を取得し、処理します
        const result = index.search("Lorem");
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度な検索機能"
  description: "GroupDocs.Search for Node.js via Java は70以上のファイル形式をインデックス化することで、文書検索の効率を向上させます。高度な検索技術を使用してコンテンツの取得を最適化します。"
  image: "/img/search/features_filters.webp" # 500x500 px
  image_description: "GroupDocs.Search の主要機能"
  features:
    # feature loop
    - title: "包括的なテキスト検索"
      content: "PDF、Word ドキュメント、スプレッドシート、プレゼンテーションなどの一般的なドキュメント形式からテキストを抽出し、見つけ出します。ファジー検索、同音異義語、ワイルドカードクエリをサポートしています。"

    # feature loop
    - title: "パフォーマンス向けに最適化されたインデックス"
      content: "再利用可能なインデックスを作成することで検索を加速します。大規模なドキュメントコレクションでの速度と効率を向上させます。"

    # feature loop
    - title: "多言語サポート"
      content: "80以上の言語で文書を検索します。キーボードレイアウトや単語の変種を認識し、精度を向上させます。"

    # feature loop
    - title: "カスタマイズ可能な検索オプション"
      content: "フィルタ、正規表現、大文字小文字の区別、その他の柔軟な設定で検索結果を調整します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "検索可能なドキュメントのフィルタリング"
      content: |
        フィルタを使用して文書の検索を洗練する方法を学びます。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 不要なファイル形式を除外するためにインデックスを設定します
          IndexSettings settings = new IndexSettings();
          DocumentFilter fileExtensionFilter = 
            searchLib.DocumentFilter.createFileExtension(".odp", ".png", ".rtf");

          DocumentFilter invertedFilter = 
            searchLib.DocumentFilter.createNot(fileExtensionFilter);
          settings.setDocumentFilter(invertedFilter);

          Index index = new searchLib.Index("c:/MyIndex", settings);
              
          // ドキュメントを含むディレクトリを指定します
          index.add("c:/MyDocuments");

          // さらなる利用のために検索出力を処理します
          const result = index.Search("Lorem", options);
          
          // さらなる利用のために検索出力を処理します
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
            link: "/examples/search/formats/searchfilters.docx"
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
    title: "主な機能"
    exclude: "filters"
    description: "文書内で迅速かつ正確なテキスト検索を実行します。"
    items: 
          
        # operation loop 1
        - name: "条件による検索"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/docx/"
          description: "ブール条件を使用してドキュメント内の情報を見つける"

        # operation loop 2
        - name: "大文字小文字を区別した検索"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "大文字小文字を考慮することで検索の精度を向上させる"

        # operation loop 3
        - name: "ドキュメントのインデックス作成"
          operation: "document"
          link: "/search/nodejs-java/document/docx/"
          description: "ドキュメントを一度インデックス化し、複数の検索にインデックスを再利用する"

        # operation loop 4
        - name: "検索フィルター"
          operation: "filters"
          link: "/search/nodejs-java/filters/docx/"
          description: "処理するデータを絞り込むためにフィルターを使用する"

        # operation loop 5
        - name: "正確なフレーズ"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/docx/"
          description: "特定の文やフレーズを検索する"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまなドキュメント形式内での検索"
    exclude: "DOCX"
    description: "GroupDocs.Search は70以上のファイルタイプをサポートしており、さまざまなオフィスおよびビジネス文書内で効率的なテキスト検索を可能にします。"
    items: 
        # format loop 1
        - name: "DOCXの検索フィルター"
          format: "DOCX"
          link: "/search/nodejs-java/filters/docx/"
          description: "Microsoft Word Open XMLドキュメント"
          
        # format loop 2
        - name: "PDFの検索フィルター"
          format: "PDF"
          link: "/search/nodejs-java/filters/pdf/"
          description: "Adobe Portable Document Format"
          
        # format loop 3
        - name: "PPTXの検索フィルター"
          format: "PPTX"
          link: "/search/nodejs-java/filters/pptx/"
          description: "PowerPoint Open XMLプレゼンテーション"

        # format loop 4
        - name: "TXTの検索フィルター"
          format: "TXT"
          link: "/search/nodejs-java/filters/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: "XLSXの検索フィルター"
          format: "XLSX"
          link: "/search/nodejs-java/filters/xlsx/"
          description: "Microsoft Excel Open XMLスプレッドシート"
  

---