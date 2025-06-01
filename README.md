# Ansible × GitHub Actions で EC2 に Nginx 自動構築

##  概要

このリポジトリは、**Ansible + GitHub Actions を使って AWS EC2 に Nginx を自動構築**する演習プロジェクトです。  
IaC（Infrastructure as Code）と CI/CD（継続的インテグレーション/デリバリー）の技術習得を目指しています。

---

## 構成技術

| 技術       | 内容                                           |
|------------|------------------------------------------------|
| AWS        | EC2 (Amazon Linux 2 or 2023)                   |
| Ansible    | Nginx の構築を自動化する構成管理ツール        |
| GitHub Actions | mainブランチへの push をトリガーにCI/CD実行 |

---

## ディレクトリ構成

```bash
ansible-nginx-demo/
├── inventory                # Ansible のインベントリファイル（EC2のIP指定）
├── nginx.yml               # Ansible プレイブック（Nginx構築処理）
└── .github/

