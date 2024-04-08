# setup_mac
Mac設定用のAnsible

```sh
curl -H 'Cache-Control: no-cache' -sfSL https://raw.githubusercontent.com/ito0804takuya/setup_mac/main/setup.sh | sh
```
（もちろん`git clone`不要。）
（キャッシュが効いて、git pushした内容が反映されずに実行されることがたまにあったのでno-cache）

# 修飾キーの動作を変更
https://support.apple.com/ja-jp/guide/mac-help/mchlp1011/mac
これは、手動でやらないといけないっぽい。
- CapsLock を Control へ。
- Control を Command へ。

# Cursorの設定
- Auto Save: afterDelay

# 参考
https://zenn.dev/shinyaoguri/articles/5caeeeea21b0c2

localのprojects/ansible_mac_setupも参照。

## Ansibleで使えるモジュールのリファレンス
https://docs.ansible.com/ansible/2.9_ja/modules/list_of_all_modules.html

### MacOSの設定値リファレンス
https://macos-defaults.com
https://developer.apple.com/documentation/devicemanagement/dock

## mas（AppleStore）で入れるアプリのIDの調べ方
```sh
mas search アプリ名
```
