# SWE_agent 標準ワークフロー (G-SPICE / A-SPICE準拠)

本ワークフローは、Automotive SPICE 4.0 の要求事項に基づき、エージェントによる自動化されたソフトウェア開発プロセスを定義します。

## プロセスフロー

0. **プロジェクト計画 (MAN3)**
   - スキル: `SWE_agent/MAN3/SKILL.md`
   - 成果物: `SWE_report/MAN3/00_ProjectPlan.md`

0b. **リスク管理 (MAN5)**
   - スキル: `SWE_agent/MAN5/SKILL.md`
   - 成果物: `SWE_report/MAN5/05_RiskManagementReport.md`

1. **ソフトウェア要件分析 (SWE1)**
   - スキル: `SWE_agent/SWE1/SKILL.md`
   - 成果物: `SWE_report/SWE1/01_SRS.md` (ID: REQ-xxx)

2. **アーキテクチャ設計 (SWE2)**
   - スキル: `SWE_agent/SWE2/SKILL.md`
   - 成果物: `SWE_report/SWE2/02_SoftwareArchitectureDesign.md` (ID: COMP-xxx)

3. **詳細設計・実装 (SWE3)**
   - スキル: `SWE_agent/SWE3/SKILL.md`
   - 成果物: `SWE_report/SWE3/03_SoftwareDetailedDesign.md` (ID: DD-xxx), `main.py`

4. **ユニット検証 (SWE4)**
   - スキル: `SWE_agent/SWE4/SKILL.md`
   - 成果物: `SWE_report/SWE4/04_SoftwareUnitVerificationReport.md` (ID: UT-xxx), `test.py` (Unit)

5. **統合検証 (SWE5)**
   - スキル: `SWE_agent/SWE5/SKILL.md`
   - 成果物: `SWE_report/SWE5/05_SoftwareIntegrationVerificationReport.md` (ID: IT-xxx), `test.py` (Integration)

6. **適格性確認テスト (SWE6)**
   - スキル: `SWE_agent/SWE6/SKILL.md`
   - 成果物: `SWE_report/SWE6/06_SoftwareQualificationTestReport.md` (ID: QT-xxx)

7. **トレーサビリティマトリクス (TraceabilityMatrix)**
   - スキル: `SWE_agent/TraceabilityMatrix/SKILL.md`
   - 成果物: `SWE_report/TraceabilityMatrix.md`

8. **問題管理 (SUP9)**
   - スキル: `SWE_agent/SUP9/SKILL.md`
   - 成果物: `SWE_report/SUP9/09_ProblemManagementList.md` (ID: PR-xxx)

8b. **変更要求管理 (SUP10)**
   - スキル: `SWE_agent/SUP10/SKILL.md`
   - 成果物: `SWE_report/SUP10/10_ChangeRequestList.md` (ID: CR-xxx)
   - *備考: CRは次サイクルのSWE1の入力となり要件を更新する。*

9. **プロセス改善 (PIM3)**
   - スキル: `SWE_agent/PIM3/SKILL.md`
   - 成果物: `SWE_report/PIM3/10_ProcessImprovementRecord.md` (ID: IMP-xxx)
   - *備考: 各スキルのSKILL.md定義自体を修正し、自己改善を図る。*

## 完了基準
- `SWE_report` 以下の全レポート（00〜10）が最新の設計/実装と一貫性を保ち生成されていること。
- `TraceabilityMatrix.md` において、要求網羅率が100%であり、全ての証跡が紐付いていること。
- 適格性確認テスト（SWE6）の結果がすべて「合格」であること。
 village
