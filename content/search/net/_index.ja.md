---
layout: "product"
date: 2021-04-27T09:31:06+03:00
draft: false

product: "Search"
product_tag: "search"
platform: ".NET"
platform_tag: "net"

head_title: "C＃.NET Text Search＆Indexing API for Word Excel PDF Email HTML"
head_description: "PDF、Microsoft Office Word、Excel、プレゼンテーション、OneNote、Eメール、ZIP、EPUB、およびWebファイルからデータをスマートにインデックス化および取得するためのC＃.NETテキスト検索API."

title: ".ドキュメントを検索してインデックスを作成するためのNETAPI"
description: ".NETアプリケーションを使用して、すべての一般的なドキュメント形式でデータのインデックスを作成し、テキスト検索を実行するAPI."
button:
    enable: true

submenu:
    enable: true
    
    left:
        img_alt: "GroupDocs.Search for .NET"
        image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-net.png"
        product: "GroupDocs.Search"
        platform: ".NET"

    middle:
        button:
            - link: "#overview"
              text: "概要"

            - link: "#features"
              text: "特徴"

            - link: "#support"
              text: "サポート"

            - link: "https://products.groupdocs.app/search"
              text: "ライブデモ"

            - link: "https://purchase.groupdocs.com/pricing/search/net"
              text: "価格設定"

    right:
        link_download: "https://downloads.groupdocs.com/search"
        link_learn: "https://docs.groupdocs.com/search/net/"
        link_buy: "https://purchase.groupdocs.com"

overview:
    enable: true
    content: |
      GroupDocs.Search for .NETは、C＃、ASP.NET、およびその他の.NETテクノロジで開発されたビジネスアプリケーション用のドキュメントおよびテキスト検索APIです。この.NETAPIは、基本から高度な検索機能をサポートします。たとえば、複数のインデックスの作成とマージ、シンプル、ブール、ファジー、正規表現（regex）を使用したインデックスの検索、その他のクエリタイプを使用して、ファイル、ドキュメント、スマート検索による電子メール。エンドユーザー向けに高速で信頼性が高く、スマートで機能豊富な検索アプリケーションを構築し、一般的なすべてのファイル形式をサポートしたい場合は、GroupDocs.Searchfor.NETが必要です。
    tabs:
      enable: true
      
      tab_one:
        description: |
          以下は、GroupDocs.Searchfor.NETの概要です。
      
        left:
          enable: true
          icon: "fas fa-search"
          title: "インデックス作成"
          content: |
            *作成および管理
            *複数のインデックスをマージする
            *マルチスレッド非同期インデックス
            *コンパクトなインデックス作成
            *アーカイブファイルのインデックス作成
        
        right:
          enable: true
          icon: "fas fa-search-plus"
          title: "高度な検索と検索クエリ"
          content: |
            *あいまい検索
            *同義語検索
            *メール検索
            *ホモフォニック用語の処理
            *保護されたファイルの検索
            * 単純
            *ワイルドカード
            *正規表現（Regex）
            *ファセットとブール
            * 大文字と小文字を区別
      
      tab_two:
        description: |
          GroupDocs.Search for .NETは、次の[ドキュメントファイル形式]（https://docs.groupdocs.com/search/net/supported-document-formats/）をサポートしています。

        left:
          enable: true
          table:
            - title: "MicrosoftOfficeの形式"
              content: |
                * ** Word **：DOC、DOCX、DOCM、DOT、DOTX、DOTM
                * ** Excel **：XLS、XLSX、XLSM、XLT、XLTX、XLTM、XLSB、XLA、XLAM、CSV、TSV
                * ** PowerPoint **：PPT、PPTX、POT、POTX、PPS、PPSX、PPTM、PPSM、POTM
                * **プロジェクト**：MPP
                * **図**：VSD、VSS
                * ** Microsoft Compiled HTML **：CHM
                * ** OneNote **：ONE

        right:
          enable: true
          table:
            - title: "OpenDocumentおよびその他の形式"
              content: |
                * **ポータブルドキュメントフォーマット**：PDF
                * ** OpenDocument **：ODT、OTT、ODS、OTS、ODP
                * **メール**：PST、OST、MSG、EML、EMLX
                * ** Webファイル形式**：XML、HTM、HTML、XHTML、MHT、MHTML
                * **オーディオ**：MP3、WAV
                * **ビデオ**：AVI、MOV、QT、FLV、ASF
                * **テキスト**：TXT
                * **リッチテキスト形式**：RTF
                * ** Markdownドキュメントファイル**：MD
                * **画像**：BMP、GIF、JP2、PNG、WEBP、TIFF、EMF、WMF、JPG、PSD
                * **その他**：TORRENT、ZIP、DCM、DJVU、EPUB、FB2

      tab_three:
        description: |
          GroupDocs.Search for .NETは、次のオペレーティングシステム、フレームワーク、およびパッケージマネージャーをサポートしています。
        
        left:
          enable: true
          table:
            - icon: "fab fa-windows"
              title: "オペレーティングシステム"
              content: |
                *Windowsデスクトップ
                * WindowsServer
                * Windows Azure
                * Linux

            - icon: "fas fa-code"
              title: "サポートされているフレームワーク"
              content: |
                * .NETFramework2.0以降
                * MonoFramework1.2以降
                * .NET Standard 2.0
                * .NET Core 2.0
                * .NET Core 2.1

        right:
          enable: true
          table:
            - icon: "fas fa-box"
              title: "パッケージマネージャー"
              content: |
                * NuGet

            - icon: "fas fa-tools"
              title: "開発環境"
              content: |
                * Microsoft Visual Studio
                * Xamarin.Android
                * Xamarin.IOS
                * Xamarin.Mac
                * MonoDevelop

