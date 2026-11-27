# renovate-config

yagihash のリポジトリで共通の [Renovate](https://docs.renovatebot.com/) 設定（shareable config preset）。

## 使い方

各リポジトリの `renovate.json` で、この preset を `extends` に指定する。

```json
{
  "$schema": "https://docs.renovatebot.com/renovate-schema.json",
  "extends": ["github>yagihash/renovate-config"]
}
```

リポジトリ固有の設定（言語ごとのパッケージのグルーピング、`ignorePaths` など）は、各リポジトリの `renovate.json` に追加で書く。

## 注意

- このリポジトリは public。Mend Renovate のホスト版アプリは、private リポジトリの preset を public リポジトリから参照できないため。
- リポジトリは gh-infra で管理している（[yagihash/.github](https://github.com/yagihash/.github) の `repos/repositoryset.yaml`）。
