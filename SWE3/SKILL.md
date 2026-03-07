---
name: SWE3
description: アーキテクチャ設計に基づき、ソフトウェアユニットの詳細設計およびソースコードの実装（SWE.3）を担当します。
---

# 目的
アーキテクチャコンポーネント（COMP）を、具体的なアルゴリズム、データ構造、および変数のレベルまで詳細化（DD）し、それに基づいた高品質なソースコードを作成すること。

# インプット
- ソフトウェアアーキテクチャ設計書: `c:\AntiGravity\Gantt\SWE_report\SWE2\02_SoftwareArchitectureDesign.md`
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\SWE3\TEMPLATE.md`

# 手順
1. **ユニット詳細設計**: 各 COMP ID に対し、内部の具体的な処理ロジックやデータ処理アルゴリズムを定義し、詳細設計 ID を付与します。
2. **上位追跡性**: 各詳細設計項目がどの **COMP-xxx** を詳細化したものかを明示します。
3. **詳細設計書の出力**: テンプレートに従い、`c:\AntiGravity\Gantt\SWE_report\SWE3\03_SoftwareDetailedDesign.md` を出力します。
4. **コーディング実装**: 詳細設計の内容に忠実に、`c:\AntiGravity\Gantt\main.py` を実装（または更新）します。
5. **コードの自己検証**: コーディング規約の遵守、および詳細設計項目に対する実装漏れの有無を確認します。

# アウトプット
- ソフトウェア詳細設計書: `c:\AntiGravity\Gantt\SWE_report\SWE3\03_SoftwareDetailedDesign.md`
- ソースコード実装: `c:\AntiGravity\Gantt\main.py`

# 制約事項
- 出力（設計書）はすべて日本語で行うこと。
- 全ての詳細設計項目に **DD-xxx**（例: DD-001）形式のIDを付与すること。
- ソースコードは詳細設計に完全に裏打ちされている必要があり、設計にないアドホックなロジックを排除すること。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
