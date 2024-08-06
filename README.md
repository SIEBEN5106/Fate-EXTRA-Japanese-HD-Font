# Fate/EXTRA Japanese HD Font
Fate/EXTRA PPSSPP用のフォントテクスチャ
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

## 他のテクスチャパックと併用する方法
HD Fontは他のテクスチャパックに後付けする形で同時に利用することができます。

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

before
![NPJH50247_00001](https://github.com/user-attachments/assets/90c10a52-f1e2-4e0e-a222-9997a4d6b281)

after
![NPJH50247_00000](https://github.com/user-attachments/assets/b2b89bdb-5a01-4eac-8d29-5b2bdd9ba7a5)

before
![NPJH50247_00006](https://github.com/user-attachments/assets/c1bf3cd0-36ea-44ee-ab4f-f665389e99cd)

after
![NPJH50247_00007](https://github.com/user-attachments/assets/37e3643d-4249-4121-887e-f02e74e61410)

before
![NPJH50247_00009](https://github.com/user-attachments/assets/3fe6d3db-e43c-42c7-9470-a1e837f36739)

after
![NPJH50247_00008](https://github.com/user-attachments/assets/4cb6e56b-9f30-4ee5-a5cf-a400a67d14d2)

before
![NPJH50247_00012](https://github.com/user-attachments/assets/c1f3833e-4bf6-46ea-923a-3e5ff71f6ff2)

after
![NPJH50247_00013](https://github.com/user-attachments/assets/55ee9bae-3694-42d2-85d9-61f9eb7dcf84)

before
![NPJH50247_00014](https://github.com/user-attachments/assets/0e31fc6d-0a69-4ac0-846b-ed8c6695faf8)

after
![NPJH50247_00003](https://github.com/user-attachments/assets/542cdb97-38c9-4fee-894a-d997d10d1e06)
