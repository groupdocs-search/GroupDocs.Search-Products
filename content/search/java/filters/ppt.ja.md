---
############################# Static ############################
layout: "auto-gen-gist"
draft: false
path: "ja/search/java/filters/ppt/"
otherformats: PDF DOC DOT DOCX DOCM DOTX DOTM TXT ODT OTT RTF XLS XLT XLSX XLSM XLSB XLTX XLTM XLA XLAM ODS OTS CSV TSV XML PPS POT PPTX PPTM POTX POTM PPSX PPSM ODP PST OST EML EMLX MSG ONE ZIP XHTML MHTML MD CHM EPUB  FB2 

############################# Head ############################
head_title: "Java API 経由で検索結果に PPT ドキュメント フィルタリングを統合しますか?"
head_description: "GroupDocs.Search Java API は、ソフトウェア開発者が PPT ドキュメント検索機能を追加し、ドキュメント フィルタリングを適用して Java API を介して検索結果をカスタマイズするのに役立ちます。"

############################# Header ############################
title: "ドキュメント フィルタリングを統合して Java アプリ内の検索結果をカスタマイズする方法"
description: "GroupDocs.Search Java API を使用すると、プログラマーは高度な PPT ドキュメント検索機能を統合したり、Java アプリでドキュメント フィルタリングを設定して検索結果をカスタマイズしたりできます。"

######################### Download Button #######################
button:
    enable: true

############################# About ############################
about:
    enable: true
    title: "ドキュメント フィルタリングを統合して Java アプリ内の検索結果をカスタマイズする方法"
    content: |
       ドキュメント フィルタリングは、ソフトウェア アプリケーションがドキュメントを検索および取得できるようにする非常に便利なアクティビティです。これにより、ユーザーがインデックス付きドキュメントのテキストに入力した関連する一連の単語が検索されます。フィルターには、レコードの選択に使用される基準を定義する一連のルールが含まれています。ドキュメント フィルタリングにより、ユーザーは検索を特定のセクションまたは特定のドキュメント タイプに限定したり、結果をナビゲートして探しているものを見つけたりすることができます。 GroupDocs.Search for Java は、機能豊富な高性能ドキュメント インデックス作成および検索 API であり、ソフトウェア開発者は、最も一般的なドキュメント ファイル形式のテキスト インデックス作成および検索を実行できるアプリケーションを作成できます。 PDF、HTML、Outlook 電子メール、Microsoft Office Word、Excel ワークシート、PowerPoint プレゼンテーション、Outlook MSG、PST などのさまざまなドキュメント タイプを完全にサポートします。ファイルパスフィルター、ファイル拡張子フィルター、属性フィルターなど、ユーザーが検索結果をカスタマイズするために使用できるさまざまな種類のファイラーがあります。

