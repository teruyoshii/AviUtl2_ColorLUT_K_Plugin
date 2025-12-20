# ColorLUT_K

![GitHub License](https://img.shields.io/github/license/korarei/AviUtl2_ColorLUT_K_Plugin)
![GitHub Last commit](https://img.shields.io/github/last-commit/korarei/AviUtl2_ColorLUT_K_Plugin)
![GitHub Downloads](https://img.shields.io/github/downloads/korarei/AviUtl2_ColorLUT_K_Plugin/total)
![GitHub Release](https://img.shields.io/github/v/release/korarei/AviUtl2_ColorLUT_K_Plugin)

AviUtl2にLUTファイルを扱えるようにするプラグイン

[ダウンロードはこちらから](https://github.com/korarei/AviUtl2_ColorLUT_K_Plugin/releases)

## 動作確認

- [AviUtl ExEdit2 beta25](https://spring-fragrance.mints.ne.jp/aviutl/)

> [!CAUTION]
> beta25以降必須．

## 導入・削除・更新

初期配置場所は`色調整`である．

`オブジェクト追加メニューの設定`から`ラベル`を変更することで任意の場所へ移動可能．

### 導入

下記のいずれかの方法で導入可能．

- 同梱の`*.aux2`をAviUtl2にD&D．

- 同梱の`*.aux2`を`%ProgramData%`内の`aviutl2\Plugin`フォルダに入れる．

- 同梱の`*.aux2`を`aviutl2.exe`と同じ階層内の`data\Plugin`フォルダに入れる．

### 削除

- 導入したものを削除する．

### 更新

- 導入したものを上書きする．

## 使い方

Cube LUT Specification Version 1.0に準拠したLUTファイル (.cube) を読み込み，画像の色を変える．

読み込んだLUTはファイルパスをキーとしてキャッシュを取るので，LUTに変更があった場合は`Reload`を有効にするか本体の`キャッシュを破棄`をクリックして再読み込みを行うこと．

本体の`キャッシュを破棄`を行った場合，すべてのLUTファイルに対してキャッシュ破棄を行う．

### パラメータ

#### LUT File

LUTファイルを指定する．

#### Reload

`LUT File`で指定したLUTを再読み込みする．

#### Opacity

適用度合．

##  ビルド方法

`.github/workflows`内の`releaser.yml`に記載．

## License
LICENSEファイルに記載．

## Credits

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

## Change Log

- **v1.0.0**
  - Release
