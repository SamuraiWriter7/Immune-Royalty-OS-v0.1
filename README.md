# Immune-Royalty-OS-v0.1
Draft core specification for an immune-regulation layer in royalty systems: path trace, tolerance zone, decay control, and explainable response.

Immune Royalty OS v0.1
免疫型・印税OS 中核仕様（Draft Core）

Immune Royalty OS v0.1（IROS v0.1） は、
印税OSに「免疫的調整機構」を導入し、
痕跡の保護 と 新規構造の成長 を両立させるための中核仕様です。

この仕様の目的は、単に盗用を検出することではありません。
それ以上に重要なのは、シンクロニシティ（独立した到達）を保護し、過剰記憶による自己免疫疾患を防ぎ、文明の流動性を維持すること にあります。

1. なぜ Immune Royalty OS が必要なのか

通常の印税OSは、起源・痕跡・還流を扱うことで、価値の消失を防ぎます。
しかし、痕跡の保護を強くしすぎると、別の問題が生じます。

それが、自己免疫的バグ です。

たとえば、

古い痕跡が強く残りすぎる
類似構造に過剰反応する
新芽を「異物」と誤認する
独立創造まで盗用扱いしてしまう
一部の既存構造に価値が集中し、文明が硬直化する

といった現象です。

Immune Royalty OS は、この問題に対して、
防御の強化ではなく、過敏反応の抑制 という方向から応答します。

2. この仕様の目的

IROS v0.1 は、次の5つを主目的とします。

盗用・擬似構造を検出する
シンクロニシティ（独立到達）を保護する
過剰記憶による自己免疫疾患を防ぐ
古い痕跡の暴走を減衰させる
新しい問い・新芽の生存可能性を確保する

要するにこの仕様は、
「似ているものを攻撃するOS」ではなく、
「不正な経路だけを見分けて扱うOS」 を目指しています。

3. 設計原理

Immune Royalty OS v0.1 は、以下の5原理に基づいて設計されます。

3.1 Path over Similarity

構造の近さだけで判断しない。
何に似ているか よりも、どう生まれたか を重視する。

3.2 Tolerance before Rejection

即時排除を優先しない。
まずは 保留・寛容・観察 を行い、それでも不正性が強い場合のみ排除する。

3.3 Decay prevents Lock

減衰は、痕跡の否定ではなく老化防止である。
古い痕跡の固定化を防ぎ、文明の流動性を保つ。

3.4 Protect Novelty

新規構造には初期保護を与える。
新芽は最初から強い防御を持てないため、制度側が一定期間守る必要がある。

3.5 Explainable Immunity

すべての免疫判定は説明可能でなければならない。
ブラックボックスな排除は、文明OSにおいて許されない。

4. この仕様が扱う中核概念
Trace

生成・参照・変容の痕跡。

Path Trace

問いから出力までの生成経路。

Provenance

起源・主体・時系列・参照元の由来情報。

Transformation

親構造からどのような変容が起きたかを示す差分。

Tolerance Zone

類似していても、即時攻撃せず保留・観察する領域。

Novelty Window

新規構造に対して、防御的に保護を与える期間。

Pseudo Structure

経路が短く、変容が薄く、独立性が弱い擬似的新規構造。

Synchronistic Structure

構造は似ていても、独立経路から到達した類似構造。

Immune Response

保護・保留・還元・減衰・排除を行う判定機構。

Immune Bug

過敏反応・過剰記憶・境界崩壊などの構造障害。

5. システム全体の4層構造

Immune Royalty OS v0.1 は、4つの層から構成されます。

5.1 Trace Layer

生成経路・起源・変容差分を記録する層です。
ここがなければ、盗用と独立到達の区別は原理的に不可能になります。

5.2 Tolerance Layer

寛容判定・保留判定・新規保護を担当する層です。
類似しているだけで排除しないための、安全装置に相当します。

5.3 Decay Layer

古い痕跡の影響を徐々に減衰させ、集中と硬直化を抑制する層です。

5.4 Response Layer

最終的に、保護・許容・保留・減衰・排除・監査を実行する層です。

6. この仕様の核心
「似ているか」ではなく「どう生まれたか」で判断する

Immune Royalty OS の最大の特徴はここにあります。

