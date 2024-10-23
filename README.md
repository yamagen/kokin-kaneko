# **Kokin-Kaneko**

[![DOI](https://zenodo.org/badge/868652787.svg)](https://zenodo.org/badge/latestdoi/868652787)

## Kokinwakashu Hyoshaku dataset

"Kokinwakashu Hyoshaku" was an annotation book of "Kokinwakashu" published in 1927 by Motoomi Kaneko.
This dataset is contemporary translation sentences of the "Kokinwakashu" poems in the "Kokinwakashu Hyoshaku" book.
The dataset contains the following information for each poem:

### **Introduction**

金子元臣著『古今和歌集評釈』のうち、大意を記録したデータベース。ただし、形態素解析で処理しやすいように、現代仮名表記に改めた。著者没後70年を経過しているので、著作権上の取り扱いには問題が発生しない。

A dataset that records the general meaning of Kaneko Motoomi's Kokin Wakashū Hyōshaku.
The text has been revised to modern kana notation to facilitate morphological analysis.
As more than 70 years have passed since the author's death, there are no copyright issues with its use.

### **Data format**

Tag sets are shown as the following:

- $A|番号=管理番号。下４桁が歌番号。
- $A|number .. the last four digits is poem number indexed by Kokkataikan.
- $B|原表記=口語訳の原表記
- $B|original sentence .. the original sentence of the contemporary translation by Motoomi Kaneko.
- $C|前書=詞書、詠み手などの現代語訳
- $C|foretext, kotobagaki, the name of poet
- $D|和歌=和歌の口語訳の現代表記
- $D|poem=contemporary translation of the poem
- $E|後書=後註、その他の現代語訳
- $E|Postscript=Translation of endnotes, and other elements into modern language.
- $G|リンク=他の古今集データベースへのリンク。
- $G|link to the Kokinshu dataset
- $H|山元=山元の注
- $H|annotation by Yamamoto
- $I|かな=和歌現代語のかな書き
- $I|kana=Kana notation of contemporary translation of the poem
- $Z|日付
- $Z|date of edited of the data

### **Example**

#### kaneko.txt

<!-- kaneko.txt: 金子元臣による古今集の現代語訳 -->

Kaneko.txt is a contemporary translation of the Kokinshu by Motoomi Kaneko.

```plaintext
$A|000001
$B|年内に思ひがけず春は来たことであるわ、さてはこの同じ一年の内の昨日までを、去年といはうか、それとも今年といはうか。
$D|年内に思い掛けず春は来たことであるわ、さてはこの同じ一年の内の昨日までを、去年と言おうか、それとも今年と言おうか。
$I|ねんないにおもいがけずはるはきたことであるわ、さてはこのおなじいちねんのうちのきのうまでを、きょねんといおうか、それともことしといおうか。
$Z|2003/09/25
```

#### kokin-kaneko.db

<!-- kokin-kaneko.db: 金子元臣による古今集の現代語訳を単語データに分割し、タグ付けを施したもの。 -->

Kokin-kaneko.db is a word data of the contemporary translation of the Kokinshu by Motoomi Kaneko, tagged.

```plaintext
kaneko 0001 1 02 00 00 BG-01-1631-01-280-A 年内 ねんない 年内
kaneko 0001 3 02 00 00 BG-01-1630-01-010-A -- とし 年
kaneko 0001 3 02 00 00 BG-08-0071-01-010-A -- の の
kaneko 0001 3 02 00 00 BG-01-1770-01-030-A -- うち 内
kaneko 0001 0 61 00 00 BG-08-0061-05-010-A に に に
kaneko 0001 1 55 00 00 BG-03-3060-09-040-A 思い掛けず おもいがけず 思い掛けず
kaneko 0001 3 55 00 00 BG-02-3060-01-010-A -- おもう おもう
kaneko 0001 3 55 00 00 BG-02-1515-07-020-A -- かける かける
kaneko 0001 3 55 00 00 BG-09-0010-01-010-A -- ず ず
kaneko 0001 0 02 00 00 BG-01-1624-02-010-A 春 はる 春
kaneko 0001 0 65 00 00 BG-08-0065-07-010-A は は は
kaneko 0001 0 48 02 04 BG-02-1527-01-010-A 来 くる 来る
kaneko 0001 0 74 54 01 BG-09-0010-04-010-A た た た
kaneko 0001 0 21 00 00 BG-01-1010-01-020-A こと こと こと
kaneko 0001 0 61 00 00 BG-08-0061-03-010-A で で で
kaneko 0001 0 47 17 01 BG-02-1200-01-010-A ある ある ある
kaneko 0001 0 69 00 00 BG-08-0069-32-010-A わ わ わ
```

<!--
### **Contributing**

If you'd like to contribute to Project Title, here are some guidelines:
-->

### **License**

Project Title is released under the Apache 2.0 License.

### **Authors and Acknowledgment**

Project Title was created by **[Hilofumi Yamamoto](https://github.com/yamagen)**.

Additional contributors include:

- **[Bor Hodošček](https://github.com/borh)**
- **[Xudong Chen](https://github.com/idiig)**

Thank you to all the contributors for their hard work and dedication to the project.

<!--
### **Code of Conduct**

Please note that this project is released with a Contributor Code of Conduct. By participating in this project, you agree to abide by its terms. See the **[CODE_OF_CONDUCT.md](https://www.blackbox.ai/share/CODE_OF_CONDUCT.md)** file for more information.

### **FAQ**

**Q:** What is Project Title?

**A:** Project Title is a project that does something useful.

**Q:** How do I install Project Title?

**A:** Follow the installation steps in the README file.

**Q:** How do I use Project Title?

**A:** Follow the usage steps in the README file.

**Q:** How do I contribute to Project Title?

**A:** Follow the contributing guidelines in the README file.

**Q:** What license is Project Title released under?

**A:** Project Title is released under the MIT License. See the **[LICENSE](https://www.blackbox.ai/share/LICENSE)** file for details.

### **Changelog**

- **0.1.0:** Initial release
- **0.1.1:** Fixed a bug in the build process
- **0.2.0:** Added a new feature
- **0.2.1:** Fixed a bug in the new feature

### **Contact**

If you have any questions or comments about Project Title, please contact **[Your Name](you@example.com)**.

### **Conclusion**

That's it! This is a basic template for a proper README file for a general project. You can customize it to fit your needs, but make sure to include all the necessary information. A good README file can help users understand and use your project, and it can also help attract contributors.

-->
