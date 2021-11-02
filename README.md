# コミュニティの目的
1. OSS 初心者学びの場
2. OSS 技術者交流の場

既存のコミュニティでは OSS の開発を目的としたやり取りがなされることが多いです。  
その OSS をこれから利用しようという初心者からすると、  
コミュニティ内ディスカッションの内容が理解できず学習が進まないということがあります。

そのため、本コミュニティでは OSS を限定することなく  
これから OSS を学ぼうという方を対象とした学びの場・技術者交流の場として設立しました。

# 参加する
[こちら](https://sios-oss-bbs.slack.com/)から参加できます。

# チャンネルについて
* ```#question``` メインチャンネル。質問はここへ  
* ```#general``` コミュニティ運営からのお知らせなどを通知するチャンネル  
* ```#randam``` 雑談用チャンネル  
* ```#newbie``` 自己紹介用チャンネル。自己紹介したい方はここへ  
* ```#discussion``` 運用のベストプラクティスなど明確な答えがないノウハウを語るための、議論用チャンネル  

# 基本ルール
* お互いに敬意を持ったコミュニケーションをとりましょう。
* コミュニティの目的から大きく逸脱する行為は禁止します。
* 公序良俗に反する行動やハラスメント行為は禁止します。
* 著作権を侵害する行為や犯罪、セキュリティ侵害につながる行動を禁止します。

# 質問に関するマナー
* 初めに  
　わからない部分について、質問をするだけでも十分すごいです！  
　「動くからいいや」「エラーを無視しよう」とならず、人に質問するのは大変な勇気が要る行為です。
 
　　そもそも質問の仕方にもコツが要るものです。

　　本項目ではそんなコツを説明します。  
　　意識したうえで質問をいただければより早く高い精度での解決につながるので、  
　　ルール程強い縛りではないですがマナー程度にとらえてください。
 
* 質問のコツ  
　●**質問の背景を教えてください**  
　●**動作環境を教えてください**  
　●**実施した作業や試みた解決策を教えてください**  
　●**エラーメッセージは抜粋や編集することなく提供してください**  

* 具体例  
　具体的に良い質問と悪い質問を考えてみましょう

　　よくない例  
```
　Web サーバが重いです。対応を教えてください。  
```

　　どこが良くないの？  
　　　1. WEB サーバとして利用できる OSS は複数あります(Apache や NGINX など)。  
　　　そのため、環境がまったくわからず、アドバイスができません。

　　　2. 「重い」という状況が漠然としています。  
　　　どこを確認して重いと判断したのか教えてください。

　　　3. 問題の着点がわからないです。  
　　　原因が知りたいのか、事象が解決できれば OK なのか、目的を明確にしましょう。

　　上記例を修正した例  
```
・事象  
　Apache を利用している WEB サーバでクライアントからのリクエストが滞留している。  

　普段セッションが 10 ～ 20 程度の WEB サーバで突然セッション数が増加しました。  
　それに伴い、一部クライアントからリクエストが受け付けられない状況となりました。  
　※実際にアクセスすると 10 回に1 回程度しかアクセスできません。  

・環境  
　CentOS 7.7.1908  
　httpd-2.4.6-97.el7.centos.x86_64  

・解決したい課題  
　1. まずは原因を知りたい  
　2. 解決策と再発防止策を考えたい
```  

　　理想を言うとログファイルやコマンドの実行があったほうがいいです。  
　　しかし、完璧な質問をするのは難しいと思います。  

　　ある程度の質問がまとまったら、投稿しちゃってください。  
  
# 回答をする人へのお願い

　まず、質問に対し、調査回答をいただきありがとうございます。  

　コミュニティから見返りはないですが、  
　そんな中でも初学者を助けようとするあなたの善意はうれしい限りです！  

　そんな善意にお願いをするようで恐縮ですが、  
　以下を気を付けてもらえると私たちはもっともっとうれしいです！  

* できる限り優しい言葉使いをしてください。  
* 理由も添えて回答するともっと親切かもしれません。  


　具体的に考えてみましょう。  
 
　よくない例  
```
【質問】
　　Squid で WEBサーバを構築したい。  
```

```
【回答】
　　無理、あきらめてください。  
```

　質問に突っ込みたくなる気持ちもわかりますが、少し改善してみましょう。

　上記例を修正した例  
```
【質問】  
　　Squid で WEBサーバを構築したい。  
```

```
【回答】  
　　結論から言うとできません。  
　　SQUID はプロキシを提供するOSSです。  
　　WEB の世界で利用する OSS ですが、WEB サーバとして利用することはできません。  
　　＊プロキシサーバが具体的に何をするかは調べてみてください  

　　WEB サーバとして利用する OSS はapache や NGINX が多いです。  
　　そちらを利用することを検討してください。  
```

言っていることは「無理だから、あきらめて」ですが、印象が大きく異なると思います。  

　1. なぜできないか理由を説明している  
　　SQUID はプロキシを提供するOSSです。  
　　WEB の世界で利用する OSS ですが、WEB サーバとして利用することはできません。  

　2. 質問者に考えてほしい部分を明示的に言っている。  
　　＊プロキシサーバが具体的に何をするかは調べてみてください。  
　　そちらを利用することを検討してください。  


　　理由を言う、相手に考えてほしい部分を明示的に言うだけでも全然印象が違うものです。  
　　コミュニティに協力いただき、回答をいただけるだけで非常にうれしいですが  
　　もうひと工夫いただけたならば、もっともっと嬉しいです！  
