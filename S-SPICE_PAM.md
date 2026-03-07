---
name: S-SPICE_PAM( G-SPICE 0.0.1)
description: S-SPICE (G-SPICE 0.0.1) プロセスアセスメントモデル定義書。
---

# S-SPICE プロセスアセスメントモデル (PAM) 定義書

## 1. 概要
S-SPICE (G-SPICE 0.0.1) は、Automotive SPICE 4.0 をベースとしつつ、LLM（大規模言語モデル）エージェントによる開発の自律性とトレーサビリティを最大化するために最適化されたプロセスモデルです。本書は、各プロセスの目的、主要な活動、成果物、および現在のプロジェクトにおける準拠状況を定義します。

## 2. プロセス能力評価 (Process Capability Assessment)

### プロセスグループ全体の推計準拠率: **92%**
### 現在の能力レベル: **能力レベル 3 (Established)** 相当

| プロセス ID | 名称 | 主要成果物 | 準拠率 | ステータス |
| :--- | :--- | :--- | :--- | :--- |
| **MAN.3** | プロジェクト管理 | `00_ProjectPlan.md` | 95% | Fully Handled |
| **MAN.5** | リスク管理 | `05_RiskManagementReport.md` | 90% | Fully Handled |
| **SWE.1** | ソフトウェア要件分析 | `01_SRS.md` | 95% | Fully Handled |
| **SWE.2** | アーキテクチャ設計 | `02_SoftwareArchitectureDesign.md` | 90% | Fully Handled |
| **SWE.3** | 詳細設計・実装 | `03_SoftwareDetailedDesign.md` | 95% | Fully Handled |
| **SWE.4** | ユニット検証 | `04_SoftwareUnitVerificationReport.md` | 90% | Fully Handled |
| **SWE.5** | 統合検証 | `05_SoftwareIntegrationVerificationReport.md` | 90% | Fully Handled |
| **SWE.6** | 適格性確認テスト | `06_SoftwareQualificationTestReport.md` | 95% | Fully Handled |
| **SUP.9** | 問題管理 | `09_ProblemManagementList.md` | 90% | Fully Handled |
| **SUP.10** | 変更要求管理 | `10_ChangeRequestList.md` | 85% | Handled |
| **PIM.3** | プロセス改善 | `10_ProcessImprovementRecord.md` | 95% | Fully Handled |

## 3. プロセス詳細定義 (Process Definitions)

### 3.1 管理プロセス群 (Management Process Group)

#### **MAN.3 プロジェクト管理 (Project Management)**
- **目的**: プロジェクトの目標を達成するために必要な活動を特定、立案、監視し、リソースを適切に割り当てること。
- **主要活動**: 多段階計画の立案、スケジューリング、進捗監視。
- **主要成果物**: `00_ProjectPlan.md`

#### **MAN.5 リスク管理 (Risk Management)**
- **目的**: プロジェクトの成功を阻害する不確実な事象を継続的に特定、分析、評価し、対策を講じること。
- **主要活動**: リスク特定、影響・確率評価、RK-ID管理、軽減策策定。
- **主要成果物**: `05_RiskManagementReport.md` (ID: RK-xxx)

### 3.2 ソフトウェアエンジニアリングプロセス群 (Software Engineering Process Group)

#### **SWE.1 ソフトウェア要件分析 (Software Requirements Analysis)**
- **目的**: 顧客要求を分析し、具体的かつ検証可能なソフトウェア要件へと具体化すること。
- **主要活動**: 原子要求抽出、REQ-ID付与、検証基準定義。
- **主要成果物**: `01_SRS.md` (ID: REQ-xxx)

#### **SWE.2 ソフトウェアアーキテクチャ設計 (Software Architecture Design)**
- **目的**: ソフトウェア要件をコンポーネントに分解し、責任範囲とインターフェースを定義すること。
- **主要活動**: コンポーネント分割、インターフェース設計、COMP-ID管理。
- **主要成果物**: `02_SoftwareArchitectureDesign.md` (ID: COMP-xxx)

#### **SWE.3 ソフトウェア詳細設計・実装 (Software Detailed Design & Implementation)**
- **目的**: 具体的ロジックを設計し、それに基づくソースコードを作成すること。
- **主要活動**: 詳細設計 (DD-ID)、コーディング、上位追跡性確保。
- **主要成果物**: `03_SoftwareDetailedDesign.md` (ID: DD-xxx), `main.py`

#### **SWE.4 ソフトウェアユニット検証 (Software Unit Verification)**
- **目的**: 最小単位が詳細設計通りに動作することをコードレベルで検証すること。
- **主要活動**: ユニットテスト (UT-ID) 設計・実行、ホワイトボックステスト。
- **主要成果物**: `04_SoftwareUnitVerificationReport.md` (ID: UT-xxx)

#### **SWE.5 ソフトウェア統合検証 (Software Integration Verification)**
- **目的**: コンポーネント間の連携を検証し、インターフェースの整合性を証明すること。
- **主要活動**: 統合テスト (IT-ID)、ブラックボックス検証。
- **主要成果物**: `05_SoftwareIntegrationVerificationReport.md` (ID: IT-xxx)

#### **SWE.6 ソフトウェア適格性確認テスト (Software Qualification Testing)**
- **目的**: 完成した製品が全ての要件 (REQ) を充足していることを証明すること。
- **主要活動**: 要件適合性テスト (QT-ID)、エンドユーザー視点検証。
- **主要成果物**: `06_SoftwareQualificationTestReport.md` (ID: QT-xxx)

### 3.3 支援・改善プロセス群 (Support & Improvement Process Group)

#### **SUP.9 問題管理 (Problem Management)**
- **目的**: 不具合や課題を特定・記録し解決までを管理すること。
- **主要活動**: PR-ID起票、原因分析、ステータス追跡。
- **主要成果物**: `09_ProblemManagementList.md` (ID: PR-xxx)

#### **SUP.10 変更要求管理 (Change Request Management)**
- **目的**: 問題変更が必要な場合に正式な変更要求を介して要求・設計に反映すること。
- **主要活動**: CR-ID管理、影響分析、要件(REQ)へのフィードバック。
- **主要成果物**: `10_ChangeRequestList.md` (ID: CR-xxx)

#### **PIM.3 プロセス改善 (Process Improvement)**
- **目的**: プロセスの定義自体を継続的に分析し改善すること。
- **主要活動**: 実行分析、SKILL.md更新、IMP-ID管理。
- **主要成果物**: `10_ProcessImprovementRecord.md` (ID: IMP-xxx)

---
**定義承認日**: 2026-03-07
**アソシエーション**: G-SPICE Global Standard
 village
