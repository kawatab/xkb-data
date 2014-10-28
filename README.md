# xkb-data

## Original files
## オリジナルファイル

We can get original files from Debian repository. Of course, you can get other repositories.
Debianのリポジトリからダウンロードできます。もちろん、他のリポジトリからも入手できます。

```
$ apt-get source xkb-data
```

## Modified file
## 変更を加えたファイル

- symbols/us

## Install
## インストール

```
$ sudo cp symbols/us /usr/share/X11/xkb/symbols/us
```

## Configure
## 設定

### Fcitx

1. Select "Configure Input Method" from Fcitx panel.
2. Add "Keyboard English (US) - English (international AltGr Dead keys)" to current input methods.

1. Fcitxのパネルから"Configure Input Method"を選択します。
2. 現在の入力方法に"Keyboard English (US) - English (international AltGr Dead keys)"を追加します。

### KDE
1. Open KDE System Settings.
2. Click Input Device.
3. Select Keyboard -> Layout.
4. Add "US International AltGr Dead keys". "US" is map name, and "international AltGr Dead keys" is variant.

1. KDEシステム設定を開きます。
2. 入力デバイスをクリックします。
3. キーボードレイアウト→レイアウトを選択します。
4. US International AltGr Dead keyを追加します。"US"がマップで、"international AltGr Dead keys"がバリアントになります。

## How to use
## 使い方

AltGr + q : Backspace
AltGr + w : PgUp
AltGr + e : move up
AltGr + r : PgDn
AltGr + a : Home
AltGr + s : move left
AltGr + d : move down
AltGr + f : move right
AltGr + z : Hiragana
AltGr + x : Katakana
AltGr + c : Henkan
AltGr + v : Muhenkan
AltGr + b : Hangul