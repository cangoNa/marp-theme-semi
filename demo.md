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
<!-- _paginate: false -->

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
- 脚注は academic$^{*1}$ を参考に
- 画像がないなら h1 を見出しにすることを推奨
  1. 数字の入れ子

> *1: ここに脚注 [academic のリンクはこちら](https://github.com/kaisugi/marp-theme-academic) ←　強調の色も academic より
>
> 1. 箇条書き
> 1. 箇条書き2

---

# その他

## &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;$\Downarrow$
###### h6 は囲み線ありの中央ぞろえ！ <br> 矢印も荒業で中央寄せ

> - 1&nbsp;: 箇条書きをどんどんながくするながくするながくするどんどんながくするながくするながくする
> - 10: 箇条書きをどんどんながくするながくするながくするどんどんながくするながくするながくする
> a

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

- これはインライン → `test` 後ろも文字
  - 入れ子インライン → `test`

---
<!-- header: その他いろいろ -->
<!-- _class: withheaderh -->

|a|A|
|---|---|
|aaaaa|b|
|c|d|
|e|f|
|g|h|

|a|A|
|:---:|---|
|aaaaa|b|
|c|d|
|e|f|

- 文字
- ここに文字 ![w:100px right](./images/black.png)

- 文字がどんどんながくなるながくなるながくなるながくなるながくなるながくなるながくなるながくなるながくなる

![right w:100px](./images/black.png)

---
<!-- header: 未解決 -->
<!-- _class: withheader -->

# キャプションをつけたい

![w:100px center](./images/black.png "fig:")

|a|b|
|---|---|
|a|b|
|表の横幅を広くしてもキャプションはうまく行ってほしい|A|

---

> 1. 
> 1. 
> 1. 
> 1. 
> 1. 
> 1. 
> 1. 
> 1. 
> 1. 内容
> 1.  内容
> 1. 