############################# content ############################
steps:
    enable: true
    block:
    - title_left: "Java 経由で PPT ドキュメントを検索する際にドキュメント フィルタを適用する"
      content_left: |
       GroupDocs.Search Java API は、ソフトウェア開発者が Java API を使用して検索機能を備えた強力なアプリケーションを作成するのに役立ちます。 以下の Java コード例は、わずか数行のコードでさまざまな種類のドキュメントを検索するためのドキュメント フィルタを適用する方法を示しています。

      title_right: "PPT文書検索時の文書フィルター設定"
      content_right: |
       * 最初に、インデックス フォルダーとドキュメント フォルダーへのパスを指定する必要があります。
       * [Index](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#Index(java.lang.String)) クラスのインスタンスを呼び出して、指定したフォルダにインデックスを作成する
       * [add](https://apireference.groupdocs.com/search/java/com.groupdocs.search/Index#add(java.lang.String)) メソッドを呼び出して、指定したフォルダーからドキュメントのインデックスを作成する
       * [earchOptions](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions) クラスを呼び出して検索オプション オブジェクトを作成する
       * [setSearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) メソッドを呼び出して、ドキュメント フィルターを設定します。
       * 検索を開始し、見つかった場合はテキスト ドキュメントを表示します
        
      gisthash: "6ad4038623777576484491239ce17125"
      gistfile: "set_document_filter_in_search_java.java"

    - title_left: "検索ドキュメント フィルターを組み合わせて Java 経由で複合フィルターを作成する"
      content_left: |
        GroupDocs.Search for Java を使用すると、ソフトウェア プログラマーは高度な検索機能を追加し、Java アプリケーション内のドキュメント検索にカスタム フィルターを適用できます。 ユーザーは、さまざまな種類の検索フィルターを組み合わせて、複合フィルターを作成できます。 次の Java コードは、検索ドキュメント フィルターを組み合わせて、ブール演算子 AND、OR、NOT などを使用して複合フィルターを作成する方法を、わずか数行のコードで示しています。

      title_right: "PPT ファイルを検索する複合フィルタを作成"
      content_right: |
       * 最初に、インデックス フォルダーとドキュメント フォルダーへのパスを指定する必要があります。
       * 絶対パスに「Einstein」という単語が含まれるすべての FB2 および EPUB ドキュメントを返す AND 複合フィルタを作成する
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) を呼び出して、filter1 を作成します。
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) を呼び出して、filter2 を作成します。
       * [createAnd](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createAnd(com.groupdocs.search.options.ISearchDocumentFilter...)) メソッドを呼び出してフィルターを組み合わせる
       * すべての DOC、DOCX、PDF、およびフル パスに Einstein という単語が含まれるすべてのドキュメントを返す OR 複合フィルターを作成します。
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) を呼び出して、filter3 を作成します。
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) を呼び出して、filter4 を作成します。
       * [createOr](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createOr(com.groupdocs.search.options.ISearchDocumentFilter...)) メソッドを呼び出してフィルターを組み合わせる
       * TXT ドキュメントを除く、見つかったすべてのドキュメントを返すフィルターの作成
       * [SearchDocumentFilter](https://apireference.groupdocs.com/search/java/com.groupdocs.search.options/SearchOptions#setSearchDocumentFilter(com.groupdocs.search.options.ISearchDocumentFilter)) を呼び出して、filter4 を作成します。
       * [createNot](https://apireference.groupdocs.com/search/java/com.groupdocs.search/SearchDocumentFilter#createNot(com.groupdocs.search.options.ISearchDocumentFilter)) メソッドを呼び出して Not フィルターを適用する

      gisthash: "db9ab9384dcacb90c5bbdad98a2d2cba"
      gistfile: "combine_document_filter_in_search_java.java"
      
    - title_left: "システム要求"
      content_left: |
        GroupDocs.Search for Javaは、すべての主要なプラットフォームとオペレーティングシステムでサポートされています。 完全なシステム要件ガイドについては、以下のコードを実行する前に[システム要件](https://docs.groupdocs.com/search/java/system-requirements/) にアクセスしてください。次の前提条件がインストールされていることを確認してください。 システム：
          *オペレーティングシステム：Microsoft Windows、Linux、MacOS
          * Javaバージョンのサポート：J2SE 7.0（1.7）、J2SE 8.0（1.8）以降
          * GroupDocsの最新バージョンを入手します。GroupDocs[リポジトリ](https://repository.groupdocs.com/repo/com/groupdocs/groupdocs-search/) からJavaAPIを検索します。
        
      title_right: "GroupDocs.Searchを使用する理由"
      content_right: |
        * メモリ内およびディスク上での検索インデックスの作成。
        * ファイル、ストリーム、または構造からインデックスを作成する機能。
        * パスワードで保護されたドキュメントのインデックス作成のサポート。
        * 複数のインデックスのマージのサポート。
        * 検索のインデックス作成中にドキュメントをフィルタリングします。
        * 検索中のスペルチェックのサポート。
        * ブレンドされた文字は完全にサポートされています
        * さまざまな種類の検索を1つの検索クエリに結合します。
        * 単純な単語と正規表現の検索のサポート
        * 検索クエリでのエイリアス置換を完全にサポートします。

demos:
    enable: true
        

more_formats:
    enable: true


back_to_top:
    enable: true
---