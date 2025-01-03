# 概要
Learn Next.js のチュートリアル実践記です。

# 学習内容
## [Chapter 2 Css Styling](https://nextjs.org/learn/dashboard-app/css-styling)
css について。基本的には [Tailwind](https://tailwindcss.com/) を使用する。
もちろん .css ファイルを新たに作成して自前で css クラスを作って割り当てることもできるが、上記のようなライブラリがあるので基本的にはそちらを使用。

条件に応じて特定の箇所の css 適用を変えたい場合は [clsx](https://www.npmjs.com/package/clsx) を利用する。

## [Chapter 3 Optimizing Fonts and Images](https://nextjs.org/learn/dashboard-app/optimizing-fonts-images)
Next.js ではビルド時に静的コンテンツと併せてフォントファイルも保持するような挙動をする。これによりフォント取得のためだけにリクエストを飛ばさないようにしてパフォーマンスの向上を図っている。

### 文字フォント
[next/font](https://nextjs.org/docs/app/api-reference/components/font) を使うことにより使いたいフォントだけ落としてくることが可能。（使わないものに対するリクエストは飛ばない。）
[google font](https://fonts.google.com/) で設定されているフォントは全て利用が可能。next/font/google ライブラリからインポートする。
