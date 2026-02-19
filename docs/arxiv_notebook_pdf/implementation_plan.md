# 実装計画: BMS群とキャロル幾何学に関する解説記事の執筆

## 目標
NotebookLMから取得した論文「A geometrical invitation to BMS group theory」に基づき、BMS群理論、キャロル幾何学、およびその物理的意義について、数式を用いて詳細に解説する約5000字の記事を作成する。

## 解説記事の構成案

### 1. 導入 (Introduction)
- 一般相対性理論における漸近的対称性としてのBMS群の発見 (Bondi, Metzner, Sachs)。
- ポアンカレ群が期待されていたが、無限次元の拡大群が現れたことの驚き。
- 近年の物理的意義の再発見 (Stromingerらによる重力の散乱行列の対称性としてのBMS群)。
- 記事の目的: BMS群の幾何学的側面（特にNull Infinity上の幾何学）に焦点を当てた自己完結的な解説。

### 2. キャロル幾何学 (Carrollian Geometry)
- ガリレイ群の双対的な極限としてのキャロル群 ($c \to 0$)。
- 弱キャロル構造 (Weak Carrollian Structure):
    - オブザーバー場 $n$ (基本ベクトル場)。
    - キャロル計量 $\gamma$ (正定値半定符号、核は $n$ で張られる)。
    - 相対性の原理: 同時性は相対的だが、静止は絶対的。
- 強キャロル構造 (Strong Carrollian Structure):
    - アフィン接続 $\nabla$ の導入 ($\nabla n = 0, \nabla \gamma = 0$)。

### 3. 共形キャロル幾何学とBMS群 (Conformal Carrollian Geometry & BMS Group)
- 共形キャロル構造の定義: 同値類 $[n, \gamma]$。
    - $n \sim \Omega^{-1}n, \gamma \sim \Omega^2 \gamma$。
- **BMS変換 = 共形キャロル等長変換**:
    - Null Infinity ($\mathscr{I}$) 上のBMS対称性を、その上の共形キャロル構造を保つ変換として定義する。
    - 具体的な変換式: $u' = \Omega(x)(u + \mathcal{T}(x))$。
    - 超並進 (Supertranslation) $\mathcal{T}(x)$ の幾何学的解釈。

### 4. BMS群の構造 (Structure of BMS Group)
- 半直積構造: $BMS \simeq SO(3,1) \ltimes C^\infty(S^2)$ (4次元の場合)。
    - ローレンツ群 $SO(3,1)$ が超並進群 $C^\infty(S^2)$ に作用する。
- 重要な部分群:
    - 超並進群: 最大正規部分群 (Sachsの定理)。
    - 並進群: 超並進群の中の唯一の不変部分空間。
- 非標準的な部分群 (Non-canonical subgroups):
    - ポアンカレ部分群の選び方は一意ではない。
    - "Good Cut" (良い切断) と重力の真空 (Gravitational Vacuum) の対応関係。
    - ミンコフスキー時空の再構築 (Holographic reconstruction)。

### 5. BMS群のユニタリ表現 (Unitary Representations)
- ポアンカレ群の誘導表現論 (Wigner) の拡張 (McCarthy)。
- 超運動量 (Supermomentum) $\mathcal{P}$ の導入。
- 軌道と固定群 (Little Group) による分類:
    - **Hard Representations**: 質量のある粒子や通常の質量ゼロ粒子に対応。ポアンカレ粒子と一対一対応する。
    - **Soft Representations**: 運動量がゼロだが、超運動量が非ゼロの場合。Komar群の表現となる。
    - **Generic Representations**: 一般的な場合。
- 物理的意味: 赤外発散やソフト・グラビトン定理との関連。

### 6. 結論 (Conclusion)
- BMS群が示唆する、重力を含む理論における粒子の概念の拡張。
- キャロル幾何学という視点の有用性。

## 数式の扱い
- 定義式、変換則、代数構造などを省略せずに記載する。
- 例: キャロル計量の定義 ($\gamma_{\mu\nu}n^\nu=0$)、BMS代数の交換関係、GJMS演算子など。

## 検証
- 記事の内容が論文の記述と整合しているか確認する。
- 数式が正確に記述されているか確認する。
- 日本語として自然で読みやすい文章になっているか確認する。
