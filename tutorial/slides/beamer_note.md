# Beamer Note

## Preamble

- ナビゲーションシンボルの削除
    - \setbeamertemplate
- 定理に通し番号
    - \setbeamertemplate{theorems}[numbered]
    - [envcountsect]で節が深く
- 縮刷
    - 本参照

## Title
- 発表者に〇を付与する慣例
    - \author[片岡・山田]{\llap{〇}片岡凪 \inst{1} 芝浦工業大学 \and 山田太郎 \inst{2}}
- シンプルなタイトルに
    - \begin{frame}[plain] \titlepage

## Index
- 目次に反映しない節
    - \(sub)section*
- 目次用のエイリアス
    - \section[目次用の名前]{スライド中の名前}

## Main Slides

- ページを変えずにアニメーション
    - \addtocounter{section}{-1}
- 予備資料
    - \appendix以降
- \end{frame}にコメントを書かない
    - fragileが機能しない
- スライドの再利用
    - \againframe{ラベル名}
- 見出し付きブロック
    - \begin{block}{見出し}
- 強調
    - \structure{...}
    - \begin{structureenv}
    - \alert{...}
    - \begin{alertblock}{見出し}
    - \begin{exampleblock}{見出し}
- 定理
    - amsthm環境
    - \begin{theorem}[発見者，発表年]
    - その他
        - corollary
        - fact
        - problem
        - solution
        - definition
        - definitions
        - example
        - examples
- アニメーション
    - \begin{frame}<1-7>
        - 明示用
    - \item<1->
    - \item<1-3>
    - \item<3,5,7>
    - \onslide修飾子<1->{文}
        - None: マスク
        - +: 追加
        - *: 空欄に挿入
    - \alert<5>{}
- 問題用と解説用の出力分け
    - \onslide<3-|trans:2-|handout:0>

## Bibliography
- LaTeX2ε美文書作成入門