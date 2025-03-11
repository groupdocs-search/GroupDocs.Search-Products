
---
############################# Static ############################
layout: "format"
date:  2025-03-11T15:59:33
draft: false
lang: ja
format: Pptx
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

############################# Head ############################
head_title: "PPTX における大文字と小文字を区別した検索を Node.js で実行する"
head_description: "GroupDocs.Search for Node.js via Java API は、JavaScript 開発者が異なるドキュメントタイプで大文字と小文字を区別した検索を実行できるようにします。"

############################# Header ############################
title: "大文字と小文字を区別した検索" 
description: "GroupDocs.Search for Node.js via Java を使用すると、Node.js アプリケーションにおいて高度な大文字と小文字を区別した検索機能を実装できます。"
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
    link_title: "詳細を見る"
    picture: "about_search.svg" # 480 X 400
    content: |
       [GroupDocs.Search for Node.js via Java](/search/nodejs-java/) は、ドキュメント内のテキストを検索およびインデックス作成するための強力なライブラリです。PDF、Word、Excel、PowerPoint、画像、ZIPファイルなど、70以上のフォーマットをサポートし、大量のデータを効率的に処理できます。

############################# Steps ############################
steps:
    enable: true
    title: "PPTX ファイルでの大文字と小文字を区別した検索の手順"
    content: |
      [GroupDocs.Search](/search/nodejs-java/) を使用すれば、PPTX ファイルで大文字と小文字を区別した検索を実行し、Node.js via Java のワークフローを強化します。
      
      1. 検索インデックスを保存するフォルダーをセットアップします。
      2. PPTX ファイルが含まれるフォルダーを選択します。
      3. 検索を実行して結果を取得します。
      4. 結果を処理して使用します。
   
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

        // インデックスフォルダーのパスを指定します
        const index = new searchLib.Index("c:/MyIndex");

        // 検索するドキュメントが含まれるフォルダーを設定します
        index.add("c:/MyDocuments");

        // 設定で大文字と小文字を区別した検索を有効にします
        const options = new groupdocs.search.SearchOptions();
        options.setUseCaseSensitiveSearch(true);

        // 検索を実行します
        const result = index.search("Lorem", options);
        ```            

############################# More features ############################
more_features:
  enable: true
  title: "文書検索とインデックス作成の主な機能"
  description: "GroupDocs.Search for Node.js via Java を使用すれば、70以上のファイルフォーマットでテキストを簡単に検索およびインデックス作成できます。高度な検索ツールを使用して情報を手軽にアクセス・整理できます。"
  image: "/img/search/features_case-sensitive.webp" # 500x500 px
  image_description: "GroupDocs.Search のコア機能"
  features:
    # feature loop
    - title: "包括的なテキスト検索"
      content: "PDF、Wordファイル、スプレッドシート、プレゼンテーションなど、さまざまなドキュメントタイプでテキストを見つけます。正確な結果を得るために、完全一致、曖昧検索、ワイルドカードなどのオプションを使用します。"

    # feature loop
    - title: "効率的なデータインデックス作成"
      content: "検索を迅速化するためにインデックスを作成および管理します。インデックス作成により、大規模なドキュメントコレクション内のデータを整理し、すばやく見つけることができます。"

    # feature loop
    - title: "複数言語のサポート"
      content: "80以上の言語でドキュメントを検索でき、多様なキーボードレイアウトや単語の変形に対応しており、正確な検索結果を保証します。"

    # feature loop
    - title: "カスタマイズ可能な検索設定"
      content: "大文字と小文字を区別する設定、日付フィルター、インデックス作成中に特定の用語やデータを除外します。"
      
  code_samples_ext:
    # code sample ext loop
    - title: "例：大文字と小文字を区別した検索の実装"
      content: |
        この例では、PPTX ドキュメントの大文字と小文字を区別した検索を実行する方法を示します。
      code:
        title: "JavaScript"
        content: |
          ```javascript {style=abap}
          const searchLib = require('@groupdocs/groupdocs.search')
          
          // 検索インデックスのフォルダーを定義します
          const index = new searchLib.Index("c:/MyIndex");
              
          // ドキュメントフォルダーへのパスを提供します
          index.add("c:/MyDocuments");

          // 検索クエリをセットアップします
          const wordQuery = searchLib.SearchQuery.createWordQuery("Lorem");

          // 大文字と小文字を区別した検索設定を有効にします
          const options = new groupdocs.search.SearchOptions();
          options.setUseCaseSensitiveSearch(true);

          // ドキュメント内のテキストを検索します
          const result = index.search(wordQuery, options);
          
          // 結果を処理および扱います
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
            link: "/examples/search/formats/searchcase-sensitive.pptx"
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
    title: "主要機能"
    exclude: "case-sensitive"
    description: "高速かつ正確なドキュメント検索のための高度な機能を探索します。"
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
    title: "対応ドキュメントフォーマット"
    exclude: "PPTX"
    description: "GroupDocs.Search は70以上のドキュメントフォーマットをサポートしています。検索オプションをカスタマイズし、インデックス作成で時間を節約できます。"
    items: 
        # format loop 1
        - name: ""
          format: "DOCX"
          link: "/search/nodejs-java/case-sensitive/docx/"
          description: "Microsoft Word オープンXMLドキュメント"
          
        # format loop 2
        - name: ""
          format: "PDF"
          link: "/search/nodejs-java/case-sensitive/pdf/"
          description: "Adobeポータブルドキュメント形式"
          
        # format loop 3
        - name: ""
          format: "PPTX"
          link: "/search/nodejs-java/case-sensitive/pptx/"
          description: "PowerPointオープンXMLプレゼンテーション"

        # format loop 4
        - name: ""
          format: "TXT"
          link: "/search/nodejs-java/case-sensitive/txt/"
          description: "テキストドキュメント"
          
        # format loop 5
        - name: ""
          format: "XLSX"
          link: "/search/nodejs-java/case-sensitive/xlsx/"
          description: "Microsoft ExcelオープンXMLスプレッドシート"
  

---