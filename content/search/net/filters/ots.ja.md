---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/net/filters/ots/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB FB2 

############################# Head ############################
head_title: ".NET アプリでドキュメント フィルタリングを設定して検索結果をカスタマイズする"
head_description: "GroupDocs.Search .NET API を使用すると、ソフトウェア開発者は OTS Documents ドキュメントを検索し、.NET アプリでドキュメント フィルタリングを適用して検索結果をカスタマイズできます。"

############################# Header ############################
title: "ドキュメント フィルタリングを設定して、.NET アプリ内の検索結果をカスタマイズする"
description: "GroupDocs.Search .NET API は、ソフトウェア専門家がドキュメント検索機能を追加し、.NET アプリ内でドキュメント フィルタリングを適用して検索結果をカスタマイズするのに役立ちます。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NET 経由で検索結果にドキュメント フィルタリングを適用する方法は?"
    content: |
       フィルタリングは、ユーザーが機能を検査および処理できるようにする非常に便利な手法です。 ドキュメント フィルタリングを使用すると、ユーザーは簡単に結果をナビゲートし、探しているものを見つけることができます。 また、検索を特定のセクションまたは特定のドキュメント タイプに制限する権限もユーザーに与えます。 GroupDocs.Search for .NET は、機能豊富な高性能ドキュメント検索 API であり、ソフトウェア開発者がテキスト検索とインデックス作成を実現できるアプリケーションを構築できるようにします。 PDF、HTML、Outlook 電子メール、Microsoft Office Word、Excel ワークシート、PowerPoint プレゼンテーション、Outlook MSG、PST など、最も一般的なドキュメント形式をサポートしています。 API は、検索結果のドキュメント ファイリングの設定を完全にサポートします。 ファイル パス フィルター、ファイル拡張子フィルター、属性フィルターなど、いくつかの種類のファイラーを使用して検索結果をカスタマイズできます。 ブール演算子 AND、OR & NOT などを使用して検索ドキュメント フィルターを組み合わせることもできます。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NET 経由で OTS ドキュメントを検索する際にドキュメント フィルタを設定する"
      content_left: |
       GroupDocs.Search .NET API は、ソフトウェア開発者が .NET アプリケーション内に検索機能を追加するのに役立ちます。 次の .NET コード例は、わずか数行のコードでさまざまな種類のドキュメントを検索する際にドキュメント フィルターを適用する方法を示しています。

      title_right: "OTS ドキュメントの検索にドキュメント フィルタを適用"
      content_right: |
       * 最初に、インデックス フォルダーとドキュメント フォルダーへのパスを指定する必要があります。
       * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) クラスのインスタンスを呼び出して、指定したフォルダにインデックスを作成する
       * [Search](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) メソッドを呼び出して、指定したフォルダーからドキュメントのインデックスを作成する
       * 検索オプション オブジェクトの作成 [SearchOptions](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions)
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) を呼び出してドキュメント フィルターを設定します。
       * 検索を開始し、検索結果を表示する
        
      gisthash: "77cafabe4e9c9256217b4326e26a59d0"
      gistfile: "set_document_filter_in_search_dotnet.cs"

    - title_left: ".NET 経由で検索ドキュメント フィルターを組み合わせる方法"
      content_left: |
        GroupDocs.Search for .NET を使用すると、ソフトウェア プログラマは、検索中に検索ドキュメント フィルタを組み合わせて、C# .NET アプリケーション内の検索の結果として返されるドキュメントを制御できます。 次の .NET コード例は、C# アプリケーション内でブール演算子 AND、OR、NOT などを使用して検索ドキュメント フィルターを組み合わせる方法を示しています。 

      title_right: "OTS ファイルの検索で文書検索フィルターを組み合わせる"
      content_right: |
       * 最初に、インデックス フォルダーとドキュメント フォルダーへのパスを指定する必要があります。
       * 絶対パスに「Einstein」という単語が含まれるすべての FB2 および EPUB ドキュメントを返す AND 複合フィルタを作成する
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) を呼び出して、filter1 を作成します。
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) を呼び出して、filter2 を作成します。
       * [andFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createand) メソッドを呼び出してフィルターを組み合わせる
       * すべての DOC、DOCX、PDF、および完全パスに Einstein という単語が含まれるすべてのドキュメントを返す OR 複合フィルターの作成
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) を呼び出して、filter3 を作成します。
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) を呼び出して filter4 を作成します。
       * [orFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createor) メソッドを呼び出してフィルターを組み合わせる
       * TXT ドキュメントを除く、見つかったすべてのドキュメントを返すフィルターの作成
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchoptions/properties/searchdocumentfilter) を呼び出して filter4 を作成します。
       * [notFilter](https://apireference.groupdocs.com/search/net/groupdocs.search.options/searchdocumentfilter/methods/createnot) メソッドを呼び出して Not フィルターを適用する

      gisthash: "db4efe513cbd34925231be10a992f23c"
      gistfile: "combine_document_filter_in_search_dotnet.cs"
      
    - title_left: "システム要求"
      content_left: |
        GroupDocs.Search for .NETは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 完全なシステム要件ガイドについては、以下のコードを実行する前に[システム要件](https://docs.groupdocs.com/search/net/system-requirements/) にアクセスしてください。次の前提条件がインストールされていることを確認してください。 システム：
          *オペレーティングシステム：Microsoft Windows、Linux、MacOS
          *開発環境：Visual Studio、Xamarin、MonoDevelopなど
          *フレームワーク：.NETフレームワーク、.NET標準、.NETコア、モノラル
          * [NuGet](https://www.nuget.org/packages/GroupDocs.search/) から最新バージョンのGroupDocs.Search for.NETAPIを入手してください。
        
      title_right: "GroupDocs.Search を使用する理由"
      content_right: |
        * メモリ内およびディスク上での検索インデックスの作成。
        * ファイル、ストリーム、または構造からインデックスを作成する機能。
        * パスワードで保護されたドキュメントのインデックス作成のサポート。
        * 複数のインデックスのマージのサポート。
        * 検索のインデックス作成中にドキュメントをフィルタリングします。
        * 検索中のスペルチェックのサポート。
        * ブレンドされた文字は完全にサポートされています
        * さまざまな種類の検索を1つの検索クエリに結合します。
        * 単純な単語と正規表現の検索がサポートされています
        * 検索クエリでのエイリアス置換を完全にサポートします。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---