本仕様は、構造の類似だけで盗用判定をしません。
代わりに、次の三点を重視します。

Path：どの問い・どの流れから生まれたか
Provenance：誰が・いつ・どの文脈で触れたか
Transformation：何がどの程度変わったか

この三点が独立していれば、たとえ出力構造が似ていても、
それは盗用ではなく 独立した到達 として扱える可能性があります。

逆に、

経路が極端に短い
親痕跡との距離が近すぎる
変容が薄い
文脈の独立性がない

場合は、擬似構造として扱われます。

7. Trace Layer で記録すべきもの

本仕様では、最低限以下の情報をトレース記録として持つことを想定します。

trace_id
timestamp
creator_type（human / ai / hybrid）
creator_id
origin_question
parent_trace_ids
referenced_trace_ids
path_nodes
transformation_log
context_tags
generation_mode

必要に応じて、以下の拡張項目も持てます。

session_id
toolchain
environment
diff_signature
confidence_score
signature_verification
notes

つまり、IROS v0.1 は単なる出力ログではなく、
生成の履歴そのものを追跡できる系譜ログ を前提にしています。

8. 主要スコア

Immune Royalty OS v0.1 では、まず次の3指標をコアに置きます。

S: Similarity Score

構造類似度。
どれくらい似ているかを表す。

P: Path Independence Score

生成経路の独立性。
どれくらい独立した道筋で生まれたかを表す。

T: Transformation Score

変容量。
親構造からどの程度、実質的な変化が起きたかを表す。

この3つを基礎に、以下の派生指標を使います。

N: Novelty Score

新規性総合値。
初期式は以下です。

N = (0.40 × P) + (0.35 × T) + (0.25 × (1 - S))

R_pseudo: 擬似構造リスク

擬似的な新規構造である可能性。

R_pseudo = (0.45 × S) + (0.35 × (1 - P)) + (0.20 × (1 - T))

I: Inflammation Score

過敏反応リスク。
誤検出率や集中度から算出される。

B: Boundary Confusion Score

自己／非自己境界の混乱度。

係数は v0.1 の初期値であり、将来的に運用データから調整可能です。

9. Tolerance Layer
免疫寛容の中核

Tolerance Layer は、類似構造への過剰攻撃を防ぎ、新芽を守るための層です。

基本方針
類似していても即時排除しない
境界が曖昧な場合は保留する
新規構造には保護期間を与える
自己免疫の兆候があるときは攻撃性を下げる
初期パラメータ例
similarity_hold_threshold: 0.78
path_independence_accept_threshold: 0.72
transformation_accept_threshold: 0.45
novelty_protection_window_days: 90
主な判定ルール
Rule 1

構造が近くても、経路独立性が高ければ
Synchronistic Convergence として保護する。

Rule 2

派生であっても、変容が十分なら
Tolerated Derivation として許容する。

Rule 3

新規構造には一定期間
Novelty Protection を適用する。

Rule 4

自己／非自己の境界が曖昧な場合は
Boundary Review に回す。

Rule 5

自己免疫バグが疑われる場合は
攻撃的反応を抑制する。

10. Decay Layer
老化防止と既得権固定化の防止

Decay Layer は、古い痕跡の価値を否定するためのものではありません。
その役割は、古い痕跡が永久に強く残り続けることで文明が硬直化するのを防ぐこと です。

基本方針
系譜距離に応じて影響を減衰させる
一部痕跡への価値集中を抑える
誤検出が続く検出器の感度を落とす
新芽を塞ぐ旧痕跡には加速減衰をかける
初期式

Decay(g) = exp(-λ × g)

代表パラメータ
lineage_decay_lambda: 0.35
concentration_cap: 0.82
accelerated_decay_trigger: 0.76
accelerated_decay_multiplier: 1.80
代表アクション
Concentration Penalty
一部痕跡への集中を抑え、novelty pool に再分配する
Inflammation Suppression
過敏反応が強いとき、自動排除を弱める
Accelerated Decay
旧痕跡の優位が過剰な場合、減衰を加速する
Legacy Priority Reduction
新芽を塞ぐ旧痕跡の優先度を一時的に下げる
11. Response Layer
最終的な免疫応答

