---
name: SWE5
description: ソフトウェアアーキテクチャ設計（COMP）に基づき、コンポーネント間の連携を検証（ブラックボックステスト：SWE.5）します。
---

# 目的
統合された複数のソフトウェアユニット（コンポーネント）間の相互作用が、アーキテクチャ設計で定義されたインターフェース仕様および動的挙動に適合していることを検証し、システムとしての整合性を証明すること。

# インプット
- ソフトウェアアーキテクチャ設計書: `c:\AntiGravity\Gantt\SWE_report\SWE2\02_SoftwareArchitectureDesign.md`
- ソースコード（ビルド済み/稼働状態）: `c:\AntiGravity\Gantt\main.py`
- 報告書テンプレート: `c:\AntiGravity\Gantt\SWE_agent\SWE5\TEMPLATE.md`

# 手順
1. **統合テスト設計**: コンポーネント間のインターフェース仕様（COMP）に基づき、データの受け渡しや状態遷移の正常性を確認するブラックボックス検証項目を作成します。
2. **テスト環境の構築**: ブラウザツール（Flask）が動作可能であることを確認し、必要に応じて検証用エンドポイントを利用します。
3. **検証の実行**: 統合テストを実行し、複数のコンポーネントが連携して意図した機能（表示の更新、タブの同期等）を提供できているかを確認します。
4. **追跡性の付与**: 各テストケースがどの **COMP-xxx**（またはインターフェース）に対応するかを明示します。
5. **検証報告書の出力**: テンプレートに従い、`c:\AntiGravity\Gantt\SWE_report\SWE5\05_SoftwareIntegrationVerificationReport.md` を出力します。

# アウトプット
- 統合テストコード/スクリプト: `c:\AntiGravity\Gantt\test.py`
- ソフトウェア統合検証報告書: `c:\AntiGravity\Gantt\SWE_report\SWE5\05_SoftwareIntegrationVerificationReport.md`

# 制約事項
- 出力はすべて日本語で行うこと。
- 各テストケースには **IT-xxx**（例: IT-001）形式の一意なIDを付与すること。
- 内部ロジックではなく「結合部分の挙動」および「設計通りの連携」に着目して検証すること。
- **必ず指定された TEMPLATE.md の構造を維持すること。**
 village
