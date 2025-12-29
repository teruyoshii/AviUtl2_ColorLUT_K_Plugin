
# ColorLUT_K改

https://github.com/user-attachments/assets/9dfe4d02-296a-4e7b-9e62-dbf66e8b673a

AviUtl2でLUTファイルを扱えるようにする ColorLUT_Kへのインターフェーススクリプト

LUTの切り替えをトラックバーから行えるようになります

[ColorLUT_Kのダウンロードはこちらから](https://github.com/korarei/AviUtl2_ColorLUT_K_Plugin/releases)

## 動作確認

- [AviUtl ExEdit2 beta26](https://spring-fragrance.mints.ne.jp/aviutl/)

> [!CAUTION]
> beta26以降必須．

## 導入・削除・更新

初期配置場所は`色調整`である．

`オブジェクト追加メニューの設定`から`ラベル`を変更することで任意の場所へ移動可能．

### 導入

1. [ColorLUT_K](https://github.com/korarei/AviUtl2_ColorLUT_K_Plugin)を本体のページのreadmeに従って導入する.
2. ColorLUT_K改.anm2とLUT(フォルダー)を`アプリケーションフォルダ > Script`に直置きする.
   (Scriptの中の子フォルダに配置すると正しく動作しないので注意)
3. 使いたいLUTファイル(.cube)を全て`アプリケーションフォルダ > Script > LUT`に入れる

### 削除

- 導入したものを削除する．

### 更新

- 導入したものを上書きする．

## 使い方

フォーク元のColorLUT_Kと同様に, 
Cube LUT Specification Version 1.0に準拠したLUTファイル (.cube) を読み込み，画像の色を変える.

「基準LUTファイル」で指定したLUTファイルと同じ階層にあるLUTファイルのうち, 辞書順で「ﾌｧｲﾙ選択」トラックバーの数値分だけ進んだところにあるLUTファイルを適用する.

LUTファイルを更新した場合は, 基準LUTファイルを再度適当な.cubeファイルに変更することでリストを再生成できる.

※「基準LUTファイル」に任意のLUTファイルを登録した状態でオブジェクト設定ウィンドウのColorLUT_K改の部分を右クリックし, 「設定を保存」から「現在の設定を初期値にする」ことをおすすめします。

### パラメータ

#### 基準LUTファイル

LUTファイルを指定する．

#### ﾌｧｲﾙ選択

「基準LUTファイル」で指定したLUTファイルと同じ階層にあるLUTファイルのうち, 辞書順で「ﾌｧｲﾙ選択」トラックバーの数値分だけ進んだところにあるLUTファイルを適用する.
トラックバーの数値がLUTフォルダの個数よりも多い場合は剰余をとってループする.

#### Opacity

適用度合．

## License
LICENSEファイルに記載．

## Credits

### AviUtl2_ColorLUT_K_Plugin

https://github.com/korarei/AviUtl2_ColorLUT_K_Plugin

### AviUtl ExEdit2 Plugin SDK

https://spring-fragrance.mints.ne.jp/aviutl/

---

The MIT License

Copyright (c) 2025 Kenkun

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
