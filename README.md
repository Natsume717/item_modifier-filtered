# item_modifier-filtered
item_modifierの1項目であるfilteredに関するサンプルになります。

~詳しくはブログ記事『[]()』を参考にしてください。~<br>
現在執筆中

<h3>概要</h3>
アイテムの条件を指示し、適切であった場合にitem_modifierを適用します。<br>
itemコマンドで行う場合には、対象となるアイテムが適切かどうか。<br>
ルートテーブルの場合には、ドロップするアイテムが適切かどうかを確認されます。

<h3>使い方</h3>

データパック導入後、ワールドに入り```/reload```と入力し実行してください。

手元にはダイヤモンドやラピスラズリ、ネザライトの剣とスポーンエッグが付与されます。

鉱石類は手に持った状態でitemコマンドを実行してください。<br>
ダイヤモンドを1個だけ持っていると、名前が変更されるようにしています。<br>
※filteredでset_nameを呼び出しています。

コマンドは、以下の通り。

```copy
/item modify entity @s weapon.mainhand sample:filtered
```

---

また、タラとサケのドロップアイテムをエメラルドに変更してます。

1つだけドロップする場合にはitemコマンドのときと同様に名前が変更されるようにしているものと、2つドロップする場合に変更されるようにしている2通りがあります。

そのため、タラからドロップするエメラルドは名前が変更されており、サケからドロップするエメラルドはitem_modifierが設定されているにもかかわらず変化がありません。
