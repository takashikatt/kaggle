# Kaggle入門
## 01.概要
`Kaggle` は、機械学習モデルを構築するコンペティションのプラットフォーム.
<br/>
企業や研究者がデータを投稿し、世界中の統計家やデータ分析者が機械学習モデルを構築してスコアを競います.

## 02.Tiers
コンテスト等で入賞すると,ユーザのランクが変動する.<br/>
ユーザ登録時は全員 `Novice` から始まり, `Grandmaster` が最高ランクとなる.
| Tiers       | url                                        |
| ----------- | ------------------------------------------ |
| Novice      | [link](https://www.kaggle.com/progression) |
| Contributor | [link](https://www.kaggle.com/progression) |
| Expert      | [link](https://www.kaggle.com/progression) |
| Master      | [link](https://www.kaggle.com/progression) |
| Grandmaster | [link](https://www.kaggle.com/progression) |

ユーザ分布は以下通りであり,[Kaggle Rankings](https://www.kaggle.com/rankings?group=competitions&page=1&pageSize=20)にて確認できる.

```mermaid
pie title 2022/01/01時点のパフォーマンス分布
    "Novice" : 92861
    "Contributor" : 65121
    "Expert" : 7254
    "Master" : 1678
    "Grandmaster" : 242
```

## 03.コンペティションの種類
代表的なコンペは以下の通り.<br>
その他は[link](https://www.kaggle.com/docs/competitions)を参照.<br>
| Competitions    | 役割                                                                                         |
| --------------- | -------------------------------------------------------------------------------------------- |
| Getting Started | メダルがなくランキングに反映されない練習用コンペ.<br>半永久的に開催されている.<br>           |
| Playground      | `Getting Started` より難易度が一段階上のお楽しみコンペ.<br>少額の賞金や景品が獲得できる.<br> |
| Featured        | 一般的なコンペ.<br>賞金やメダルが獲得できる.<br>                                             |
| Research        | `Featured` よりも実験的な問題を扱うコンペ.<br>賞金やメダルが獲得できる.<br>                  |


## 04.コンペティションの提出種類
[competition-formats](https://www.kaggle.com/docs/competitions#competition-formats)を参照.<br>
| Competition formats      | 役割                                                                                                                                                                                                                                                                                                                                               |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Simple   Competitions    | 標準のKaggleコンペで利用される.<br>ローカルorノートブックでモデルを構築し,予測結果ファイルをKaggleにアップロードすることで競う形式.<br>                                                                                                                                                                                                            |
| Two-stage   Competitions | xxx                                                                                                                                                                                                                                                                                                                                                |
| Code   Competitions      | 全てKaggle Notebook上で作成するコンペ.<br>提出物を直接コンペにアップロードすることはできない.<br>このコンペには2種類の特徴がある.<br>・全ユーザが同じマシンスペックで競技するため,参加者のバランスが取れている.<br>・また,プラットフォームによって課せられた制約内のスペックで実行する必要があるため,他のコンペよりもモデルは単純になる傾向がある. |

## 05.Leaderboard
コンペの順位表のこと.<br>
テストデータの `oo%` に対してのモデル順位がPublic Leaderboardに、それ以外の `oo%` に対してのモデル順位がPrivate Leaderboardに記録される.<br>
モデルの提出回数が多いと最終順位が良くなるよう調整が可能なため,`Public` と `Private` でデータやLeaderboardが分けられている.<br>
基本的にデータ量は `Private > Public` となる.<br>

| Leaderboard         | 役割                                          |
| ------------------- | --------------------------------------------- |
| Public Leaderboard  | テストデータの一部で評価された暫定順位表.<br> |
| Private Leaderboard | コンペ終了後に発表される最終順位表.<br>       |
