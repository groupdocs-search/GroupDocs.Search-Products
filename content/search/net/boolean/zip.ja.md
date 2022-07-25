---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/net/boolean/zip/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: ".NETを介した検索クエリにブール検索演算子(AND、OR、NOT)を追加する"
head_description: "GroupDocs.Search .NET APIを使用すると、ソフトウェア開発者は、.NETアプリ内ではなく、ブール演算子AND、ORを使用して、ブール検索を追加したり、新しいクエリを開発したりできます。."

############################# Header ############################
title: ".NETアプリではなく、ブール演算子AND、ORを使用して複雑な検索クエリを開発する"
description: "GroupDocs.Search .NET APIを使用すると、コンピュータープログラマーは、.NETアプリケーション内でブール演算子(AND、OR、NOT) を使用して複雑な検索クエリを開発できます。 "

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "ブール検索とは何ですか？ブール演算子の使用方法は？"
    content: |
       ブール検索は、ユーザーがさまざまなキーワードを演算子と組み合わせて、検索結果をバインド、拡大、および定義できるようにする非常に便利な検索手順です。 AND、OR、NOT、NEARなどのブール演算子は、制限を定義することにより、ユーザーがより広い範囲の結果を取得したり、無関係な検索結果の数を減らしたりするのに役立ちます。 GroupDocs.Search for .NETは、強力な高性能ドキュメント検索APIであり、ソフトウェア開発者は、PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシートなどの最も一般的なドキュメントファイル形式のテキスト検索とインデックス作成を実行できるアプリケーションを開発できます。 、PowerPointプレゼンテーション、Outlook MSG、PSTなど。ブールAND演算子を使用して、入力したすべての単語の結果を表示できます。OR演算子を使用すると、入力した任意の単語の結果を表示できます。NOT演算子を使用すると、出現しない検索結果を表示できます。優れた機能の1つは、キーボードレイアウトと一致しない言語で記述された検索クエリを認識できることです。  

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NETを介した検索クエリでブールAND演算子を使用する"
      content_left: |
       GroupDocs.Search .NET APIは、.NETアプリケーション内にブール検索機能を追加するための完全なサポートを提供します。 以下のC＃コード例は、独自の.NETアプリケーション内でテキストおよびオブジェクト形式のクエリでブール「AND」演算子を作成する方法を示しています。

      title_right: " ブール演算子ANDを使用してZIPドキュメントを検索 "
      content_right: |
         * まず、インデックスフォルダとドキュメントフォルダへのパスを指定する必要があります。
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
         * [検索](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
         * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)クラスを呼び出してサブクエリ1を作成し、サブクエリ2を作成する
         * [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search) メソッドを呼び出して、サブクエリを1つのクエリに結合します
         * 検索を開始し、検索結果を表示します
         
        
      gisthash: "fa9773cd8d0f379a638e495ad2541a5b"
      gistfile: "use_boolean_and_operator_dotnet.cs"

    - title_left: "ブール演算子の使用方法または.NET経由"
      content_left: |
       GroupDocs.Search for .NETは、ソフトウェアプログラマーが多くの一般的なドキュメント形式を検索できるようにする強力なAPIです。 以下のC＃.NETコード例は、C＃アプリケーション内のテキストおよびオブジェクトフォームクエリでブール「OR」演算子を使用する方法を示しています。

      title_right: "ブールOR演算子を使用してZIPファイルを検索します"
      content_right: |
        * まず、インデックスフォルダとドキュメントフォルダへのパスを指定する必要があります。
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
        * [検索](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
        * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery) クラスを呼び出してサブクエリ1を作成し、サブクエリ2を作成する
        * [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) メソッドを呼び出して、サブクエリを1つのクエリに結合します
        * 検索を開始し、検索結果を表示します
     
      gisthash: "c0b22e80f881f8dbc0da17f92c01efc7"
      gistfile: "use_boolean_or_operator_dotnet.cs"
      
    - title_left: "ブール演算子を使用して複雑な検索クエリを作成する"
      content_left: |
        GroupDocs.Search .NETを使用すると、コンピュータープログラマーは、さまざまなブール演算子を組み合わせて、独自の.NETアプリ内に複雑な検索クエリを作成できます。 次の.NETコード例は、外部のソフトウェアやツールをインストールせずにドキュメント検索機能を複雑にする方法を示しています。

      title_right: "複雑な検索クエリを使用してZIPドキュメントを検索する"
      content_right: |
        * まず、インデックスフォルダとドキュメントフォルダへのパスを指定する必要があります。
        * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2)クラスのインスタンスを呼び出して、指定したフォルダーにインデックスを作成します
        * [検索](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)メソッドを呼び出して、指定したフォルダーからドキュメントにインデックスを付ける
        *検索を開始し、検索結果のテキストクエリを表示します
        *オブジェクトクエリで検索
        * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)クラスを呼び出してWordQueryとrelativityWordQueryを作成する
        * [CreateAndQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/index/methods/search)メソッドを呼び出して、サブクエリを1つのクエリに結合します
        * [SearchQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery)クラスを呼び出してeinsteinWordQueryとalbertWordQueryを作成する
        * [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) メソッドを呼び出して、サブクエリを1つのクエリに結合します
        * [CreateOrQuery](https://apireference.groupdocs.com/search/net/groupdocs.search/searchquery/methods/createorquery) メソッドを呼び出して、サブクエリを1つのクエリに結合します
        * 検索を開始し、検索結果を表示します
     
      gisthash: "216af02ebdd08331fdd05faf8c39e528"
      gistfile: "create_complex_queries_boolean_operator_dotnet.cs"

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