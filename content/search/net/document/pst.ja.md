---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/net/document/pst/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPT PPS POT PPTX PPTM POTX POTM PPSX PPSM PST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "ドキュメントの作成と追加.NETアプリケーション内での検索とインデックス作成"
head_description: "GroupDocs.Search .NET APIを使用すると、.NET Apps内で、PDF DOC、DOCX、RTF、XLSX、CSV、PPTX、および電子メールメッセージなどのサポート形式を検索するインスタントドキュメントを追加できます。"

############################# Header ############################
title: "C＃.NETAPIを介してインスタントドキュメント検索をPST に追加する方法 "
description: "GroupDocs.Search .NET APIを使用すると、開発者は堅牢なドキュメント検索およびインデックス作成機能をアプリに追加できます。 PDF DOC、DOCX、RTF、XLSX、CSV、PPT、PPTX、MSG、EMLなどのドキュメントをサポートします。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: ".NET APIを使用してドキュメントの検索とインデックス作成を作成および追加する方法は？"
    content: |
       このページは、ユーザーがわずかな労力とコストで自分のアプリケーション内にドキュメント検索およびインデックス作成機能を追加する方法を学ぶのに役立ちます。インデックス作成は、関連する検索結果を生成できるようにデータを整理および構造化するために検索エンジンで使用されるプロセスです。目的は、ユーザーのクエリに関連する情報をすばやく正確に見つけて表示することです。 GroupDocs.Search for .NETは、強力な高性能ドキュメント検索APIであり、ソフトウェア開発者が独自のアプリケーション内でファジーおよび同義語アルゴリズムに基づいて高度な検索およびインデックス作成操作を実行できるようにします。ユーザーのマシンにサードパーティのツールや外部ソフトウェアをインストールする必要はありません。 PDF、HTML、Outlook電子メール、Microsoft Office Word、Excelワークシート、PowerPointプレゼンテーション、Outlook MSG、PSTなど、最も一般的に使用されるドキュメント形式のサポートが含まれています。単純な単語、ブール、正規表現検索、大文字と小文字を区別する検索、柔軟なファジー、同義語、ホモフォン、ワイルドカード、チャンクによる検索、オブジェクトタイプ検索、データ範囲の設定など、いくつかのタイプの検索をサポートします。 

############################# content ############################
steps:
    enable: true
    block:
    - title_left: ".NETAPIを介したPSTドキュメントのインデックス作成の検索"
      content_left: |
       GroupDocs.Search .NET APIは、独自のアプリ内で新しいインデックスを作成したり、既存の検索インデックスを開いたりするための完全なサポートを提供します。 以下のC＃コード例は、数行のコードを使用して、新しいインデックスを作成し、既存のインデックスを開く方法を示しています。 

      title_right: "新規または既存の検索インデックスを開く方法"
      content_right: |
         * まず、インデックスフォルダへのパスを指定する必要があります
         * [Index](https://apireference.groupdocs.com/search/net/groupdocs.search/index/constructors/2) クラスのインスタンスを作成します
         *上記は、メモリまたはディスクにインデックスを作成し、既存のインデックスを開くこともできます。
       
      gisthash: "9651c19a9436afee860b7f39197f8399"
      gistfile: "create_or_open_new_search_index.cs"

    - title_left: "PSTドキュメントを検索インデックスに同期的に追加する方法"
      content_left: |
       GroupDocs.Search .NETを使用すると、ソフトウェア開発者は、独自の.NETアプリ内でドキュメントのインデックス作成を同期的に実行できます。 以下のC＃.NETコード例は、インデックス作成を簡単に同期的に実行する方法を示しています。 

      title_right: "C＃を介した同期ドキュメントインデックス作成"
      content_right: |
        * まず、インデックスフォルダへのパスを指定する必要があります
        * 検索するドキュメントを含むフォルダへのパスを指定します
        * [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) クラスのインスタンスを作成します
        * 上記は、メモリまたはディスクにインデックスを作成するか、既存のインデックスを開きます。
        * 指定されたフォルダからの同期インデックスドキュメント
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_synchronously_to_indexing.cs"
      
    - title_left: ".NETを介して非同期でドキュメントのインデックス作成を実行する"
      content_left: |
        GroupDocs.Search .NETを使用すると、コンピュータープログラマーは、独自の.NETアプリ内で非同期のドキュメントインデックス作成を実行できます。 次の.NETコード例は、わずか数行のコードで非同期にドキュメントのインデックス作成を実現する方法を示しています。

      title_right: "非同期 PST C＃によるドキュメントのインデックス作成 "
      content_right: |
        * まず、インデックスフォルダへのパスを指定する必要があります
        * 検索するドキュメントを含むフォルダへのパスを指定します
        * [Index(indexFolder)](https://apireference.groupdocs.com/search/net/groupdocs.search.indexrepository/search/methods/2) クラスのインスタンスを作成します
        * イベントへの登録
        * 操作の完了を示すコードを記述する必要があります
        * 非同期インデックスのフラグを設定する
        * 指定されたフォルダからの非同期インデックスドキュメント
     
      gisthash: "1c5f672c83e741280fd24c58fe51f707"
      gistfile: "add_files_asynchronously_to_indexing.cs"

    - title_left: "PST Docs.NETで検索結果を使用および強調表示する方法"
      content_left: |
       GroupDocs.Search .NET APIを使用すると、プログラマーはsarchの結果を解釈し、見つかったドキュメントの単純なリスト、または見つかった単語やフレーズによって結果を表示できます。 ドキュメントのテキストを簡単に強調表示することもできます。 次の.NETコード例は、見つかったドキュメントを一覧表示し、数行のコードで検索結果を強調表示する方法を示しています。

      title_right: "C＃を介してPSTファイルの検索結果を強調表示する "
      content_right: |
        * インデックスでのPeform検索
        * 検索に成功したら、結果を印刷します
        * ドキュメントを繰り返し、見つかったドキュメントを表示します
        * テキスト内の出現を強調表示
        * 検索結果が強調表示された出力HTML形式のドキュメントを生成する
     
      gisthash: "a5d1ad6eedd2acf12a33b541e763cdb4"
      gistfile: "how_to_list_search_result.cs"

    - title_left: "システム要求"
      content_left: |
        GroupDocs.Search for .NETは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 完全なシステム要件ガイドについては、以下のコードを実行する前に[システム要件](https://docs.groupdocs.com/search/net/system-requirements/) にアクセスしてください。次の前提条件がインストールされていることを確認してください。 システム：
          *オペレーティングシステム：Microsoft Windows、Linux、MacOS
          *開発環境：Visual Studio、Xamarin、MonoDevelopなど
          *フレームワーク：.NETフレームワーク、.NET標準、.NETコア、モノラル
          * [NuGet](https://www.nuget.org/packages/GroupDocs.search/) から最新バージョンのGroupDocs.Search for.NETAPIを入手してください。
        
      title_right: "GroupDocs.Assemblyを使用する理由"
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