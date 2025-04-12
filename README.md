# Assignment_02


## 項目概述

`Assignment_02` 是一個展示 GitHub 功能與自動化測試的示例項目。本項目旨在展示如何使用 GitHub 進行代碼管理、問題追蹤和自動化測試，涵蓋以下功能：
- 創建和管理分支（`hw1-p` 和 `hw1-f`）
- 設置並運行 GitHub Actions 進行自動化測試
- 創建 Pull Requests 並進行互動評論
- 設置 Issue 模板並提交問題報告

## 環境要求

- **Python**: 3.8 或以上版本
- **依賴**:
  - `pytest`（用於單元測試）
  - `flake8`（用於代碼風格檢查）



## 使用說明

### 1. 運行測試
- 本項目使用 `pytest` 進行單元測試，測試文件位於 `test_main.py`。
- 運行以下命令執行測試：
  pytest

### 2. 分支管理
- **主分支**：`main`（包含穩定代碼）
- **功能分支**：
  - `hw1-p`：用於提交正確代碼並通過 GitHub Actions 測試
  - `hw1-f`：用於提交錯誤代碼以展示測試失敗

### 3. GitHub Actions
- 工作流程文件位於 `.github/workflows/test.yml`，在每次 Pull Request 提交時自動運行。
- 包含以下測試：
  - 代碼風格檢查（`flake8`）
  - 單元測試（`pytest`）

### 4. Issue 模板
- 本項目設置了 Bug Report 模板，位於 `.github/ISSUE_TEMPLATE/bug_report.md`。
- 創建 Issue 時可選擇此模板，規範問題報告格式。

## 貢獻指南

1. 創建新分支：
   git checkout -b <分支名稱>

2. 提交更改並推送：
   git add .
   git commit -m "描述您的更改"
   git push origin <分支名稱>

3. 創建 Pull Request 並等待審查。

## 聯繫方式

如有問題，請通過 GitHub Issues 提交，或聯繫項目維護者。
