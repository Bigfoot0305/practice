いっぱいあるみたいだけれども、有名どこだけでも。

## Aレコード
Addressレコード　ドメインをIPアドレスに変換する。
一番オーソドックスなタイプ
```
hp-bigfoot.jp. IN A 192.168.1.5
```
## MXレコード
Mail eXchangeレコード
メールの@以下を決めているのはここ。
10 の部分で優先度が決められる。
```
hp-bigfoot.jp. IN MX 10 mail.hp-bigfoot.jp.
```
この場合、**@hp-bigfoot.jp**のアドレスは、
**mail.hp-bigfoot.jp**ドメインが処理してくれる。


## CNAMEレコード
Canonical NAMEレコード
ドメインを別のドメインに変換する。
www付けても同じアドレスへ繋げるよ。って時などに。
```
hp-bigfoot.jp. IN A 192.168.0.1
www.hp-bigfoot.jp. IN CNAME hp-bigfoot.jp.
```
