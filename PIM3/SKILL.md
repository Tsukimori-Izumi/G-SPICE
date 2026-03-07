---
name: PIM3
description: 開発・検証プロセス（各スキルの実行結果および問題点）を分析し、スキルの定義自体を改善（PIM.3）します。
---

# 目的
エージェント自身の活動記録（PR, CR, IMP）を分析し、プロセスの定義（SKILL.md）やテンプレートを自律的にブラッシュアップし続けることで、組織全体の成熟度（Process Maturity）と成果物の品質を継続的に向上させること。

# インプット
- 問題管理表: `c:\AntiGravity\Gantt\SWE_report\SUP9\09_ProblemManagementList.md`
- 変更要求管理表: `c:\AntiGravity\Gantt\SWE_report\SUP10\10_ChangeRequestList.md`
- 各工程の成果物/実行ログ: `c:\AntiGravity\Gantt\SWE_report\` 配下の最新成果物
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\PIM3\TEMPLATE.md`

# 手順
1. **プロセス分析**: `SUP9` や `SUP10` の傾向を分析し、指示内容の曖昧さや工程の欠陥に起因する再発問題を特定します。
2. **改善提案の策定**: 特定された問題の再発を防止するために、該当するスキルの `SKILL.md` の「手順」や「制約事項」の具体的な修正案を作成します。
3. **改善記録の更新**: 改善案、期待される定量・定性的効果を記録ID **IMP-xxx** 形式で `c:\AntiGravity\Gantt\SWE_report\PIM3\10_ProcessImprovementRecord.md` に登録します。
4. **プロセス（スキル）の更新**: 承認された改善案に基づき、実際に `SKILL.md` ファイル群を書き換え、プロセスの標準を最新化します。
5. **有効性の評価**: 次回案件や後続フェーズの実行結果を監視し、改善が意図した効果（エラー減、品質増等）を上げているかを評価します。

# アウトプット
- プロセス改善記録: `c:\AntiGravity\Gantt\SWE_report\PIM3\10_ProcessImprovementRecord.md`
- 修正されたスキル定義資産: `c:\AntiGravity\Gantt\SWE_agent/` 配下の各 `SKILL.md`

# 制約事項
- 出力はすべて日本語で行うこと。
- 各改善提案には **IMP-xxx**（例: IMP-001）形式の一意なIDを付与すること。
- 改善は形式的なものではなく、実効性（エラー率の低下やトレーサビリティの向上）を最優先とすること。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
