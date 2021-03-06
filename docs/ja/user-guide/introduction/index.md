---
title: はじめに
page_id: "010.0"
---

## はじめに

### TreeFrog Framework とは

TreeFrog Framework は フルスタックの Web アプリケーションフレームワークです。C++ で作られているので、極めて高速かつ軽量（低リソース）に動作します。

C++フレームワークでありながら「設定より規約」のポリシーで、開発コストを抑えることを目指しています。設定ファイルは極力小さくなっており、また、足場となるコードの自動生成（スキャフォールディング）、テンプレートシステム、O/Rマッピング(ORM)や多くのヘルパーメソッドを提供しているので、開発者はロジックに専念できます。

### クロスプラットフォーム

TreeFrog Framework はクロスプラットフォームで動作します。Windows はもちろん、Linux や macOS の UNIX 系OS で動作するので、コーディングは Windows 上で行い、一般公開は Linux マシンで提供することが可能です。ソースコードをコンパイルしなおすだけで、複数のプラットフォームで動作するWebアプリができるのです。

### コントローラ

コントローラに中から、HTTPリクエスト／レスポンス、セッションのデータに簡単にアクセスできます。この他に、ログイン認証、フォームのバリデーション、アクセスコントールなどの便利な機能があらじめ提供されています。<br>
また、リクエストされた URL から該当するコントローラのメソッド（アクション）を呼び出す仕組み（ルーティングシステム）が備わっているので、リクエストをどのアクションに振り分けるかを設定ファイルにいちいちルールを書く必要はありません。

### ビュー

ビュー層では、Rails でよく知られたERB形式で記述することができます。HTMLファイルの中に <% … %> でC++コードを埋め込みます。スクリプト言語と似た感覚でコーディングすることができます。

もう１つ、テンプレートとプレゼンテーションロジックを完全に分離した新しいテンプレートシステム（Otama）を提供しています。テンプレートは純粋なHTMLで記述し、C++コードはロジックファイルに記述するのです。こうすることで、デザイナーとプログラマが協業することが可能になっています。

### モデル

モデル層では、SqlObject と呼ばれる O/R マッパー （O/Rマッピングシステム） が提供されます。このおかげでアプリ開発者は SQL をあまり書くことなくビジネスロジックの開発に専念できるでしょう。<br>
とは言っても、複雑な条件でデータを取り出す場合は、やはり SQL の出番となります。SQL の記述する際はプレースホルダを利用することで、簡単かつ安全にクエリを実行できます。<br>
また、本フレームワークは MySQL、PostgreSQL、SQLite、OracleやDB2といった主要なデータベースに対応しています。

### Qt ベース

TreeFrog Framework は Qt を使用しています（リンクしています）。Qt は GUI フレームワークという認識が強いですが、非GUIの機能も大変優れているのです。コンテナクラス、ネットワーク、SQL、JSON、ユニットテスト、メタオブジェクトのコアモジュールをWebアプリケーション向けにラップすることで、アプリ開発者は大変便利な機能を使うことができます。

### オープンソース

TreeFrog Framework は New BSD ライセンス (3-clause BSD License) を採用するオープンソースソフトウェアです。