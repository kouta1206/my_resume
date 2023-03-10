# 職務経歴書

## アジェンダ
- [職務経歴書](#職務経歴書)
  - [アジェンダ](#アジェンダ)
  - [職務経歴](#職務経歴)
  - [アサインプロジェクト](#アサインプロジェクト)
    - [高齢者向けヘルスケアサービス](#高齢者向けヘルスケアサービス)
  - [失敗から何を学んだか？（どう乗り越えていったか）](#失敗から何を学んだかどう乗り越えていったか)
  - [このプロジェクトで何を成し遂げたか？(問題解決事項)](#このプロジェクトで何を成し遂げたか問題解決事項)
  - [訪問介護員向けアセスメントサービス](#訪問介護員向けアセスメントサービス)
  - [失敗から何を学んだか？（どう乗り越えていったか）](#失敗から何を学んだかどう乗り越えていったか-1)
  - [このプロジェクトで何を成し遂げたか？(問題解決事項)](#このプロジェクトで何を成し遂げたか問題解決事項-1)
  - [技術スタック](#技術スタック)
    - [言語](#言語)
    - [フレームワーク・その他](#フレームワークその他)
  - [自己PR](#自己pr)
  - [その他](#その他)
  - [ポートフォリオ](#ポートフォリオ)
## 職務経歴
|  会社名  |  期間  |  やったこと  |
| ---- | ---- | ---- |
|  [Trilium株式会社]()(現:ブロードバンドテクノロジーコンサルティング株式会社)  |  2022/03 〜 2023/01  | システムエンジニアリングサービスとして開発業務にアサイン |
|  [ALSOK香川株式会社]  |  2016/04 〜 2022/03 | 空港保安業務|


## アサインプロジェクト

### 高齢者向けヘルスケアサービス
<br/>

利用者に対して、健康状態をWeb上でアセスメントし利用者に応じた、健康レシピの提供、zoomでの運動トレーニングの実施、看護師による、面談の実施を提供するWebアプリケーション
<br/>

- プロジェクト規模
    - バックエンド5名、フロントエンド2名、デザイナー1名、プロジェクトリーダー1名。計10程度のメンバーで担当
- 役割
    - フロントエンド
        - WordPressのデザイン修正
        - ページネーションのデザイン修正(テンプレートエンジン)
        - スケジュールのバグフィックス(Vue.js)
    - バックエンド
        - 協業している外部API連携の実装
        - スケジュールAPI側修正
- 使用技術
    - フロントはVue.js、テンプレートエンジンを使用（一部WordPress）
     - バックエンドはLaravelを使用
     - インフラはAWSを使用
     - GitHubを使用したチーム開発(10人)

<br/>

## 失敗から何を学んだか？（どう乗り越えていったか）
未経験より初のプロジェクトにアサインされ、当初は理解するのにも右も左もわからない状況でした。
タスクの進め方、実装の仕方、実務におけるGitHubのフロー、デバッグの方法、エラーログの見方等々。
以前より、エンジニアになる前から習慣化している事がありました。それはゼロ秒思考です。
ですので、直面する課題をまずは書き出し、課題を明確にし、タスクバラシをしていく事を学びました。
以上のことから、困難は切り離し、タスクを細分化する事が重要だと学ぶ事できました。

<br/>

##  このプロジェクトで何を成し遂げたか？(問題解決事項)
カレンダーページでスケジュールごとのチェックボックスが存在しチェックをtrue,falseで切り替える度にAPIが飛ぶ仕様があったのですが、
スケジュールの種類が多く、かつ頻繁に切り替える事から、APIが頻繁に飛んでカレンダーページだけパフォーマンスにかけている部分が存在
していました。
そこで、PLと相談いただける機会を設け、タスクに余裕があった事から、仕様を変更いただける機会をいただき、PLと密に仕様を再定義し、
一度のページ遷移でユーザーに紐付いているスケジュールを全て取得し、スケジュールの表示、非表示は頻繁に切り替える事から、フロント側で
制御させる事で、カレンダーページのパフォーマンス向上させる事ができました。

<br/>

## 訪問介護員向けアセスメントサービス

訪問介護員が訪問介護時にアセスメントを実施して記録するWebシングルページアプリケーション

- プロジェクト規模
    - バックエンド5名、フロントエンド2名、プロジェクトリーダー1名、計８名程度のメンバーで担当
- 役割
    - フロントエンド
        - Nuxt.jsを用いた新規機能開発のフロントエンド開発
    - バックエンド
        - Laravelを用いた新規機能開発のAPI開発
- 使用技術
    - フロントはNuxt.js
     - バックエンドはLaravelを使用
     - インフラはAWSを使用
     - AWSのサービスである、CodeCommitを使用したチーム開発

<br/>

## 失敗から何を学んだか？（どう乗り越えていったか）
バックエンドにLaravelを用いており、今までLaravelのAPI開発にはORMを用いた開発を
やってきておりましたが、今回のプロジェクトではAPI開発にクエリビルダでの実装というコーディング規約
があり、SQLライクな実装を心掛ける必要がありました。ORMで実装している時はSQLをあまり気にする
必要もなく、今回でSQLの必要性を非常に感じました。
まず、クエリビルダで実装する為にも業務外では、既存のAPI処理のコードリーディングを図りました。
コールドリーディングを実施する上で理解できない箇所は全て、DBクライアントツールで確認しました。
また、テーブルが多く存在しており、サブクエリを多用に使用しておりましたので、サブクエリもDBクラアント
ツールで確認し、テンポラリーテーブルがどういったテーブルなのかも逐一確認しました。
これらを実施する事で、与えて頂いた新規機能開発のタスクをこなす事ができました。

<br/>

##  このプロジェクトで何を成し遂げたか？(問題解決事項)
今まで、コードレビューの経験がなくやってみたい事の1つでした。
ミーティングでフロントにおけるコードレビューをできる人が少なく、自身が経験したかったのもあり
率先して手を上げ、コードレビューの機会を頂きました。
フロントはNuxt.jsを使用しておりましたので、実務における経験はありませんでしたが、フロントにおける
コードレビューをメインで担当させていただく事になりました。
コードレビューで学んだ事は憶測でコードリーティングしない事と、ドメイン知識を実装者又は、PLに
確認することが肝要だと学びました。

<br/>


## 技術スタック

### 言語
- 実務 
  <p>
  <img alt="JavaScript" src="https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=JavaScript&logoColor=white" />
  <img alt="PHP" src="https://img.shields.io/badge/-PHP-4B275F?style=flat-square&logo=PHP&logoColor=white" />
  <img alt="HTML" src="https://img.shields.io/badge/-HTML-0095D5?style=flat-square&logo=HTML&logoColor=white" />
  <img alt="CSS" src="https://img.shields.io/badge/-CSS-007396?style=flat-square&logo=CSS&logoColor=white" />
    </p>
- 実務外
    <p><img alt="Ruby" src="https://img.shields.io/badge/-Ruby-CC342D?style=flat-square&logo=Ruby&logoColor=white" /></p>


### フレームワーク・その他
- 実務
    <p>
        <img alt="Vue.js" src="https://img.shields.io/badge/-Vue.js-4FC08D?style=flat-square&logo=Vue.js&logoColor=white" />
        <img alt="Nuxt.js" src="https://img.shields.io/badge/-Nuxt.js-45b8d8?style=flat-square&logo=Vue.js&logoColor=white" />
         <img alt="Laravel" src="https://img.shields.io/badge/-Laravel-092E20?style=flat-square&logo=Laravel&logoColor=white" />
        <img alt="Vuex" src="https://img.shields.io/badge/-Vuex-646CFF?style=flat-square&logo=Vuex&logoColor=white" />
        <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
    </p>
- 実務外
    <p>
         <img alt="Ruby-on-Rails" src="https://img.shields.io/badge/-Rails-CC0000?style=flat-square&logo=Ruby-on-Rails&**logoColor****=white" />
         <img alt="AWS" src="https://img.shields.io/badge/-AWS-CC0000?style=flat-square&logo=AWS&**logoColor****=white" />
    </p>

## 自己PR
私は解決課題を俯瞰的に捉え問題解決にあたっていく事を得意とします。
私は未経験からアサインされたプロジェクトでは、上記で挙げた様々な問題が発生しておりました。
ただ、これらの問題を自身の信念に従って、今必要なものは何なのか？、現状足りない自身のリソース
はどこなのか？と問題を俯瞰的、客観的に注視する事で最短でPDCAを回して問題解決にあたる事が
得意だと認識しました。
ただ、課題解決を俯瞰的に捉えるには以下の能力も必要だと考えております。
- 具体から抽象を認識する能力
- 高度なコミュニケーション能力
- 問題解決能力

自身の課題解決の俯瞰的に捉え問題解決にあたっていく能力を最大限に上げる為にも、これらの能力
を今以上に高めていきます。

<br/>

## その他
- 今後成し遂げたいこと（やってみたい事）
    - 新規事業開発
      - 新規事業開発にも携わりたいと思っております。
        というのも、システムエンジニアリングサービスでアサインされたのは、すべて要件定義、設計以降の
        アサインが全てでした。やはり、自分たちが考えてプロダクトを作っていくというプロセスにやりがいを感じて
        おり、今回転職を決意した理由の一つでもあります。

    - 英語
      - もともと英語が好きだったのですが、高校時代に英検2級を取得して依頼業務で使う事もなかったので
      英語学習とは疎遠になっておりました。
      しかし、エンジニアに転職してから英語の必要性を肌で感じています。公式ドキュメント、変数名、
      学習教材等、必然的に英語を使用する機会が多く苦労する場面が多いのでTOEICなど業務で苦にならないように学習していきます。

    - 技術登壇、アウトプット
       - 休日は業務のインプットばかりでしたので、アウトプットの頻度を上げていきます。
        Qiitaによる技術記事の投稿頻度を上げたり、LT登壇をやります。

<br/>

## ポートフォリオ
Railsの学習と趣味が映画鑑賞ですが、以前から鑑賞した映画の記録Webアプリがあればなと、
考えておりました。今回の機会に簡易的なWebアプリを作成してみました。
- 作成期間
    - 1ヶ月程度
- 使用技術
    - バックエンド
        - <p>
            <img alt="Ruby-on-Rails" src="https://img.shields.io/badge/-Rails-CC0000?style=flat-square&logo=Ruby-on-Rails&**logoColor****=white" />
        </p>
    - フロントエンド
      - <p>
            <img alt="Nuxt.js" src="https://img.shields.io/badge/-Nuxt.js-45b8d8?style=flat-square&logo=Vue.js&logoColor=white" />
        </p>
    - その他
        - <p>
              <img alt="Docker" src="https://img.shields.io/badge/-Docker-46a2f1?style=flat-square&logo=docker&logoColor=white" />
                <img alt="AWS" src="https://img.shields.io/badge/-AWS-CC0000?style=flat-square&logo=AWS&**logoColor****=white" />
                <img alt="CI/CD" src="https://img.shields.io/badge/-CI/CD-CC0000?style=flat-square&logo=CI/CD&**logoColor****=white" />
                <img alt="jwt認証" src="https://img.shields.io/badge/-jwt認証-CC0000?style=flat-square&logo=jwt&**logoColor****=white" />
        </p>
<br>

- URL（下記のURLになります）
    - https://github.com/kouta1206/movie_record_app


