folk 手順
https://tech.qookie.jp/posts/use-npm-package-github-fork/

<修正内容>
block/index.ts を修正。
block にタイムスタンプが付与されるようにした。
また、同じく div タグの id にもタイムスタンプを付与。これにて getElementByID でタイムスタンプ指定で対象の div を特定できる。
その子要素が contentseditable となる。

<delete method>
api/blocks.tsを修正
caret positionを設定しないdeleteWithoutCaretSet を追加。
他の人の修正でcaret positionが変更されてしまわないように、deleteWithoutCaretSetを呼び出す。
