# Terraform AWS EC2 Project

## 概要

このプロジェクトはTerraformを使用してAWS上にEC2インスタンスとセキュリティグループを構築するIaC構成です。

インフラをコードとして管理し、再現性と自動化を目的としています。

---

## アーキテクチャ

- EC2インスタンス（Amazon Linux / Ubuntu）
- セキュリティグループ（SSH: 22番ポート許可）
- デフォルトVPCを使用

---

## 使用技術

- Terraform
- AWS (EC2, Security Group)
- HCL（HashiCorp Configuration Language）

---

## 設計ポイント

- インフラをコード化し、手動構築を排除
- セキュリティグループでSSHアクセスを最小限に制限
- Terraformにより再現可能な構成を実現

---

## 前提条件

以下がインストール・設定済みであること

- AWS CLI設定済み
- Terraformインストール済み
- AWSアカウントとアクセスキー設定済み

---

## 実行手順（デプロイ〜削除まで）

```bash
terraform init
terraform plan
terraform apply
terraform destroy

※AWS課金を防ぐため、検証後は必ずリソースを削除してください。
