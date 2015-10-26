# csv_to_markdonw
CSVで書かれた以下のような２次元配列が与えられたものとする。
clojure版配列
```clojure
(def data [
           ["見出し１" "見出し２" "見出し３"]
           ["11" "12" "13"]
           ["21" "22" "23"]
           ["31" "32" "33"]
           ])
```
これを以下のようなMarkdown方式のテキストに変換してください。
```
|見出し１|見出し２|見出し３|
|:-:|:-:|:-:|
|11|12|13|
|21|22|23|
|31|32|33|
```
見出し数（列数）は可変、行数も可変と３行３列とは限らず可変とする。
１行目が見出しとするかいなかはオプションで決められるものとする。
