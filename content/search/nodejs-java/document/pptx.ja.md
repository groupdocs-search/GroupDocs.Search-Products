
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:35
draft: false
lang: ja
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PPTX内のテキストをGroupDocs.Searchを使用してNode.jsで検索"
head_description: "JavaScriptを使用して、さまざまな文書形式で効率的にテキストを検索するためにGroupDocs.Search for Node.js via Javaを利用しましょう。"

############################# Header ############################
title: "スマート文書検索ソリューション" 
description: "GroupDocs.Search for Node.js via Javaを使用して、さまざまな文書形式でテキストを正確に特定します。Node.jsアプリケーション内で高度な検索クエリを作成できます。"
subtitle: "GroupDocs.Search for Node.js via Java" 

header_actions:
  enable: true
  items:
    #  loop
    - title: "無料で試す"
      link: "https://releases.groupdocs.com/search/nodejs-java/"
      
############################# About ############################
about:
    enable: true
    title: "GroupDocs.Searchの紹介"
    link: "/search/nodejs-java/"
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/)は、フルテキスト検索と文書インデックス作成のための高性能ライブラリです。PDF、Word、PowerPoint、Excel、画像、ZIPアーカイブを含む70以上のファイルタイプをサポートし、高速かつ正確な結果が得られます。

############################# Steps ############################
steps:
    enable: true
    title: "PPTXファイルで検索を実行"
    content: |
      [GroupDocs.Search](/search/nodejs-java/)を使用すると、PPTXファイル内での検索を実行し、Node.js via Javaアプリケーション内で結果を絞り込むことができます。
      
      1. 検索インデックスのためのストレージフォルダを定義します。
      2. PPTXファイルを含むフォルダを選択します。
      3. 追加の検索パラメータを設定します。
      4. 検索を実行し、結果を分析します。
   
    code:
      platform: "nodejs-java"
      copy_title: "コピー"
      result_enable: true
      result_link: "/examples/search/search_all.pdf"
      result_title: "{common-content.format-code.result_title}"
      install:
        command: "npm i @groupdocs/groupdocs.search"
        copy_tip: "クリックしてコピー"
        copy_done: "コピーしました"
      links:
        #  loop
        - title: "さらに例を見る"
          link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
        #  loop
        - title: "ドキュメンテーション"
          link: "https://docs.groupdocs.com/search/nodejs-java/"
          
      content: |
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search')

        // 検索インデックスストレージのディレクトリを指定
        const index = new searchLib.Index("c:/MyIndex");

        // 検索対象の文書を含むフォルダーを選択
        index.add("c:/MyDocuments");

        // 類似の音を持つ単語のために同音検索を有効化
        const options = new searchLib.SearchOptions();
        options.setUseHomophoneSearch(true);

        // 複雑な検索クエリを実行
        const result = index.search("metis", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "高度な検索およびインデックス作成機能"
  description: "GroupDocs.Search for Node.js via Javaは70以上の文書形式にわたる強力なテキスト検索およびインデックス作成ツールを提供し、情報の検索と整理を容易にします。"
  image: "/img/search/features_document.webp" # 500x500 px
  image_description: "GroupDocs.Searchの主な利点"
  features:
    # feature loop
    - title: "包括的なテキスト検索"
      content: "PDF、Word文書、PowerPointプレゼンテーション、スプレッドシートなど複数の文書タイプ内でテキストを特定します。正確な一致、ファジー検索、ワイルドカードを使用して結果を絞り込みます。"

    # feature loop
    - title: "大規模データの効率的なインデックス作成"
      content: "構造化インデックスを作成することで検索を高速化し、大量の文書コレクションから情報を簡単に取得できるようにします。"

    # feature loop
    - title: "80以上の言語をサポート"
      content: "さまざまな言語の文書内で検索を行い、さまざまな単語の形やキーボードレイアウトを自動的に認識します。"

    # feature loop
    - title: "カスタム検索設定"
      content: "大文字・小文字の区別、日付フィルタ、単語の除外などの検索オプションを調整することで、正確な結果を得られます。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "PPTX文書での検索の使用"
      content: |
        この例は、PPTX文書内での検索クエリの使用方法を示しています。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 検索インデックスのためのディレクトリを設定
          const index = new searchLib.Index("c:/MyIndex");
              
          // 文書ストレージのファイルパスを提供
          index.add("c:/MyDocuments");

          // 保護されたファイルのパスワードを入力
          index.getDictionaries().getDocumentPasswords().add("protected.pptx", '123456');

          // 類似語検出のためにファジー検索を有効化
          const options = new searchLib.SearchOptions();
          options.getFuzzySearch().setEnabled(true);
          options.getFuzzySearch().setFuzzyAlgorithm(new searchLib.SimilarityLevel(0.8));

          // 検索結果を抽出
          const result = index.search("Loarem", options);
          
          // 結果を処理してレビューします
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
          - title: "{common-content.format-code.result_title_bottom}"
            icon: "download"
            link: "/examples/search/formats/searchdocument.pptx"
        links:
          #  loop
          - title: "さらに例を見る"
            link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
          #  loop
          - title: "ドキュメンテーション"
            link: "https://docs.groupdocs.com/search/nodejs-java/"
            

            


############################# Actions ############################

actions:
  enable: true
  title: "始める準備はできましたか？"
  description: "GroupDocs.Searchの機能を無料で試すか、ライセンスをリクエストしてください"
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
    title: "主要機能を探索"
    exclude: "document"
    description: "効率と精度を向上させるために設計された高速検索機能を発見します。"
    items: 
          
        # operation loop 1
        - name: "{common-content.operations.boolean.name}"
          operation: "boolean"
          link: "/search/nodejs-java/boolean/pptx/"
          description: "{common-content.operations.boolean.description}"

        # operation loop 2
        - name: "{common-content.operations.case-sensitive.name}"
          operation: "case-sensitive"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "{common-content.operations.case-sensitive.description}"

        # operation loop 3
        - name: "{common-content.operations.document.name}"
          operation: "document"
          link: "/search/nodejs-java/document/pptx/"
          description: "{common-content.operations.document.description}"

        # operation loop 4
        - name: "{common-content.operations.filters.name}"
          operation: "filters"
          link: "/search/nodejs-java/filters/pptx/"
          description: "{common-content.operations.filters.description}"

        # operation loop 5
        - name: "{common-content.operations.phrase.name}"
          operation: "phrase"
          link: "/search/nodejs-java/phrase/pptx/"
          description: "{common-content.operations.phrase.description}"
          
        
          
############################# More Formats ########################
more_formats:
    enable: true
    title: "さまざまな文書で検索"
    exclude: "PPTX"
    description: "GroupDocs.Searchは70以上のファイル形式で動作し、オフィス文書を含み、インデックス作成サポートにより迅速かつ正確な検索を実現します。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/document/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/document/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/document/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/document/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/document/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---