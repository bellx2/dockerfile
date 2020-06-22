# Jessie + gcc9 Image

テスト用です。

dist-upgradeせずにgcc-9.1.0のバイナリー追加していまいます。
VSCodeのExtensionを利用するためのモジュールです。

/opt/gcc-9.1.0/
cp -R /opt/gcc-9.1.0/lib/* /usr/lib/arm-linux-gnueabihf/

## テストフレームワーク
https://github.com/bats-core/bats-core

doc
https://github.com/bats-core/bats-core/blob/v1.2.0/README.md

## 注意

+ 純正jessieでないので、コンパイル後の動作確認注意

## 参考

バイナリーインストールに変更した方が良い気がする
https://solarianprogrammer.com/2017/12/08/raspberry-pi-raspbian-install-gcc-compile-cpp-17-programs/
