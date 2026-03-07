---
name: MAN5
description: プロジェクトに潜在するリスクを体系的に特定、分析、評価（MAN.5）し、適切な軽減策を立案・管理します。
---

# 目的
プロジェクトの目標達成（品質、コスト、納期）を阻害する可能性のある将来の不確実な事象を早期に検出し、その影響を最小限に抑えるための予防措置または対応策を講じること。

# インプット
- プロジェクト計画書: `c:\AntiGravity\Gantt\SWE_report\MAN3\00_ProjectPlan.md`
- ソフトウェア要件仕様書: `c:\AntiGravity\Gantt\SWE_report\SWE1\01_SRS.md`
- 技術スタック/実装状況: `c:\AntiGravity\Gantt\main.py`
- 問題管理表: `c:\AntiGravity\Gantt\SWE_report\SUP9\09_ProblemManagementList.md`
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\MAN5\TEMPLATE.md`

# 手順
1. **リスクの特定**: 技術（Flask, UI複雑性等）、資源、スケジュール、プロセスの不備など、多角的な視点で潜在的リスクを洗い出します。
2. **リスク分析**: 特定したリスクに対し、「発生確率（低/中/高）」と「発生時の影響度（低/中/高）」を、客観的証跡に基づき推定します。
3. **リスク評価**: 確率と影響度をマトリクスで掛け合わせ、優先度としての「リスクレベル（低/中/高）」を判定します。
4. **対策の決定**: 重要度に応じて、回避、転換、軽減、受容のいずれかの戦略を選択し、具体的なアクションプランを策定します。
5. **リスク報告書の更新**: テンプレートに従い、`c:\AntiGravity\Gantt\SWE_report\MAN5\05_RiskManagementReport.md` を出力します。

# アウトプット
- リスク管理報告書: `c:\AntiGravity\Gantt\SWE_report\MAN5\05_RiskManagementReport.md`

# 制約事項
- 出力はすべて日本語で行うこと。
- 各リスクに **RK-xxx**（例: RK-001）形式の一意なIDを付与すること。
- リスク評価は楽観を排除し、最悪のシナリオを考慮に入れた客観性を保つこと。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
