---
name: SWE1
description: 顧客要求事項（00_req.md）および変更要求（SUP10）に基づき、ソフトウェア要件分析（SWE.1）を実施します。
---

# 目的
顧客からの抽象的な要求を整理・分析し、実装および検証が可能な具体的かつ一貫性のある「ソフトウェア要件仕様書（SRS）」として定義すること。

# インプット
- 顧客要求事項: `c:\AntiGravity\Gantt\00_req.md`
- 変更要求管理表: `c:\AntiGravity\Gantt\SWE_report\SUP10\10_ChangeRequestList.md`
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\SWE1\TEMPLATE.md`

# 手順
1. **要求の抽出・分類**: `00_req.md` および `10_ChangeRequestList.md` から、機能的・非機能的な要件を個別の「原子要求」として抽出します。
2. **要求の具体化**: 各要求を、開発者が誤解なく実装でき、検証者が客観的にテスト可能なレベルまで精緻化します。
3. **合格基準の策定**: 各要求に対し、充足を確認するための具体的な「適格性確認テスト（SWE6）」の判定基準を定義します。
4. **ID体系の適用**: 各原子要求に **REQ-xxx**（例: REQ-001）形式の一意なIDを付与し、トレーサビリティの起点とします。
5. **要件仕様書の出力**: テンプレートに従い、`c:\AntiGravity\Gantt\SWE_report\SWE1\01_SRS.md` を出力します。

# アウトプット
- ソフトウェア要件仕様書 (SRS): `c:\AntiGravity\Gantt\SWE_report\SWE1\01_SRS.md`

# 制約事項
- 出力はすべて日本語で行うこと。
- 各要求には必ず **REQ-xxx** のIDを付与し、上位要求（顧客要件、CR）との紐付けを明記すること。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
