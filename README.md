# Komorebi — 神社と森のプロシージャルマップ（Codex版）

WebGPUで描く、ブラウザで歩ける神社と森の3Dシーンです。画像・3Dモデル・音声ファイルは一切使わず、地形も社殿も音もすべてコードで生成しています（単一の `index.html`、約100KB）。

**▶ Play: https://kouki0822.github.io/shrine-forest-map-codex/**

## これは何か

話題になった Abyssal Garden（97KBの単一HTMLで泳げる水中世界）と同じ作り方を、別のAIモデルで再現する比較実験の Codex 版です。

- 初回プロンプトは Claude 版と完全に同一（`prompt.txt` に全文を掲載）
- 制作：Codex（GPT-6.1 Sol、reasoning effort xhigh）
- Claude 版（Claude Code / Opus 5.5）：https://kouki0822.github.io/shrine-forest-map/

WIP（制作途中）です。見た目と性能の最終検品はこれからで、数値はすべて未検証です。

## 動作環境

- WebGPU 対応ブラウザが必要です（デスクトップ／モバイルの Chrome、Edge など）
- WebGPU が使えない場合は、その旨のメッセージが画面に表示されます

## 操作

- PC：WASD 移動、マウスで視点、Q/E で下降／上昇、Shift で加速、1〜6 で視点ジャンプ
- スマホ：1本指を押し続けると前進、指を滑らせると視点移動、2本目の指を触れると加速。画面のメニューから視点や画質も選べます
- 画質は Low / Medium / High の3段階で、端末に合わせて自動選択されます（スマホは Low〜Medium、PCは High から開始）。重い場合は描画解像度が自動で調整されます。
