# Frank Furt

[![IMAGE ALT TEXT HERE](https://github.com/jphacks/C_2002/wiki/images/pop-logo.png)](https://github.com/jphacks/C_2002/wiki/images/pop-logo.png)

## デモ動画

## アーキテクチャ

[![Architecture.png](https://github.com/jphacks/C_2002/blob/master/%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3/Architecture.png?raw=true)](https://github.com/jphacks/C_2002/blob/master/%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3/Architecture.png?raw=true)


## 製品概要

### ビジネスマナー × Tech

[![×TECH.png](https://github.com/jphacks/C_2002/blob/master/%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3/%C3%97TECH.png?raw=true)](https://github.com/jphacks/C_2002/blob/master/%E3%83%97%E3%83%AC%E3%82%BC%E3%83%B3/%C3%97TECH.png?raw=true)

### 背景(製品開発のきっかけ、課題等）
COVID-19(新型コロナウイルス)の影響により世の中で様々なことがオンライン化した．
その中でコミュニケーション様式もまた大きな影響を受け，**対面からビデオ会議やテキストベースに変化**している．
テキストベースのコミュニケーションでの適切な言葉遣いという点に着目した．
また、近年は，LINEといったチャット形式のコミュニケーションツールが普及し，若者がメール形式でコミュニケーションを行うことが減った。
従って、電子メールなどを作成する際に**適切な体裁や言葉遣いを意識しない**傾向にある．
こうした傾向を背景にして私たちは「チャットに慣れた者が適切な体裁・言葉遣いが上手くできない」ということを課題とした．

### 製品説明（具体的な製品の説明）
本製品は，**統合ビジネスメール作成環境(IBE)** の **デスクトップアプリ** である．

* 就職活動を行っている大学生と，若手社員のためのメールクライアントソフトウェア

* メール文をビジネスに即したメールに変換し、送信を行う

### 特長

#### 1. **エンジニアが使う超有能ツールをユーザーのメール作成に落としこみ，意識することなく利用可能**
*  **Gitによるメール文の差分管理**
Gitのコードの差分管理をメール文の差分管理に使用することで，文章校正の高速化を実現した。

*  **IDEの機能をビジネスメール作成補助に応用**
   * **文章校正**
   コードのデバッグやコンパイルのように，メールを作成した際に，自動で校正や敬語変換を行い、丁寧な表現に変換ができる．ON/OFFで切り替え可能．．
   * **ソフトウェア内で送受信**
   IDE内のターミナル上でコードを実行できるように、ソフトウェア上で文章作成から送受信までを一括で行える．

#### 2. **チャット形式のUI**
メールの送受信の確認のUIをチャット形式にすることで，ビジネスメールに不慣れで且つエンジニアではない若者に受け入れられやすい動作性をもっている．

### 解決出来ること
* 不適切なメール文での悪印象を回避
    * ビジネスメールのやりとりで生じる不適切なメール本文を事前に修正

* メールの見落としを無くす
    * メールのやりとりをメール相手によってフィルタリングし，さらに送受信の方向性を一目でわかるUI

### 今後の展望
今後は対応できるメールサービスの数を増やし，1つのアプリケーションでの完結性を向上させる．

# **そのほかもあれば**

### 注力したこと（こだわり等）
* 特長の内容
* クロスプラットホームで、OSに関わらず使用することが可能
* 認証情報は、サーバーにあげずに保管するため、セキュリティ面も安心

## 開発技術
### 活用した技術

#### 使用言語
* HTML
* SCSS
* JavaScript
* Python 3

#### フレームワーク・ライブラリ・モジュール
* [Git](https://git-scm.com/)
* [Vue.js](https://jp.vuejs.org/index.html)
* [Node.js](https://nodejs.org/ja/)
* [Electron](https://www.electronjs.org/)
* [jQuery](https://jquery.com/)
* [Flask](https://flask.palletsprojects.com/en/1.1.x/)
* [MySQL](https://www.mysql.com/jp/)

#### API・データ
* スポンサー様の提供サービス
    * [goo ラボ API](https://labs.goo.ne.jp/)
        * [固有表現抽出API](https://labs.goo.ne.jp/api/jp/named-entity-extraction/)
        * [形態素解析API](https://labs.goo.ne.jp/api/jp/morphological-analysis/)
        * [時刻情報正規化API](https://labs.goo.ne.jp/api/jp/time-normalization)
* 外部サービス
    * [AWS EC2](https://aws.amazon.com/jp/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc)
    * [Proofreading API](https://a3rt.recruit-tech.co.jp/product/proofreadingAPI/)

#### デバイス
* なし

### 独自技術
#### ハッカソンで開発した独自機能・技術
* 独自で開発したものの内容をこちらに記載してください
* 特に力を入れた部分をファイルリンク、またはcommit_idを記載してください。
* アプリケーションの画面や画面遷移等
    * **[メールの送受信をチャット形式で表示](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/components/columns/ChatTree.vue)**
    * [メールの作成画面](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/components/columns/MailEditer.vue)
    * [校正画面](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/components/columns/Preview.vue)
* アプリケーション本体の処理
    * [クライアント側の処理](https://github.com/jphacks/C_2002/tree/master/front/src)（Electron）
        * **[メール本文の差分管理](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/utils/NodeGit.js)**（Git）
        * [クロスプラットフォーム対応](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/utils/OS.js)
        * [メール送信](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/utils/MailSend.js)
        * [メール受信](https://github.com/jphacks/C_2002/blob/master/front/src/renderer/utils/MailReceive.js)
        * カレンダーイベント(.ics)ファイルの作成（時刻情報正規化API）
    * [サーバ側の処理](https://github.com/jphacks/C_2002/blob/master/server/server.py)（AWS EC2）
        * **[敬語への変換](https://github.com/jphacks/C_2002/blob/master/server/FunctionTest/NewHonorificsConvert.py)**（形態素解析API，機械学習）
        * [人名と会社名の抽出](https://github.com/jphacks/C_2002/blob/master/server/FunctionTest/ExtractProperNoun.py)（固有表現抽出API）
        * [校正箇所の指摘](https://github.com/jphacks/C_2002/blob/master/server/FunctionTest/Proofreading_RECRUIT.py)（Proofreading API）
        * [日時情報の抽出](https://github.com/jphacks/C_2002/blob/master/server/FunctionTest/getTime.py)(時刻情報正規化API)

#### 製品に取り入れた研究内容（データ・ソフトウェアなど）（※アカデミック部門の場合のみ提出必須）
* なし

#### 事前開発プロダクト
* なし


## 開発チーム
### Pied Piper

* [RyogaTakao](https://github.com/RyogaTakao): サーバーサイド
* [YoshiharuSenna](https://github.com/YoshiharuSenna): サーバーサイド
* [ReERishun](https://github.com/ree-rishun): フロントエンド
* [OkazakiTatsuya](https://github.com/TatsuyaOkazaki324): フロントエンド
* [rappy-git](https://github.com/rappy-git): データサイエンティスト, 情報収集
* [Miyu Oba](https://github.com/mlieynua): データサイエンティスト, 情報収集
