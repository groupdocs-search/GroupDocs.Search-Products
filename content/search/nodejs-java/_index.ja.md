---
############################# Static ############################
layout: "landing"
date: 2025-01-09T15:38:59
draft: false

lang: ja
product: "Search"
product_tag: "search"
platform: "Node.js via Java"
platform_tag: "nodejs-java"

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
head_title: "Node.js ドキュメント、PDF、Office、ウェブのテキスト検索およびインデックス作成ライブラリ"
head_description: "Node.jsアプリケーション向けの高度なテキスト検索ソリューション。ドキュメント（PDF、Word、Excel、プレゼンテーション、メール、ウェブファイル形式）からデータを検索、インデックス化、および収集できます。"

############################# Header ############################
title: "Node.js APIを使用してドキュメントを検索およびインデックス作成"
description: "すべての一般的なドキュメント形式でテキスト検索を実装することにより、Node.jsアプリケーションを強化します。"
words:
  for: "のための"

actions:
  main: "無料のNPMダウンロード"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "ライセンス管理"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "今日から旅を始めましょう！"
  description: "GroupDocs.Searchの機能を無料で探索するか、ライセンスを取得してその可能性を最大限に活かしてください。"

release:
  title: "バージョン {0} リリース"
  notes: "新着情報を確認する"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "JavaScriptを使用してフォルダー内でテキスト検索を実行"
  more: "その他の例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    const searchLib = require('@groupdocs/groupdocs.search');

    // ドキュメント用のインデックスを作成
    const index = new searchLib.Index('c:/MyIndex');

    // 効率的な検索のためにインデックスに文書を追加
    index.add('c:/MyDocuments');
    
    // 特定の単語やフレーズを検索。例:
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search 概要"
  description: "Node.js JavaScriptライブラリによるテキスト検索"
  features:
    # feature loop
    - title: "Node.jsにおけるインデックス作成と検索操作"
      content: "GroupDocs.Search for Node.js via Javaのインデックス作成では、データを収集、保存し、正確で効率的な検索操作のために解析します。これらのインデックスは、検索を実行するためによく使用されます。"

    # feature loop
    - title: "検索効率を向上させるために複数のインデックスを結合"
      content: "GroupDocs.Search for Node.js via Java APIは、複数のインデックスを1つに結合することを可能にします。頻繁な変更により、複数のデルタインデックスが作成され、検索パフォーマンスが低下する可能性があります。当社のソリューションでは、これらのデルタインデックスを共通インデックスに結合し、すべての情報を一元管理し、その結果、検索効率が大幅に向上します。"

    # feature loop
    - title: "異なるキーボードレイアウトからの検索クエリを認識"
      content: "GroupDocs.Search for Node.js via Javaは、キーボードレイアウトと一致しない検索クエリを認識します。現在、88の言語と164の異なるキーボードレイアウトに対応しています。"

    # feature loop
    - title: "形態素単語での検索が可能"
      content: "GroupDocs.Search for Node.js via Javaを使用すれば、単数形と複数形の名詞や動詞全般といったさまざまな単語の形を検索できます。英語や他の言語に特化したカスタマイズが可能です。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Search for Node.js via Javaはすべての一般的なオペレーティングシステムおよびパッケージマネージャーをサポートしています。"
  items:
    # platform loop
    - title: "Windows"
      image: "windows"
    # platform loop
    - title: "macOS"
      image: "finder"      
    # platform loop
    - title: "Linux"
      image: "linux"
    # platform loop
    - title: "NPM"
      image: "npm"  
    # platform loop
    - title: "NuGet"
      image: "nuget"      
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
    - title: "Eclipse"
      image: "eclipse"
    # platform loop
    - title: "IntelliJ"
      image: "intellij"

