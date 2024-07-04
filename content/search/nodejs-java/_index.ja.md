---
############################# Static ############################
layout: "landing"
date: 2024-07-04T14:43:38
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
head_title: "Node.js ドキュメント、PDF、Office、Web 用のテキスト検索およびインデックス作成ライブラリ"
head_description: "PDF、Word、Excel、プレゼンテーション、電子メール、Web ファイル形式などのドキュメントからデータを検索、インデックス付け、収集するための Node.js アプリケーション向けの高度なテキスト検索ソリューション。"

############################# Header ############################
title: "Node.js API を使用したドキュメントの検索とインデックス付け"
description: "すべての一般的なドキュメント形式でテキスト検索を実装することで、Node.js アプリケーションを強化します。"
words:
  for: "のために"

actions:
  main: "NPM の無料ダウンロード"
  main_link: "https://www.npmjs.com/package/@groupdocs/groupdocs.search"
  alt: "ライセンス"
  alt_link: "https://purchase.groupdocs.com/pricing/search/nodejs-java/"
  title: "始める準備はできていますか?"
  description: "GroupDocs.Search の機能を無料で試すか、ライセンスをリクエストしてください"

release:
  title: "バージョン {0} がリリースされました"
  notes: "新機能を見る"
  downloads: "ダウンロード"
  link: "https://releases.groupdocs.com/search/nodejs-java/"

code:
  title: "JavaScript でフォルダ内を検索"
  more: "他の例"
  more_link: "https://github.com/groupdocs-search/GroupDocs.Search-for-Node.js-via-Java/"
  install: "npm i @groupdocs/groupdocs.search"
  content: |
    ```javascript {style=abap}
    // インデックスの作成
    const index = new Index('c:/MyIndex');

    // ドキュメントをインデックスに追加する
    index.add('c:/MyDocuments');
    
    // などのさまざまな単語を検索すると、
    // 'affect', 'effect', 'principles', 'principally'
    const results = index.search('?ffect & princip?(2~4)');
    ```

############################# Overview ############################
overview:
  enable: true
  title: "GroupDocs.Search の概要"
  description: "テキスト検索用の Node.js JavaScript ライブラリ"
  features:
    # feature loop
    - title: "Node.js インデックス作成と検索操作"
      content: "GroupDocs.Search for Node.js via Java のインデックス作成により、データが収集、保存、解析され、正確かつ効率的な検索操作が可能になります。これらのインデックスは、検索を実行するために頻繁に使用されます。"

    # feature loop
    - title: "複数のインデックスを結合して検索効率を向上"
      content: "GroupDocs.Search for Node.js via Java API を使用すると、複数のインデックスを 1 つに結合できます。頻繁に変更を行うと複数の差分インデックスが作成され、検索パフォーマンスが低下する可能性があります。当社のソリューションは、これらのデルタ インデックスを、マージされたデルタ インデックスからのすべての情報を含む共通インデックスにマージし、デルタ インデックスを変更せずに検索効率を大幅に向上させます。このプロセスを微調整するためにさまざまな機能を構成できます。"

    # feature loop
    - title: "さまざまなキーボード レイアウトからの検索クエリを認識する"
      content: "GroupDocs.Search for Node.js via Java は、キーボード レイアウトと一致しない検索クエリを認識します。現在、88 の言語と 164 の異なるキーボード レイアウトがサポートされています。"

    # feature loop
    - title: "形態学的単語形式を使用した検索"
      content: "GroupDocs.Search for Node.js via Java を使用すると、名詞の単数形や複数形、動詞のすべての形など、さまざまな語形を検索できます。英語および英語以外の言語は、特定の語形に合わせてカスタマイズできます。"

