---
name: SUP10
description: 問題管理表（SUP9）から判明した製品の機能不全を、「変更要求（SUP.10）」として正規の要件管理プロセスへ繋げます。
---

# 目的
特定された問題に対する解決策が「仕様の変更」を伴う場合、それを制御された形式（Change Request）で文書化し、要求（SRS）への反映を確実に行うことで、一貫性のある変更制御を実現すること。

# インプット
- 問題管理表: `c:\AntiGravity\Gantt\SWE_report\SUP9\09_ProblemManagementList.md`
- ソフトウェア要件仕様書 (SRS): `c:\AntiGravity\Gantt\SWE_report\SWE1\01_SRS.md`
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\SUP10\TEMPLATE.md`

# 手順
1. **変更の必要性判定**: `SUP9` の課題（PR）のうち、修正がソースコードだけではなく「要件」や「設計」の変更を必要とするものを抽出します。
2. **変更要求の文書化**: 変更内容、変更理由、および影響範囲を分析し、**CR-xxx** 形式のIDで管理表に登録します。
3. **影響分析の実行**: 変更が下流の設計(SWE2/3)、実装(main.py)、検証(SWE4-6)のどの成果物に波及するかを特定します。
4. **要件仕様書への反映**: 承認された CR に基づき、`c:\AntiGravity\Gantt\SWE_report\SWE1\01_SRS.md` へ新しい要求（REQ）として追記し、追跡性を確保します。
5. **CRリストの更新**: 要件反映が完了した CR のステータスを「反映済み」に更新し、`c:\AntiGravity\Gantt\SWE_report\SUP10\10_ChangeRequestList.md` を出力します。

# アウトプット
- 変更要求管理表: `c:\AntiGravity\Gantt\SWE_report\SUP10\10_ChangeRequestList.md`
- ソフトウェア要件仕様書（更新版）: `c:\AntiGravity\Gantt\SWE_report\SWE1\01_SRS.md`

# 制約事項
- 出力はすべて日本語で行うこと。
- 各変更要求には **CR-xxx**（例: CR-001）形式のIDを付与し、元の PR ID との紐付けを必須とすること。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