############################# File formats ############################
formats:
  enable: true
  title: "サポートされるファイル形式"
  description: |
    GroupDocs.Search for Node.js via Javaを使用して幅広いファイル形式を処理します。[完全なリストを探る](https://docs.groupdocs.com/search/nodejs-java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### 一般的なオフィス形式
        * **ポータブル:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **テキスト:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### メディア形式
        * **一般的な画像形式:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **マルチページ画像:** GIF, WEBP, TIFF
        * **オーディオ:** MP3, WAV
        * **ビデオ:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### その他
        * **メール:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **ウェブ:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **その他:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Javaの機能"
  description: "PDF、DOCX、XLSX、PPTXなどの一般的なファイル形式をサポートする高度な検索エンジンを使用して、ビジネスドキュメントの内容を管理します。"

  items:
    # feature loop
    - icon: "document_info"
      title: "柔軟なパラメータ"
      content: "日付範囲および大文字小文字の区別を検索パラメータとして使用します。"

    # feature loop
    - icon: "detect"
      title: "スペルチェック検索"
      content: "スペルチェックとワイルドカードを使用し、クエリで特殊文字をスキップします。"

    # feature loop
    - icon: "collect"
      title: "結果のフィルタリング"
      content: "検索結果において文書の種類を設定します。"

    # feature loop
    - icon: "get"
      title: "インポートおよびエクスポート"
      content: "インポートを実行したり、インデックス化中に文字を修正するためのリストを使用してファイルにエクスポートします。"

    # feature loop
    - icon: "remove"
      title: "不必要なデータをスキップ"
      content: "特定のファイルに対してインデックス化を選択的にスキップし、特定の単語をスキップして迅速にインデックス化します。"

    # feature loop
    - icon: "style"
      title: "URL処理"
      content: "HTML形式のテキストをファイルに抽出し、検索結果をHTMLでナビゲートするためのURLを生成します。"

    # feature loop
    - icon: "detect"
      title: "迅速検索"
      content: "検索を小さなチャンクに分割して、大きなインデックスを迅速に検索します。"

    # feature loop
    - icon: "manipulate"
      title: "ストリーム処理"
      content: "ストリームおよびデータ構造から文書をインデックス化します。"

    # feature loop
    - icon: "compare"
      title: "誤字を扱う"
      content: "発見した各単語の出現回数を正確に提示し、誤字の場合に代替単語の提案を行います。"

    # feature loop
    - icon: "unreadable_characters"
      title: "アーカイブのサポート"
      content: "他のZIPアーカイブ内の圧縮アーカイブをインデックス化し、アーカイブ内のインデックスされたファイルのリストを取得します。"

    # feature loop
    - icon: "hidden_print"
      title: "ディスクスペースの節約"
      content: "コンパクトなインデックスでスペースを節約し、パスワード保護された文書のインデックスを作成します。"

    # feature loop
    - icon: "style"
      title: "カスタム同義語"
      content: "デフォルトの同義語辞書に英語の同義語を追加します。"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "GroupDocs.Search for Node.js via Javaの機能例を探検してください。"
  items:
    # code sample loop
    - title: "'ファジー'検索を使用して生産性を向上"
      content: |
        洗練された検索アルゴリズムによって文書のコンテンツ管理を向上させる柔軟なGroupDocs.Search for Node.js via Javaの機能を楽しみます。[さらに詳しく](https://docs.groupdocs.com/search/nodejs-java/search-results/)。
        {{< landing/code title="検索結果を処理する方法">}}
        ```javascript {style=abap}
        const searchLib = require('@groupdocs/groupdocs.search');

        // インデックスを作成
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // 検索オプションを設定
        const options = new searchLib.SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 'water'という単語または'Lorem ipsum'というフレーズを含むドキュメントを検索
        const query = 'water OR "Lorem ipsum"';
        const result = index.search(query, options);
        
        // 検索結果を処理
        console.log('Documents: ' + result.getDocumentCount());
        console.log('Total occurrences: ' + result.getOccurrenceCount());
        for (let i = 0; i < result.getDocumentCount(); i++) {
            const document = result.getFoundDocument(i);
            console.log('Document: ' + document.getDocumentInfo().getFilePath());
            console.log('Occurrences:  + document.getOccurrenceCount());
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "正規表現が高度な検索シナリオに役立つ"
      content: |
        GroupDocs.Search for Node.js via Javaによって正規表現を使用でき、検索結果を狭めます。[高度な検索テクニックに飛び込む](https://docs.groupdocs.com/search/nodejs-java/regular-expression-search/)。
        {{< landing/code title="正規表現を使用して検索を行う方法">}}
        ```javascript {style=abap}   
        const searchLib = require('@groupdocs/groupdocs.search');

        // インデックスを作成
        const index = new searchLib.Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // テキスト形式でフレーズを検索

        // 最初のキャレット文字が先頭で、このクエリが正規表現検索であることを示します。
        const query = '^^(.)\\1{1,}';
        // 単語の先頭に同じ文字が2つ以上存在するか検索
        const result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
