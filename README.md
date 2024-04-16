# XAMPP

## 前提条件

7-Zipがインストールされていること  
インストール方法は下記を参照

https://github.com/room202/7-zip

## インストールの手順

### ダウンロード

下記サイトからXAMPPをダウンロードする  
https://www.apachefriends.org/jp/

`その他のバージョンについては、こちらをクリックしてください`をクリック  
![](images/001.png)

`More Downloads`をクリック  
![](images/002.png)

`XAMPP Windows`をクリック  
![](images/003.png)

`8.2.12`をクリック  
![](images/004.png)

`xampp-windows-x64-8.2.12-0-VS16.zip`をクリック  
![](images/005.png)

`ダウンロード`フォルダに保存する  
![](images/007.png)

### インストール  

ダウンロードしたファイルを解凍(展開)する  
対象のファイルの上で`Shiftキーを押しながら右クリック`→`7-Zip`→`ここに展開`
![](images/008.png)

解凍(展開)されたフォルダ`xampp`を`Cドライブ(C:\)`の真下に移動  
![](images/009.png)
![](images/010.png)

`C:\xampp\setup_xampp.bat`をダブルクリックで実行する  
![](images/011.png)

`続行するには何かキーを押してください. . .`と表示されたら`Enterキー`を押す  
※この画面が閉じる  
![](images/012.png)

## 初期設定

デスクトップにショートカットキーを作る  
`C:\xampp\xampp-control.exe`を`Shiftキーを押しながら右クリック`→`送る`→`デスクトップ(ショートカットを作成)`
![](images/013.png)

デスクトップにショートカットができている事を確認する  
ショートカットができていたら、それをダブルクリックして起動する  
![](images/014.png)

`Language`画面では、そのまま`Save`をクリック  
![](images/015.png)

## 動作確認

XAMPP(XAMPPコントロールパネル)が起動する  
そのまま`Apache`と`MySQL`と書かれている横の`Start`ボタンをクリック  
![](images/016.png)

`Apache`と`MySQL`の背景が薄い緑色になれば起動成功  
![](images/017.png)

`Chrome`で下記URLにアクセスする  
http://localhost  
※URLが勝手に`http://localhost/dashboard/`になるが問題ない  
メニューにある`PHPInfo`をクリック  
![](images/018.png)


このような画面になる事を確認する  
![](images/019.png)

http://localhost  
に戻ってきて、`phpMyAdmin`をクリック  
![](images/020.png)

このような画面になる事を確認する  
![](images/021.png)

## PHPプログラムを作って動作確認

ファイルの保存先 : `C:\xampp\htdoc\php`

### PHPプログラム保存用のフォルダを作る

`C:\xampp\htdoc`フォルダの中に`php`フォルダを作る  
![](images/022.png)
![](images/023.png)

### PHPプログラムを作る 

作った`php`フォルダをVisual Studio Codeで開く  
`php`フォルダを`Shiftキーを押しながら右クリック`→`Codeで開く`  
![](images/024.png)

`index.php`ファイルを作って、下記PHPプログラムを打ち込むかコピペする  

```php
<?php
echo "Hello World";
?>
```

`Chrome`で下記URLにアクセスする  
http://localhost/php/index.php

![](images/025.png)

このような画面になればOK  
![](images/026.png)

## XAMPPの終了方法

XAMPPコントロールパネルの`Apache`と`MySQL`と書かれている横の`Stop`ボタンをクリック  
![](images/027.png)

`Apache`と`MySQL`の背景が灰色になればOK  
その後、右下の`Quit`ボタンでXAMPPを終了させる  
![](images/028.png)