features:
    enable: true
    title: "GroupDocs.Search for .NET Features"

    feature:
      - icon: "fas fa-copy"
        content: "メモリまたはディスクにインデックスを作成し、マルチスレッドのインデックス作成とマージを実行します"

      - icon: "fas fa-eye"
        content: "すでにインデックスが作成されているファイル、または名前に特定の文字列が含まれているファイルのインデックス作成を防止する"

      - icon: "fas fa-bolt"
        content: "インデックスの作成と更新の進捗率を表示し、検索レポートを取得する"
      
      - icon: "fas fa-file-powerpoint"
        content: "最近処理されたファイルの特定の単語とインデックスステータス通知を除外することによるインデックス作成の高速化"

      - icon: "fas fa-code"
        content: "ZIPアーカイブ内のZIPアーカイブにインデックスを付け、アーカイブに含まれるインデックスファイルのリストを取得する"

      - icon: "fas fa-cloud"
        content: "リストまたはインポートを使用して、インデックス作成中に文字を置き換え、ファイルにエクスポートします"

      - icon: "fas fa-remove-format"
        content: "パスワードで保護されたファイルのインデックス作成と検索、ディスクスペースを節約するためのコンパクトなインデックス作成"

      - icon: "fas fa-comment-slash"
        content: "インデックスまたはソースファイルからテキストを抽出し、テキストファイルのエンコーディングをインデックスに自動的に保存する"

      - icon: "fas fa-location-arrow"
        content: "インデックス作成中に各ドキュメントに任意の追加フィールドを追加する"

      - icon: "fas fa-border-all"
        content: "検索結果でドキュメントフィルタリングを設定する"

      - icon: "fas fa-wrench"
        content: "あいまい検索で入力ミスを処理し、あいまい検索で類似性レベルを設定し、最良の結果のみを表示する"

      - icon: "fas fa-columns"
        content: "ストリームとデータ構造からのインデックスドキュメント"

      - icon: "fas fa-file-word"
        content: "ストップワードを使用して完全なフレーズを検索し、ファセット検索とブール検索を組み合わせます"

      - icon: "fas fa-envelope"
        content: "ホモフォニック用語、同義語、日付範囲、ワイルドカード、大文字と小文字の区別に基づいて検索"

      - icon: "fas fa-print"
        content: "Outlookからの電子メールのインデックス作成と検索、およびAspose.EmailAPIを使用した参照"

      - icon: "fas fa-file-archive"
        content: "検索クエリでスペルチェックとワイルドカードをサポートし、検索フレーズで特殊文字をスキップします"

      - icon: "fas fa-lock"
        content: "検索クエリの各用語とすべての結果の結果を制限する"

      - icon: "fas fa-file-code"
        content: "HTMLテキストをファイルに抽出してURLを生成し、HTML形式の検索結果をナビゲートします"
      
      - icon: "fas fa-fill-drip"
        content: "複数のクエリを1つのオブジェクトツリーに結合する"

      - icon: "fas fa-file-excel"
        content: "インデックス作成エラーが発生した場合に、サポートされていない設定と自動インデックスの再読み込みについてユーザーに警告する"

      - icon: "fas fa-heading"
        content: "見つかった単語ごとに正確な出現回数を有効にして、スペルミスの場合に代替単語の提案を提供します"

      - icon: "fas fa-project-diagram"
        content: "インデックスを再作成せずに、インデックス付きドキュメントにテキスト属性を追加する"

      - icon: "fas fa-cube"
        content: "文字に基づいて索引付けおよび検索操作を実行する"

      - icon: "fab fa-uncharted"
        content: "非テキストドキュメント形式のインデックスメタデータ"

    more_feature:
      - title: "インデックス作成と検索"
        content: |
          GroupDocs.Search for .NET APIは、検索を実行するためにインデックスを頻繁に使用します。インデックスは、高速で正確な検索のためにデータを収集、解析、または保存するために使用されます。

          * **インデックスの作成**：インデックスフォルダを作成し、そのフォルダにドキュメントを追加/インデックス付けします。
          * **ロードインデックス**：既存のインデックスをロードします。
          * **ドキュメントをインデックスに追加**：ドキュメントを既存のインデックスに非同期で追加します。
          * **インデックスの更新**：ドキュメントが変更、追加、または削除されるたびに、既存のインデックスを更新します。これにより、検索結果が最新の状態に保たれます。

          ```cs
           //インデックスを作成します
          Index  index = new Index(@"c:\MyIndex");
          //ドキュメントをインデックスに追加します
          index.AddToIndex(@"c:\MyDocuments");
          //インデックスで検索
          SearchResults searchResults =  index.Search("searchTerm");
          ```
      - title: "複数のインデックスをマージして検索効率を向上させる"
        content: "GroupDocs.Search for .NETは、複数のインデックスを単一のインデックスにマージできます。インデックスが頻繁に更新される場合、いくつかのデルタインデックスがありますが、このアプローチでは検索パフォーマンスが低下します。 GroupDocs.Search for .NET APIは、すべてのデルタインデックスを1つの統合インデックスにマージします。プライマリマージされたインデックスには、マージされたデルタインデックスからのすべての情報が含まれます。ただし、デルタインデックスは変更されません。 APIで使用されるこのアプローチにより、検索効率が大幅に向上します。インデックスマージ機能は、このプロセスをさらに微調整するために微調整するための多数の機能を提供します。"

      - title: "HTMLマークアップを生成するために、テキストをインデックスに保存します"
        content: "GroupDocs.Search for .NETは、インデックス付きドキュメントのテキストをインデックスにキャッシュできます。このキャッシュされたテキストは、検索結果を強調表示することにより、HTMLマークアップを迅速に生成するために使用されます。このアプローチは、ファイルから直接テキストを抽出するよりもはるかに高速です。ソースファイルが使用できなくなった場合でも、キャッシュからテキストを取得できます。キャッシュされたテキストは、さまざまな圧縮レベルを適用して、占有するディスクスペースを減らし、インデックス作成時間を短縮することで保存できます。."

      - title: "Fuzzy＆RegexSearchで関連ドキュメントを取得する"
        content: "ファジー検索または正規表現検索を実行すると、提供された入力に完全に一致するドキュメントのリストを取得できます。ただし、入力に類似した単語または用語を含むドキュメントのリストも表示されます。たとえば、GroupDocs.Search for .NETを使用して、クエリ「cost」のあいまい検索を実行すると、「cost」という単語を含むドキュメントと「coat」などの類似した単語を含むドキュメントが取得されます。結果は、このAPIを使用して構成したあいまいさのレベルによって異なります。."

      - title: "さまざまなキーボードレイアウトの検索クエリを認識する"
        content: "GroupDocs.Search for .Netは、キーボードレイアウトと一致しない言語で書かれた検索クエリを認識できます。現在、この.NET APIは、88の言語と164の異なるキーボードレイアウトを正常に認識できます。."

      - title: "形態論的単語形式を使用した検索"
        content: "GroupDocs.Search for .NET APIを使用すると、さまざまな単語形式を検索できます。たとえば、名詞の場合、その単数形と複数形を検索できます。動詞の場合、その動詞のすべての形式を検索できます。また、ルート、三人称単数、単純過去形、その他のさまざまな形を検索することもできます。英語以外の言語の場合、カスタマイズされた単語形式を実装できます."

support:
    enable: true

solutions:
    enable: true
    title: "GroupDocs.Searchは、他の一般的な開発環境向けのドキュメント表示APIを提供します"

    solution:
        - img_alt: "GroupDocs.Search for Java"
          image: "https://www.groupdocs.cloud/templates/groupdocs/images/product-logos/groupdocs-search-java.png"
          product: "GroupDocs.Search"
          platform: "Java"
          link: "/search/java/"

back_to_top:
  enable: true
---
