---
layout: project
title: "Xserver Free VPS Auto-Renewal Script"
title_ja: "Xserver無料VPS自動更新スクリプト"
description: "Automates the manual renewal process of Xserver's free VPS every 2 days using Selenium browser automation, enabling permanent usage."
description_ja: "Xserver無料VPSの「2日ごと手動更新」を自動化し、永続利用を可能にするPythonスクリプトです。"
permalink: /xservervps/
github_url: "https://github.com/superdoccimo/xservervps"
image: /assets/logo.png
---

## 概要

2025年7月にリリースされたXserver無料VPSは、4GBのRAMと3コアのCPUという高性能ながら、2日ごとの手動更新が必要です。このPythonスクリプトは、Seleniumを使用してブラウザ操作を自動化し、面倒な更新作業から解放します。

### 年間約14,000円の節約効果

このスクリプトを使えば、月額1,190円の有料プランに相当する環境を無料で維持でき、年間で約14,000円のコストを削減できます。

## 主な特徴

- **完全自動化**: ログインから更新完了まで、すべて自動で実行します。
- **スマートな実行**: 更新可能な時間帯だけを狙って動作し、無駄がありません。
- **エラーハンドリング**: 万が一失敗した場合は、スクリーンショットを保存して原因究明を助けます。
- **ヘッドレス対応**: サーバー環境でもバックグラウンドで静かに動作します。

## 動作要件

- Python 3.7以上
- Google Chrome
- ChromeDriver
- Xserver無料VPSアカウント

## 設定方法

スクリプト内の設定項目に、ご自身のXserverアカウント情報（ユーザー名、パスワード、サーバーID）と、最後に手動更新した日時を正確に入力するだけで準備は完了です。

## なぜ自動化が重要か？

Xserver無料VPSは、そのままだと2日ごとに手動で更新ボタンを押さないとサーバーが削除されてしまいます。この「うっかり忘れ」のリスクをなくし、開発や実験に集中できる環境を永続的に確保することが、このプロジェクトの目的です。

Dockerを使った複雑な環境の構築、AI関連のツール（Claude Code, ComfyUIなど）の検証、あるいは単に自分だけのオンライン実験場として、この無料VPSのポテンシャルを最大限に引き出しましょう。
