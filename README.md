# MatchingServiceIsm
マッチングサービス制作のための何か

# コーディング規約

BEM <br>
htmlhint: 標準設定 <br>
stylelint: recommended, recess, prettier <br>
eslint: airbnb-base/legacy (JSはES5を利用) <br>

# ディレクトリ解説

| 名前 | 説明 |
| - | - |
| _dev | 開発用のフォルダ。pug, scss, js, 画像ファイルが格納されます。 |
| dist | 成果物のフォルダ。gitの管理対象には含まれません。`yarn dev`や`yarn build`で生成されます。 |
| docs | ボイラープレートの詳細資料のフォルダ。開発には直接利用しませんが、細かいカスタマイズの際に参照してください。 |
| setup | 初期環境構築用のファイルです。環境構築ウィザードを完了すると削除されます。 |
| gulpfile.js | gulpの設定ファイル |

初回起動前にはパッケージのインストールが必要です。下記のコマンドを実行して、モジュールをインストールしてください。
yarn

### yarn scripts 一覧

| コマンド | 内容 |
| - | - |
| dev   | gulp でプレビューサーバーと watch タスクを開始します。 |
| build | ビルド用の設定で`dist`配下のファイルを作成します。**webpack 等の設定が`dev`とは異なる**ため、納品時は必ずこちらのコマンドを利用してください。 |
| eslint | ESLintを実行します。 (指摘のみ) |
| eslint:fix | ESLintを実行します。 (fixできるものは修正します) |
| stylelint | stylelintを実行します。 (指摘のみ) |
| stylelint:fix | stylelintを実行します。 (fixできるものは修正します) |
| format | prettierでフォーマットをかけます。 |
| test | jest のテストスイートを実行します。 |

## 開発を開始する

```
yarn dev
```
