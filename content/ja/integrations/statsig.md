---
app_id: statsig
app_uuid: 57fb9235-151d-4ed9-b15e-a3e6f918dcca
assets:
  integration:
    configuration: {}
    events:
      creates_events: true
    metrics:
      check: statsig.log_event.count
      metadata_path: metadata.csv
      prefix: statsig.
    service_checks:
      metadata_path: assets/service_checks.json
    source_type_name: Statsig
author:
  homepage: https://github.com/DataDog/integrations-extras
  name: 不明
  sales_email: support@statsig.com
  support_email: support@statsig.com
categories: []
dependencies:
- https://github.com/DataDog/integrations-extras/blob/master/statsig/README.md
display_on_public_website: true
draft: false
git_integration_title: statsig
integration_id: statsig
integration_title: Statsig
integration_version: ''
is_public: true
kind: integration
manifest_version: 2.0.0
name: statsig
oauth: {}
public_title: Statsig
short_description: Datadog で Statsig の変更を監視する
supported_os:
- linux
- macos
- windows
tile:
  changelog: CHANGELOG.md
  classifier_tags:
  - Supported OS::Linux
  - Supported OS::macOS
  - Supported OS::Windows
  configuration: README.md#Setup
  description: Datadog で Statsig の変更を監視する
  media: []
  overview: README.md#Overview
  support: README.md#Support
  title: Statsig
---



## 概要

Datadog-Statsig インテグレーションにより、Statsig でイベントおよびメトリクスを送信できるようになるため、製品やサービスを監視し、機能のロールアウトまたはコンフィギュレーションの変更がエコシステムに与える影響を可視化できます。

## セットアップ

### インストール

Statsig のインテグレーションセットアップにインストールは必要ありません。

### コンフィギュレーション

1. Datadog API キーをコピーします。
2. [Statsig コンソールで Integrations タブに移動します][1]。
3. Datadog カードをクリックします。
4. 上部のフィールドに API キーを貼り付け、Confirm をクリックします。

## 収集データ

Statsig インテグレーションでは、Datadog からのデータは収集されません。

### メトリクス
{{< get-metrics-from-git "statsig" >}}


### サービスのチェック

Statsig インテグレーションには、サービスのチェック機能は含まれません。

### イベント

Statsig インテグレーションにより、Statsig でのコンフィギュレーション変更イベントが Datadog に送信されます（たとえば、更新された機能ゲートまたは新しいインテグレーション）。

## トラブルシューティング

ヘルプが必要ですか？[Statsig サポート][3]にお問い合わせいただくか、[Statsig ウェブサイト][4]をご覧ください。

## その他の参考資料

お役に立つドキュメント、リンクや記事:

- [Datadog マーケットプレイスの Statsig の提供とモニター機能のリリース][5]

[1]: https://console.statsig.com/integrations
[2]: https://github.com/DataDog/integrations-extras/blob/master/statsig/metadata.csv
[3]: mailto:support@statsig.com
[4]: https://www.statsig.com/contact
[5]: https://www.datadoghq.com/blog/feature-monitoring-statsig-datadog-marketplace/