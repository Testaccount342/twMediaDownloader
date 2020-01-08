Twitter Media Downloader - Reverse engineering version for studying. All credit to Furyutei here on Github.
================================================

- License: The MIT license  
- Copyright (c) 2016 風柳(furyu)  
- Target/Supported browsers: Google Chrome、Firefox

A script designed for Twitter(https://twitter.com/) user timeline scraping of full size media. 
Note of Testaccount342: I only know C. I intend to learn JS as I go through this program, just ignore me for now.

■ Way of use
---
[Web 版公式 Twitter](https://twitter.com/) 上で、ユーザータイムラインや検索タイムラインを開くと、「メディア↓」のようなリンクが挿入される。  
![下向き矢印のリンク](https://cdn-ak.f.st-hatena.com/images/fotolife/f/furyu-tei/20160723/20160723224518.jpg)  

これをクリックするとダイアログが表示されるので、[開始]ボタンをクリックすると、原寸画像/動画の ZIP 化が開始される。  
※ ZIP 化の進捗は、下部にログ出力される。  
![ダイアログ](https://cdn-ak2.f.st-hatena.com/images/fotolife/f/furyu-tei/20171029/20171029090641.png)  

ZIP 化が完了するか、もしくは[停止]を押すと、対象となる画像/動画ファイルをまとめた ZIP ファイルがダウンロードされる。  
※ ログの内容も ZIP の中に保存される。

必要に応じて、保存対象となるツイートの Tweet ID 範囲、および、ツイートの制限数を指定可能。  
※デフォルト(範囲空白)の状態では、Tweet ID 範囲は全てで、ツイートの制限数にのみ制限される。  

また、各メディア付ツイートにもダウンロード用のリンクが追加され、個別にダウンロードすることも可能。  
※ Chrome 拡張機能の場合、この機能は ON/OFF できる。  


■ External libraries (?)
---
- [jQuery](https://jquery.com/), [jquery/jquery: jQuery JavaScript Library](https://github.com/jquery/jquery)  
    [License | jQuery Foundation](https://jquery.org/license/)  
    [The MIT License](https://tldrlegal.com/license/mit-license)  

- [JSZip](https://stuk.github.io/jszip/)  
    Copyright (c) 2009-2014 Stuart Knightley, David Duponchel, Franz Buchinger, António Afonso  
    [The MIT License](https://github.com/Stuk/jszip/blob/master/LICENSE.markdown)  

- [MikeMcl/decimal.js: An arbitrary-precision Decimal type for JavaScript](https://github.com/MikeMcl/decimal.js)  
    Copyright (c) 2016, 2017 Michael Mclaughlin  
    [The MIT Licence](https://github.com/MikeMcl/decimal.js/blob/master/LICENCE.md)  

- [lambtron/chrome-extension-twitter-oauth-example: Chrome Extension Twitter Oauth Example](https://github.com/lambtron/chrome-extension-twitter-oauth-example)  
    Copyright (c) 2017 Andy Jiang  
    [The MIT Licence](https://github.com/lambtron/chrome-extension-twitter-oauth-example/blob/master/LICENSE)  

- [sha1.js](http://pajhome.org.uk/crypt/md5/sha1.html)  
    Copyright Paul Johnston 2000 - 2009
    The BSD License

- [oauth.js](http://code.google.com/p/oauth/source/browse/code/javascript/oauth.js)(^1)  
    Copyright 2008 Netflix, Inc.
    [The Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)  
    (^1) archived: [oauth.js](https://web.archive.org/web/20130921042751/http://code.google.com/p/oauth/source/browse/code/javascript/oauth.js)  

- [jsTwitterOAuth/twitter-api.js](https://github.com/furyutei/jsTwitterOAuth/blob/master/src/js/twitter-oauth/twitter-api.js)  
    Copyright (c) 2018 風柳 (furyu)  
    [MIT License](https://github.com/furyutei/jsTwitterOAuth/blob/master/LICENSE)   
