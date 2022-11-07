---
marp: true
theme: semi
paginate: true
math: katex
# size: 16:9
size: 4:3
---

<!-- _class: lead -->
<!-- _footer: yy/mm/dd <br> ○○研究室 -->

# Marpでつくる<br>ゼミ用発表スライド

<br>
<br>

**作成者**
所属

---

<!-- _header: 見出しがどんどんながくなるながくなる -->
<!-- footer:  ○○研究室 -->
<!-- _class: hh -->

# ヘッダをタイトルにできる

普通にテキスト

1. ナンバリングありの箇条書き
     1. こんな感じ
2. ヘッダが折り返されると本文と被る
3. 右に画像を貼ってもボーダーが途切れないけど、タイトルは乱れる
4. 実際に画像を貼りたいなら、白を貼り付けて領域確保 → スライドソフトを開いて自分で貼る

![bg right:20% contain](./images/black.png)

---

<!-- _header: ヘッダありでタイトルは h1 -->
<!-- _class: withheader -->
# こちらもどんどんながくなるながくなるながくなるながくなるながくなるながくなる

普通にテキスト

- 本文箇条書きはこんな感じでどんどん長く書くとしっかり折り返しもできる
  - 入れ子はこんな感じ
    1. さらに入れ子
- 脚注は academic$[1]$ を参考に
- 画像がないなら h1 を見出しにすることを推奨
  1. 数字の入れ子

> ここに脚注 [academic のリンクはこちら](https://github.com/kaisugi/marp-theme-academic) ←　強調の色も academic より

---

# その他

## &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;$\Downarrow$
###### h6 は囲み線ありの中央ぞろえ！ <br> 矢印も荒業で中央寄せ

---

- シンタックスハイライト

```c
#include <stdio.h>
int main(){
  printf("test\n");
  return 0;
}
```

- diff もできる

*ソースコード１　キャプション*

```diff
int main(){
-   printf("hello world\n");
+   puts("hello world"); 
```

- これはインライン → `test`

---
<!-- header: 解決済み -->
<!-- _class: withheaderh -->

- ヘッダありで見出しなしの時、本文が上に行き過ぎる問題をなんとかしないといけない。とくに16:9 の時とかページ番号に直撃する

|a|A|
|:---:|---|
|aaaaa|b|
|c|d|
|e|f|
|g|h|

---
<!-- header: 未解決 -->
<!-- _class: withheader -->

# キャプションをつけたい

![w:100px center](./images/black.png)

|表の横幅を広くしてもキャプションはうまく行ってほしい|A|
|---|---|
|a|b|
