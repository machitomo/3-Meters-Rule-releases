# 3 Meters Rule! v0.0.1

南極の雪原で、人懐っこいペンギンを避けながら観測基地へ帰るGame Boy Color用ゲームです。
全3ステージを順番にクリアして、合計クリア時間を縮めてみてください。

## ファイル

- `3_meters_rule.gbc`: ゲームROM
- `3_meters_rule_cover.png`: スタート画面風のパッケージ絵
- `README.md`: この遊び方

## 起動

ZIPを展開して、mGBAの「ファイル → ROMを開く」、またはSameBoyのROMを開く操作から `3_meters_rule.gbc` を選びます。
iPhoneのDeltaでは「＋」から「Files」を選び、ROMを読み込んでください。
Game Boy Color専用です。通常の白黒Game Boyには対応していません。

## 操作

| ボタン | 操作 | mGBA標準キー |
|---|---|---|
| 十字キー | 8方向移動 | 矢印キー |
| A | 所持アイテムを使用 | X |
| B | 押している間ダッシュ | Z |
| START | 開始・ポーズ・再開・リトライ | Enter |
| SELECT | ポーズ・失敗・最終結果からタイトルへ | 設定したキー |

黄色い雪上車から轍をたどり、赤い屋根の基地へ帰ります。近道も可能です。
各ステージでペンギンに3回触れるとゲームオーバーです。ペンギンは攻撃できません。
滑る前に身を低くするので、構えを見て横へ避けてください。
スタミナが尽きたらBを離すと回復します。

物資は近づくと拾い、一度に1個だけ持てます。Aで使います。
赤い魚袋はペンギンを誘導、青いスノーシューは深雪の減速を無効化、黄色いコンパスは基地の方向を示します。
ポーズ画面でも各アイテムの用途を確認できます。
ステージをクリアすると次へ自動で進み、全3ステージ後に合計タイムを表示します。セーブ機能はありません。

## Deltaの表紙

PNGをiPhoneの「ファイル」または写真ライブラリに保存し、Deltaのゲーム一覧でゲームを長押しします。
**Change Artwork → Files** または **Photo Library** から `3_meters_rule_cover.png` を選びます。
表紙はROMとは別に設定します。
参考: [Delta公式](https://faq.deltaemulator.com/about/press-kit)、[画像選択の公式実装](https://github.com/rileytestut/Delta/blob/main/Delta/Game%20Selection/GameCollectionViewController.swift)。

## 配布・確認状況

最新版: https://github.com/machitomo/3-Meters-Rule-releases/releases/latest

GBDK-2020 4.5.0でビルドした32 KiBのROMです。リリース時にヘッダー・チェックサムとmGBAの自動検証を実行します。
GBC実機・SameBoy・iOS版Deltaでの最終確認は未実施です。
パッケージ絵は内蔵imagegenで制作しました。
