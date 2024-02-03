
# FileWrapper_Setup![_2849a3fe-b4f9-4911-8150-1866270efe5e (1)](https://github.com/k-ayaki/FileWrapper_Setup/assets/40140916/355271c0-cc77-4298-89c0-a6e092a989e9)

特許経過情報取得アドインのsetup

# １．はじめに
 特許情報取得アドインとは、クラウドから特許情報を取得するアドイン・ソフトウェアです。出願の書誌事項、ファミリーリスト、経過情報、包袋などが取得可能であり、特許の中間コメントの作成を支援することができます。WORD画面上で編集中にシームレスに動作可能です。なお、上記アイキャッチ画像は、生成AIのDALL-E 3と、uncropで作成したものです。

 
# ２．動作環境
・OSは、Windows 10 32bit版、Windows 10 64bit版、Windows 11の何れかです。
・Office365同梱のWordまたはWord2019で動作します。
・ネットワークに接続可能な環境であることが必要です。

# ３．インストール方法
・Microsoft Wordを起動して、AppLintリボンに特許情報取得アドインに関連する以下のボタンが設定されているか確認してください。

<img width="113" alt="button" src="https://github.com/k-ayaki/FileWrapper_Setup/assets/40140916/9be33b13-7562-4ed8-b2a4-89d0557ea926">

# ４．操作画面
・特許情報ボタン、アカウントボタン、バージョンボタンが設けられています。

<img width="113" alt="button" src="https://github.com/k-ayaki/FileWrapper_Setup/assets/40140916/9be33b13-7562-4ed8-b2a4-89d0557ea926">

## ４．１．アカウントボタン
・アカウントボタンをクリックすると、Word画面の右側にアカウントペインが開きます。ここに、特許情報取得APIのアカウントを設定してください。なお、特許情報取得APIのアカウントは、APIを利用した特許情報の試行提供のページを参考に、特許庁に申し込んでください。

<img width="159" alt="account" src="https://github.com/k-ayaki/FileWrapper_Setup/assets/40140916/ae715a4a-f1aa-4735-9451-94119850fb30">

## ４．２．特許情報ボタン
・特許情報ボタンをクリックすると、Word画面の右側に特許情報ペインが開きます。ここに出願番号を入れて、各ボタンをクリックしてください。
・出願番号は、以下の何れかの形式を受け付け可能です。

<img width="156" alt="patentInfo" src="https://github.com/k-ayaki/FileWrapper_Setup/assets/40140916/a6de4bc2-48dc-480a-a0c3-4e8a5dcb25c3">


```
　特願２０２０－００８４２３
　２０２０－００８４２３
　２０２０－８４２３
　２０２０００８４２３
　特願2020-008423
　2020-008423
　2020-8423
　2020008423
```
・その後、出願の書誌情報ボタンをクリックすると、以下のような情報が現在の文書ファイルに挿入されます。

```
書誌事項：特願２０２０－００８４２３
　発明の名称：管理システム及び管理方法
　出願日：令和０２年０１月２２日
　公開番号：特開２０２１－０２２３５９
　公開日：令和０３年０２月１８日
　登録番号：特許第６６９１２８０号
　登録日：令和０２年０４月１４日
　存続期間満了年月日：令和２２年０１月２２日
　国内優先権出願番号：特願２０１９－１３９７５９
　国内優先権主張日：２０１９年０７月３０日
```

・「OPDファミリーリスト」ボタンをクリックすると、OPDファミリーのリストがDocdb形式で表示されます。

```
OPDファミリーリスト情報：2020008423
出願番号：JP.2020008423.A　出願日：2020-01-22
公開番号：JP.2021022359.A
登録番号：JP.6691280.B1

出願番号：JP.2020011838.W　出願日：2020-03-17
公開番号：WO.2021019831.A1
```

・「経過情報」ボタンをクリックすると、経過情報が表示されます。

```
経過情報：特願２０２０－００８４２３
　　　　出願　　　　　　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　　　　　　　　　　　　　　　　　　　　　（優先日２０１９年０７月３０日）
審査記録：特願２０２０－００８４２３
　　　　早期審査に関する事情説明書　　　　　　　　令和０２年０１月２２日
　　　　明細書　　　　　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　請求の範囲　　　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　特許願　　　　　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　図面　　　　　　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　要約書　　　　　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　出願審査請求書　　　　　　　　　　　　　　令和０２年０１月２２日
　　　　手続補正書　　　　　　　　　　　　　　　　令和０２年０２月０６日
　　　　添付書類　　　　　　　　　　　　　　　　　令和０２年０２月０６日
　　　　早期審査に関する報告書　　　　　　　　　　令和０２年０３月０２日
　　　　特許査定　　　　　　　　　　　　　　　　　令和０２年０３月１０日
　　　　優先権証明請求（電子データ交換協定）　　　令和０２年０４月０２日
　　　　優先権証明応答（電子データ交換協定）　　　令和０２年０４月０３日
　　　　要約不備職権訂正　　　　　　　　　　　　　令和０２年０４月０８日
　　　　ファイル記録事項の閲覧（縦覧）請求書　　　令和０２年０８月１３日
公開記録：特開５０３０－２２３５９
登録記録：特許第６６９１２８０号
　　　　特許査定　　　　　　　　　　　　　　　　　令和０２年０３月１０日
　　　　特許証　　　　　　　　　　　　　　　　　　令和０２年０４月２８日
審判記録：査定不服審判２０２０－７００８５０
　　　　異議申立書　　　　　　　　　　　　　　　　令和０２年１０月２９日
　　　　異議番号通知　　　　　　　　　　　　　　　令和０２年１１月１２日
　　　　異議番号通知　　　　　　　　　　　　　　　令和０２年１１月１２日
　　　　異議番号通知　　　　　　　　　　　　　　　令和０２年１１月１２日
　　　　予告登録通知　　　　　　　　　　　　　　　令和０２年１１月１３日
　　　　審判官指定（変更）通知　　　　　　　　　　令和０２年１１月１９日
　　　　審判官指定（変更）通知　　　　　　　　　　令和０２年１１月１９日
　　　　異議の決定　　　　　　　　　　　　　　　　令和０２年１２月０７日
　　　　郵便送達報告書　　　　　　　　　　　　　　令和０２年１２月１１日
　　　　異議の決定　　　　　　　　　　　　　　　　令和０３年０１月１９日
　　　　再送　　　　　　　　　　　　　　　　　　　令和０３年０１月１９日
　　　　郵便送達報告書　　　　　　　　　　　　　　令和０３年０２月０２日
　　　　確定登録通知　　　　　　　　　　　　　　　令和０３年０２月０３日
出訴事件番号：５　０３１００３５
```

・「包袋取得」ボタンをクリックすると、包袋ファイルがカレントフォルダにダウンロードされ、かつ以下の簡略化した経過情報リストが表示されます。なお、リンクをクリックすると包袋ファイル（実体）が開きます。

```
経過情報：特願２０２０－００８４２３
　　　　出願　　　　　　　　　　　　　令和０２年０１月２２日
　　　　　　　　　　　　　　　　　　（優先日２０１９年０７月３０日）
　　　　出願審査請求書　（提出日）　　令和０２年０１月２２日
　　　　手続補正書　　　（提出日）　　令和０２年０２月０６日
　　　　特許査定　　　　（起案日）　　令和０２年０３月０２日
　　　　特許査定　　　　（発送日）　　令和０２年０３月１０日
```
