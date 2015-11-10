# xkb-data

## What is this?

This is data for xkb to provide Japanese keyboard layout and US keyboard layout with ESDF keys and Japanese specific keys, and Hungarian keyboard layout with Japanese specific keys. <LSGT> key may work as left Ctrl key.

This is one of options for using ESDF keys. You can use ESDF keys, Home/End, PgUp/PgDn and BS with pressing AltGr without your hand moving from home position.

Additionally, you can use some Japanese specific keys, Hiragana key, Eisu key, Henkan key and Muhenkan key as well, even if your keyboard is non-Japanese keyboard. If you set configures for IM properly, you can choose keyboard layouts and letter type easily.

Unfortunately, this Hungarian keyboard layout does not have ESDF keys. Technically, I can assign ESDF keys, but I don't want to disable to input brackets, backslash and bar.


## Original files

You can get original files from Debian repository. Of course, you can get other repositories.

```
$ apt-get source xkb-data
```

## Modified files

- symbols/hu
- symbols/jp
- symbols/us
- rules/evdev.xml

## Added file

- symbols/jp_alt

## Install

```
$ sudo cp symbols/hu /usr/share/X11/xkb/symbols/hu
$ sudo cp symbols/jp /usr/share/X11/xkb/symbols/jp
$ sudo cp symbols/jp_alt /usr/share/X11/xkb/symbols/jp_alt
$ sudo cp symbols/us /usr/share/X11/xkb/symbols/us
$ sudo cp rules/evdev.xml /usr/share/X11/xkb/rules/evdev.xml
```

## Configure

### Fcitx

1. Select "Configure Input Method" from Fcitx panel.
2. Add "Keyboard English (US) - English (ESDF keys and Japanese specific keys)" to current input methods.
3. Add "Keyboard Hungarian (HU) - Hungarian (standard with Japanese specific keys)" to current input methods. (if you want to use Hungarian keyboard layout)

### KDE

1. Open KDE System Settings.
2. Click Input Device.
3. Select Keyboard -> Layout.
4. Add "US ESDF keys and Japanese specific keys". "US" is map name, and "ESDF keys and Japanese specific keys" is variant.
5. Add "HU standard with Japanese specific keys". (if you want to use Hungarian keyboard layout)

## How to use

AltGr + q : Backspace

AltGr + w : PgUp

AltGr + e : move up

AltGr + r : PgDn

AltGr + a : Home

AltGr + s : move left

AltGr + d : move down

AltGr + f : move right

AltGr + g : end

AltGr + h : Muhenkan

AltGr + j : Hiragana

AltGr + k : Eisu

AltGr + l : Henkan

~~AltGr + z : Hiragana~~

~~AltGr + x : Katakana~~

~~AltGr + c : Henkan~~

~~AltGr + v : Muhenkan~~

~~AltGr + b : Hangul~~

## Known problem

- Even in Hungarian keyboard layout, <LSGT> (í) key can work as ctrl key. Don't push any key quickly after push <LSGT>.

-----------
## これはなんですか？

これは日本語キーボードレイアウトや英語キーボードレイアウトにESDFキーや日本版独自のキーを追加したり、ハンガリー語キーボードレイアウトに日本語版独自のキーを追加するためのものです。<LSGT>キーをコントロールキーとして使うこともできます。

これはESDFキーを使うための選択肢の1つです。AltGrキーを押すことで、手をホームボジションに置いたまま、 ESDFキーの他にHome/EndやPgUp/Dn、バックスペースを押すことができます。

また、日本語版独自のキーである、ひらがなキーや英数キー、変換キー、無変換キーを非日本語キーボードでも打つことができます。IMを適切にセットすることで、キーボードレイアウトの切り替えや入力文字種の選択を簡単に行なえます。

残念ながら、ハンガリー語キーボードレイアウトではESDFキーを使うことはできません。技術的には可能ですが、角括弧やバックスラッシュ、バーを打てなくなるようにはしたくないからです。

## オリジナルファイル

Debianのリポジトリからダウンロードできます。もちろん、他のリポジトリからも入手できます。

```
$ apt-get source xkb-data
```

## 変更を加えたファイル

- symbols/hu
- symbols/jp
- symbols/us
- rules/evdev.xlm

## 追加したファイル

- symbols/jp_alt

## インストール

```
$ sudo cp symbols/hu /usr/share/X11/xkb/symbols/hu
$ sudo cp symbols/jp /usr/share/X11/xkb/symbols/jp
$ sudo cp symbols/jp_alt /usr/share/X11/xkb/symbols/jp_alt
$ sudo cp symbols/us /usr/share/X11/xkb/symbols/us
$ sudo cp rules/evdev.xml /usr/share/X11/xkb/rules/evdev.xml
```

## 設定

### Fcitx

1. Fcitxのパネルから"Configure Input Method"を選択します。
2. 現在の入力方法に"Keyboard English (US) - English (ESDF keys and Japanese specific keys)"を追加します。
3. 現在の入力方法に"Keyboard Hungarian (HU) - Hungarian (standard with Japanese specific keys)"を追加します。（ハンガリー語キーボードレイアウトが必要でなければ、これは不要です）

### KDE

1. KDEシステム設定を開きます。
2. 入力デバイスをクリックします。
3. キーボードレイアウト→レイアウトを選択します。
4. US ESDF keys and Japanese specific keysを追加します。"US"がマップで、"ESDF keys and Japanese specific keys"がバリアントになります。
5. HU standard with Japanese specific keysを追加します。（ハンガリー語キーボードレイアウトが必要でなければ、これは不要です）

## 使い方

AltGr + q : Backspace

AltGr + w : PgUp

AltGr + e : move up

AltGr + r : PgDn

AltGr + a : Home

AltGr + s : move left

AltGr + d : move down

AltGr + f : move right

AltGr + g : end

AltGr + h : Muhenkan

AltGr + j : Hiragana

AltGr + k : Eisu

AltGr + l : Henkan

~~AltGr + z : Hiragana~~

~~AltGr + x : Katakana~~

~~AltGr + c : Henkan~~

~~AltGr + v : Muhenkan~~

~~AltGr + b : Hangul~~


## 既知の問題

- ハンガリー語キーボードレイアウトにおいても<LSGT> (í) キーがCtrlキーとして動作してしまいます。<LSGT>を押した後は、他のキーを素早く押さないようにしてください。