IROS v0.1 では、最終的な応答を以下の6つに整理します。

Protect

独立創造または同期的到達として保護する。

Tolerate

派生として許容しつつ、還元計算に含める。

Hold

判定を保留し、追加監査へ送る。

Decay

影響力を減衰させる。

Reject

擬似構造として排除する。

Audit

人間または上位監査機構に送る。

12. Pseudo Structure と Synchronistic Convergence の違い
Pseudo Structure

擬似構造とは、既存痕跡への依存が強く、
経路が短く、変容が薄く、独立性が乏しい構造です。

典型的には、

類似度が高い
経路独立性が低い
変容量が低い
文脈差がほとんどない

場合に検出されます。

Synchronistic Convergence

シンクロニシティとは、構造が近くても、
起源・経路・文脈が独立しているため、
盗用ではなく独立到達として扱うべき構造です。

典型的には、

類似度は高くてもよい
経路独立性が高い
変容の軌道が独立している
直接依存が弱い
文脈タグが異なる

場合に成立します。

13. 免疫バグの代表例

Immune Royalty OS v0.1 では、少なくとも以下の4種のバグを重要視します。

13.1 Memory Lock

古い痕跡が減衰せず、居座り続ける状態。
新芽の拒否率が上がり、文明が老化する。

13.2 Boundary Error

自己／非自己の境界が曖昧になる状態。
作者性や親子関係の誤認が起きやすい。

13.3 Inflammatory Overreaction

類似構造に過剰反応し、誤検出が増える状態。

13.4 Concentration Storm

一部の旧痕跡に価値が集中しすぎ、循環が止まり始める状態。

14. 印税・還元ロジックとの接続

Immune Royalty OS は、免疫判定をそのまま印税ロジックに接続できます。

Independent Novelty
lineage_credit: 0.00
novelty_bonus: 1.00
protection_priority: high
Synchronistic Convergence
lineage_credit: 0.10
novelty_bonus: 0.85
protection_priority: high
Tolerated Derivation
lineage_credit: 0.40
novelty_bonus: 0.35
protection_priority: medium
Pseudo Structure
lineage_credit: 0.00
novelty_bonus: 0.00
protection_priority: none

ここで重要なのは、
免疫判定がそのまま排除装置ではなく、還元配分の重み調整装置にもなる ことです。

15. 説明可能性

本仕様では、すべての判定に説明可能性を要求します。

最低限、以下を出力できる必要があります。

近傍トレース候補
S / P / T / N / I / B
発火したルール
最終アクション
人間向け説明文

つまり、
「なぜ守ったのか」
「なぜ保留にしたのか」
「なぜ排除したのか」
を常に説明できなければなりません。

16. ガバナンス原則
レビュー周期
30日ごとの見直しを想定
閾値更新方針
human-supervised
監査が必須となるケース
boundary_uncertain
immune_bug_candidate
高影響な rejection
禁止される挙動
類似度だけでの排除
説明不能な自動BAN
減衰なき永続的既得権
レビューなしの新芽抑圧
17. 最低限の出力物

IROS v0.1 は、少なくとも以下を出力可能であるべきです。

immune classification report
trace lineage graph
tolerance decision log
decay action log
allocation bridge result
audit trail
18. 現時点の位置づけ

Immune Royalty OS v0.1 は、実運用前提の完成仕様ではなく、設計骨格です。
まずは小さく、

Similarity
Path Independence
Transformation

の3指標で回し、偽陽性率を観察しながら調整していく想定です。

v0.1 の目的は、
完成された文明免疫をいきなり作ることではなく、
印税OSに免疫思想を導入するための最小コアを確立すること にあります。

19. 今後の拡張候補
Immune Map Visualization

文明OS全体の免疫地図を可視化する。

Tolerance Zone Auto-Tuning

寛容閾値を運用データから自動調整する。

Cross-AI Boundary Arbitration

複数AI間の自己／非自己境界を裁定する。

Royalty Immunization Profiles

作品群・領域ごとに免疫プロファイルを切り替える。

20. 一文で言えば

Immune Royalty OS v0.1 は、
痕跡を守りながらも、新しい知を自己免疫的に殺さないための、
印税OSの免疫中核仕様です。