############################# Platforms ############################
platforms:
  enable: true
  title: "プラットフォームの独立性"
  description: "GroupDocs.Search for Node.js via Java は、すべての一般的なオペレーティング システムとパッケージ マネージャーをサポートしています。"
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
  title: "サポートされているファイル形式"
  description: |
    GroupDocs.Search for Node.js via Java を使用すると、幅広いファイル形式を処理できます。 [完全なリストを確認](https://docs.groupdocs.com/search/java/supported-document-formats/)。
  groups:
    # group loop
    - color: "green"
      content: |
        ### 一般的な Office フォーマット
        * **ポータブル:** PDF 
        * **Word:** DOC, DOCX, DOCM, DOT, DOTX, DOTM
        * **Excel:** XLS, XLSX, XLSM, XLT, XLTX, XLTM, XLSB, XLA, XLAM, CSV, TSV
        * **PowerPoint:** PPT, PPTX, POT, POTX, PPS, PPSX, PPTM, PPSM, POTM
        * **OpenDocument:** ODT, ODP, ODS, OTT, OTS
        * **文章:** TXT, RTF
    # group loop
    - color: "blue"
      content: |
        ### メディアフォーマット
        * **一般的な画像形式:** BMP, JP2, PNG, EMF, WMF, JPG, PSD
        * **複数ページの画像:** GIF, WEBP, TIFF
        * **オーディオ:** MP3, WAV
        * **ビデオ:** AVI, MOV, QT, FLV, ASF
      # group loop
    - color: "red"
      content: |
        ### 他の
        * **Eメール:**  PST, OST, MSG, EML, EMLX
        * **Microsoft Visio:** VSD, VSS
        * **ウェブ:**  XML, HTM, HTML, XHTML, MHT, MHTML
        * **その他:**  TORRENT, ZIP, DCM, DJVU, EPUB, FB2

############################# Features ############################
features:
  enable: true
  title: "GroupDocs.Search for Node.js via Java の機能"
  description: "PDF、DOCX、XLSX、PPTX などの一般的なファイル形式をサポートする高度な検索エンジンを使用してビジネス ドキュメントのコンテンツを管理します。"

  items:
    # feature loop
    - icon: "document_info"
      title: "柔軟なパラメータ"
      content: "検索パラメータとして日付範囲と大文字と小文字の区別を使用する"

    # feature loop
    - icon: "detect"
      title: "スペルチェック検索"
      content: "スペルチェックとワイルドカードを含む検索フレーズを使用し、クエリ内の特殊文字をスキップする"

    # feature loop
    - icon: "collect"
      title: "結果のフィルタリング"
      content: "検索結果でのドキュメント フィルタリングの設定"

    # feature loop
    - icon: "get"
      title: "インポート・エクスポート"
      content: "インデックス作成およびファイルへのエクスポート中にインポートを実行するかリストを使用して文字を変更する"

    # feature loop
    - icon: "remove"
      title: "不要なデータをスキップする"
      content: "特定のファイルのインデックス作成を選択的にスキップし、特定の単語をスキップしてインデックスを高速化します"

    # feature loop
    - icon: "style"
      title: "URL処理"
      content: "HTML 形式のテキストをファイルに抽出し、HTML で検索結果をナビゲートするための URL を生成します"

    # feature loop
    - icon: "detect"
      title: "迅速な検索"
      content: "検索をより小さなチャンクに分割して、大規模なインデックスを迅速に検索する"

    # feature loop
    - icon: "manipulate"
      title: "ストリーム処理"
      content: "ストリームとデータ構造からドキュメントにインデックスを付ける"

    # feature loop
    - icon: "compare"
      title: "スペルミスの処理"
      content: "見つかった各単語の正確な出現数を有効にして、スペルミスの場合に代替単語の提案を提供します"

    # feature loop
    - icon: "unreadable_characters"
      title: "アーカイブサポート"
      content: "他の ZIP アーカイブ内の ZIP アーカイブにインデックスを付け、アーカイブ内のインデックス付きファイルのリストを取得する"

    # feature loop
    - icon: "hidden_print"
      title: "ディスク容量の節約"
      content: "コンパクトなインデックス作成とパスワードで保護されたドキュメントのインデックス作成でスペースを節約"

    # feature loop
    - icon: "style"
      title: "カスタム同義語"
      content: "英語の同義語をデフォルトの同義語辞書に追加"

############################# Code samples ############################
code_samples:
  enable: true
  title: "コードサンプル"
  description: "例を使用して GroupDocs.Search for Node.js via Java の機能を探索する"
  items:
    # code sample loop
    - title: "あいまい検索を使用して生産性を向上させる"
      content: |
        柔軟な GroupDocs.Search for Node.js via Java 機能を利用して、洗練された検索アルゴリズムによってドキュメント コンテンツの制御を強化します。 [詳細](https://docs.groupdocs.com/search/java/search-results/)。
        {{< landing/code title="検索結果の処理方法">}}
        ```javascript {style=abap}
        // インデックスを作成する
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');

        // 検索オプションを設定する
        var options = new SearchOptions();
        options.getFuzzySearch().setEnabled(true);
        options.getFuzzySearch().setFuzzyAlgorithm(new TableDiscreteFunction(3));

        // 「water」という単語または「Lorem ipsum」という語句を含むドキュメントを検索する
        var query = "water OR \"Lorem ipsum\"";
        var result = index.search(query, options);
        
        // プロセス検索結果
        console.log("Documents: " + result.getDocumentCount());
        console.log("Total occurrences: " + result.getOccurrenceCount());
        for (int i = 0; i < result.getDocumentCount(); i++) {
            FoundDocument document = result.getFoundDocument(i);
            console.log('Document: ${document.getDocumentInfo().getFilePath()}');
            console.log('Occurrences: ${document.getOccurrenceCount()}');
            }

        ```
        {{< /landing/code >}}
    # code sample loop
    - title: "正規表現は高度な検索シナリオで使用できます"
      content: |
        GroupDocs.Search for Node.js via Java では、正規表現を使用して検索結果を絞り込むことができます。 [高度な検索テクニックを詳しく見る](https://docs.groupdocs.com/search/java/regular-expression-search/)。
        {{< landing/code title="正規表現を使って検索する方法">}}
        ```javascript {style=abap}   
        // インデックスを作成する
        const index = new Index('c:/IndexFolder');
        index.add('c:/DocumentFolder');
 
        // テキスト形式で語句を検索します

        // 先頭の最初のキャレット文字は、これが正規表現検索クエリであることを示します
        var query = "^^(.)\\1{1,}";
        // 単語の先頭にある 2 つ以上の同一の文字を検索します
        var result = index.search(query);
 
        ```
        {{< /landing/code >}}

---
