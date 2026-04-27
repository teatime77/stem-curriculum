stem-curriculum/
├── 00_Introduction/
│   └── roadmap.md             # プロジェクトの全貌と「計算機という筆」の思想
│
├── 01_Phase1_Elementary/      # 【テーマ：測る・数える・動かす】
│   ├── math_01_numbers.md     # 離散と連続
│   ├── science_01_world.md    # 観察と測定
│   └── comp_01_logic.md       # ロジック：コンピュータとの対話（TS入門）
│
├── 02_Phase2_JuniorHigh/      # 【テーマ：未知の操作と自動化】
│   ├── math_01_algebra.md     # 代数：文字という型
│   ├── physics_01_force.md    # 力：変化の原因
│   └── comp_01_simulation.md  # シミュレーション：法則をコードで動かす
│
├── 03_Phase3_HighSchool/      # 【テーマ：多次元と極限の計算】
│   ├── math_01_vector.md      # ベクトル：空間の記述
│   ├── math_02_calculus.md    # 微積分：変化の追跡
│   └── comp_01_numerical.md   # 数値解析：無限を有限で計算する（オイラー法等）
│
├── 04_Phase4_University/      # 【テーマ：抽象化と並列計算】
│   ├── math_01_linear_alg.md  # 線形代数：空間の変換
│   ├── physics_01_analytical.md # 解析力学：作用最小の原理
│   ├── physics_03_quantum.md  # 量子力学：確率と演算子
│   └── comp_01_webgpu.md      # WebGPU：並列宇宙の計算機（GPGPU入門）
│
└── 05_Phase5_LatticeQCD/      # 【最終到達点：格子上の宇宙】
    ├── math_group_theory.md   # 群論：対称性の数学（SU(3)）
    ├── phys_statistical.md    # 統計力学：経路積分と分配関数
    ├── comp_monte_carlo.md    # モンテカルロ法：HMCアルゴリズムの実装
    └── comp_lattice_qcd.md    # 格子ゲージ理論：WebGPUによるQCDシミュレーション

---

## Project Update: Computation Axis (2026-04-27)

### Core Policy
- コードは「第二の筆」であり、数学・物理の概念を検証する実験装置として扱う。
- プログラミングは独立教科ではなく、各 Phase の数理・物理内容に統合する。
- 最終ゴールは、TypeScript + WebGPU による格子ゲージ理論（LGT）シミュレータの自力実装。

### Implementation Rules for Future `comp_` Chapters
- 文法中心ではなく「物理法則をアルゴリズムへ翻訳する」ことを主目的にする。
- 既習概念（離散/連続、ベクトル、保存則、対称性、作用）を必ずコード上で再登場させる。
- 型（TypeScript）を次元・状態空間・演算子の安全な表現として設計する。
- WebGPU は「高速化ツール」ではなく、並列時間発展・格子更新の思考様式として導入する。
- 各 `comp_` 章には「理論式 -> 擬似コード -> 実装骨格 -> 検証」の流れを含める。

### Educational Throughline
- Phase 1-2: 観測とルールを小さなコード実験で再現
- Phase 3: 微積分・ベクトルを数値計算として離散化
- Phase 4: 線形代数・微分方程式・場を TypeScript で抽象化
- Phase 5: HMC と格子QCDを WebGPU で並列実装し、理論と計算を統合