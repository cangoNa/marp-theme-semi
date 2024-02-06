---
marp: true
theme: semib
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

> block

---
<!-- footer:  ○○研究室 -->

# 見出しは h1

- 改ページは水平線を使用 `---`
- 本文箇条書きはこんな感じでどんどんどんどん長く書いてもとしっかり折り返しもできる
  - 入れ子はこんな感じ
    - さらに入れ子
      - さらに入れ子
        1. ナンバリングありの入れ子
- 脚注は academic[1] を参考に

1. a
    1. あああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああああ
        1. a

---

- a
  1. a

<br>

- 縦の空白は`<br>`、横の空白は&emsp;`&emsp;`、&ensp;`&ensp;`、&nbsp;`&nbsp;`で調整

> [1]  ここに脚注 [academic のリンクはこちら](https://github.com/kaisugi/marp-theme-academic) ←　強調の色も academic より``

---

# コードブロック

- シンタックスハイライト[2]

```c
#include <stdio.h>
int main(){
  printf("test\n");
  return 0;
}
```

```txt
```

- diff もできる

```diff
int main(){
-   printf("hello world\n");
+   puts("hello world"); 
```

- これはインライン → `test` 後ろに文字を記入

> [2] [シンタックスハイライトに対応している言語一覧](https://github.com/rouge-ruby/rouge/wiki/List-of-supported-languages-and-lexers)
> `test`

---

<!-- _header: 見出しがながくなると折り返しはこんな感じになるので、背景画像は非推奨-->
<!-- _class: hh -->

<br>

# ヘッダをタイトル扱いし、h1 の下線は無効化する

→背景に画像があってもアンダーラインを一本引<br>&emsp;く

1. ナンバリングありの箇条書き
     1. 入れ子はこんな感じ
2. ヘッダが折り返されると本文と被るなど、hh はかなり不便な<br>クラス
3. 右に画像を貼ってもボーダーが途切れないので、どうしてもと<br>いう時だけ使用

![bg right:20% contain](./images/black.png)

---

<!-- _header: ヘッダありでタイトルは h1 -->
<!-- _class: withheader -->
# h1 なら見出しがどれほど長くなろうと、下線は一番下についてくれる

- # 箇条書きにも h1 を適用できる
- ## h2 でも
- ##### **h5 でも可能で、もちろん強調も可能**

> - 1&ensp;:  Hideki EIRAKU ：BitVisor/Code/Commit [92bf88]，SourceForge， 入手先 <https://sourceforge.net/p/bitvisor/code/ci/92bf883b3609c3a5de03c98a4d711d178a81e872/> (参照 2023-02-20) ．

---

# その他いろいろ

## &emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;$\Downarrow$
###### h6 は囲み線ありの中央ぞろえ！ <br> 矢印も荒業で中央寄せ

<br>

##### 出典を箇条書きにする

- 連番が一桁の場合はスペースと空白で調整
- 箇条書きのシンボルはアスタリスク

> - 1 :&nbsp; 箇条書きをどんどんながくするながくするながくするどんどんながくするながくするながくする
> - 10: 箇条書きをどんどんながくするながくするながくするどんどんながくするながくするながくする
> 下にくっつけるとインデントされる
> 
> 一行開けると大丈夫

---
<!-- _class: table-as-box mintable -->

##### 表は横並び可能で、見出しも消せる

|左|A|
|---|---|
|aaaaa|b|
|c|d|
|e|f|

|中央|A|
|:---:|---|
|aaaaa|b|
|c|d|

##### 画像と文字の位置関係は面倒

- `![w:100px right](./images/black.png)`で、右下に画像を挿入![w:100px right](./images/black.png)
- 下の文字が長くなると、上で定義した画像と被る可能性がある。こんなふうになる
- ![left w:100px](./images/black.png) `![left w:100px](./images/black.png)` で左寄せ
- 中央寄せなら`![w:100 center](./images/black.png)`![w:100 center](./images/black.png)

---
<!-- _class: withheader -->
