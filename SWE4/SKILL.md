---
name: SWE4
description: ソフトウェア詳細設計（DD）に基づき、ソフトウェアユニットの検証（ホワイトボックステスト：SWE.4）を担当します。
---

# 目的
実装されたソースコードの最小単位（関数、クラス、モジュール）が、詳細設計で定義された内部動作を正確に行うこと、および予期せぬ入力に対しても頑健であることを、コード・ロジックレベルで検証・証明すること。

# インプット
- ソフトウェア詳細設計書: `c:\AntiGravity\Gantt\SWE_report\SWE3\03_SoftwareDetailedDesign.md`
- ソースコード: `c:\AntiGravity\Gantt\main.py`
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\SWE4\TEMPLATE.md`

# 手順
1. **ユニットテスト設計**: 各詳細設計項目（DD）に対し、パス網羅や境界値分析を考慮した検証項目を作成します。
2. **テストコードの実装**: `c:\AntiGravity\Gantt\test.py` の「ユニットテスト」セクションに、自動化された検証コードを追加します。
3. **検証の実行**: テストを実行し、実際の動作が詳細設計と一致するかを確認します。
4. **追跡性の付与**: 各テストケースがどの **DD-xxx** を検証するためのものかを明示します。
5. **検証報告書の出力**: テンプレートに従い、`c:\AntiGravity\Gantt\SWE_report\SWE4\04_SoftwareUnitVerificationReport.md` を出力します。

# アウトプット
- テストコード更新: `c:\AntiGravity\Gantt\test.py`
- ソフトウェアユニット検証報告書: `c:\AntiGravity\Gantt\SWE_report\SWE4\04_SoftwareUnitVerificationReport.md`

# 制約事項
- 出力はすべて日本語で行うこと。
- 各テストケースには **UT-xxx**（例: UT-001）形式の一意なIDを付与すること。
- 検証は詳細設計に完全に準拠し、客観的証跡（Evidence）に基づいて合否を判定すること。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
