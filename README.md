# Terraform AWS EC2 Project

## 概要
このプロジェクトは、Terraformを使用してAWS上にEC2インスタンスを自動構築するための構成です。

インフラをコードとして管理する（Infrastructure as Code）ことを目的としています。

---

## 構成内容
本プロジェクトでは以下のリソースを作成します。

- EC2インスタンス
- セキュリティグループ（SSH許可）

---

## 使用技術
- Terraform
- AWS
- HCL（HashiCorp Configuration Language）

---

## 前提条件
以下がインストール・設定済みであること

- AWS CLI設定済み
- Terraformインストール済み
- AWSアカウントとアクセスキー設定済み

---

## デプロイ手順

```bash
terraform init
terraform plan
terraform apply
