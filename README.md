# Fate/EXTRA Japanese HD Font
Fate/EXTRA PPSSPP用のフォントテクスチャ

オリジナルのフォントを源暎ラテミンやしっぽり明朝、Bizin Gothicに置き換えました。

4×PSP向け


## 使い方
インストールする前にPPSSPP側の設定を以下のように変更してください。

* レンダリング解像度を[自動(1:1)]または[4×PSP]に変更する

`グラフィック > レンダリング解像度 > [自動(1:1)]または[4×PSP]`

* テクスチャスケーリングをOFFにする。

`グラフィック > テクスチャスケーリング > アップスケールのレベル > [OFF]`

* テクスチャパックを利用可能にする。

`ツール > 開発者向けツール > テクスチャを置き換える [ON]`


解凍したzipファイルの中身を`PPSSPP/memstick/PSP/TEXTURES/%GAME_ID%`に配置する。
日本版Fate/EXTRAのゲームIDは`NPJH50247`です。

（このような構成になるように）

```
.
└── NPJH50247/
    ├── Fonts
    └── textures.ini
```

## 他のテクスチャパックと併用する方法
HD Fontは他のテクスチャパックに後付けする形で同時に利用することができます。

事前に併用したいテクスチャパックのインストールを済ませてください。

![NPJH50247_00017](https://github.com/user-attachments/assets/6663c42e-970e-4c20-a767-b9c132de3ab5)
（組み合わせ例です。HD Fontにはフォント以外は入っていません。）

併用するテクスチャパックの`hash =`の種類によって方法が異なります。

* `hash = quick`の場合

以下の内容をコピーし、併用するテクスチャパックの`textures.ini`の`#Fonts`にペーストして上書きする。（`#Fonts`が存在しない場合は`[hashes]`より下にペーストする。）
```
#region --- Fonts ---
00000000693a49fe148ac97f = Fonts/Font_01.png
00000000693a49fe0cb57ffa = Fonts/Font_02.png
00000000693a49feecab6a80 = Fonts/Font_03.png
00000000693a49fee84661df = Fonts/Font_04.png
00000000693a49fe53c2c1a8 = Fonts/Font_05.png
00000000693a49fe13401393 = Fonts/Font_06.png
00000000693a49fef7f45402 = Fonts/Font_07.png
00000000693a49fe49159703 = Fonts/Font_08.png
00000000693a49fefcd21d61 = Fonts/Font_09.png
00000000693a49fe8819c35b = Fonts/Font_10.png
00000000693a49fe74aa4ebe = Fonts/Font_11.png
00000000693a46f156e049a5 = Fonts/Font_12.png
00000000693a46f1723d9a07 = Fonts/Font_13.png
00000000693a49fecbc2cc8b = Fonts/Font_14.png
00000000693a49fe47c9e47f = Fonts/Font_15.png
00000000693a49fe3e39ff0c = Fonts/Font_16.png
#endregion
```

HD Fontの`Fonts`フォルダを併用するテクスチャパックの`textures.ini`があるフォルダにコピーする。

（このような構成になるように）


```
.
└── NPJH50247/
    ├── （その他いろいろ）
    ├── Fonts
    └── textures.ini
```

* `hash = xxh64`の場合

以下の内容をコピーし、併用するテクスチャパックの`textures.ini`の`#Fonts`にペーストして上書きする。（`#Fonts`が存在しない場合は`[hashes]`より下にペーストする。）
```
#region --- Fonts ---
00000000693a46f1710960f9 = Fonts/Font_13.png
00000000693a46f1f8ef1c56 = Fonts/Font_12.png
00000000693a49fe044d3917 = Fonts/Font_03.png
00000000693a49fe1abccc37 = Fonts/Font_02.png
00000000693a49fe3ac3ffc4 = Fonts/Font_09.png
00000000693a49fe3bd01903 = Fonts/Font_11.png
00000000693a49fe745b66d7 = Fonts/Font_08.png
00000000693a49fe85e390d7 = Fonts/Font_06.png
00000000693a49febd97f542 = Fonts/Font_05.png
00000000693a49fec0096bd4 = Fonts/Font_10.png
00000000693a49fecaedf2d9 = Fonts/Font_07.png
00000000693a49feddabeeb3 = Fonts/Font_04.png
00000000693a49fedeb20577 = Fonts/Font_01.png
00000000693a49fe3b27c79e = Fonts/Font_15.png
00000000693a49fed7a2f7cc = Fonts/Font_14.png
00000000693a49fe76371a4f = Fonts/Font_16.png
#endregion
```

HD Fontの`Fonts`フォルダを併用するテクスチャパックの`textures.ini`があるフォルダにコピーする。

（このような構成になるように）

```
.
└── NPJH50247/
    ├── （その他いろいろ）
    ├── Fonts
    └── textures.ini
```
## プレビュー

![NPJH50247_00016](https://github.com/user-attachments/assets/8e048b59-a725-45d9-8ff3-d036be5187ee)


![NPJH50247_00000](https://github.com/user-attachments/assets/b2b89bdb-5a01-4eac-8d29-5b2bdd9ba7a5)


![NPJH50247_00018](https://github.com/user-attachments/assets/e2b543cc-c8fb-4544-a49d-ae73d7a73cce)


![NPJH50247_00003](https://github.com/user-attachments/assets/542cdb97-38c9-4fee-894a-d997d10d1e06)


## 使用したフォント
* 本文・・・「源暎ラテミン V2」(https://okoneya.jp/font/genei-latin.html)

   Licensed under SIL Open Font License 1.1 (http://scripts.sil.org/OFL)
  
* ポエム・・・「しっぽり明朝 OTF 太字」(https://fontdasu.com/shippori-mincho/)

  Licensed under SIL Open Font License 1.1 (http://scripts.sil.org/OFL)
  
* コードキャスト・・・「Bizin Gothic」(https://github.com/yuru7/bizin-gothic)

  Licensed under SIL Open Font License 1.1 (http://scripts.sil.org/OFL)



## AIの使用
元のテクスチャを拡大する際、AIによるアップスケールを使用しました。その後大部分の文字は置き換えられましたが、一部のアイコンや未使用文字と思われるものは、
置き換えずそのまま使用しています。



## 更新履歴
v1.01 いくつかのアイコンの影を修正。
