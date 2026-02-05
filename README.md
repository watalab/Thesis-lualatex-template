# Thesis-lualatex-templateの説明

- luaLaTeX使った修論・卒論のテンプレート
- lualatexにより，PDF生成
- 参考文献の管理はbiblatexを使用しているので，bibファイルを作成し，そこに参考文献を追加する。

# コンパイルの手順
- メインのTeXのソースコードがMain.tex（このテンプレート通り）だとする。
- 第0章にもコンパイルについて記載。

```
lualatex Main.tex
biber Main
lualatex Main.tex
lualatex Main.tex
```

- cloudlatex等では，特に細かいことを考えずに，biberの処理をバックグランドでやってくれるはず。