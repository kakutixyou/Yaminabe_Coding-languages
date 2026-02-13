# 🍲 Tech Yaminabe (技術闇鍋ジェネレーター)

技術スタックの相性を可視化し、カオス度を測定する面白ツールです。  
Claude、ChatGPT、Gemini、おじさんAI、Aiderなど、様々なAIペルソナが技術選定にコメントします。

![Tech Yaminabe Demo](./demo.gif) <!-- デモGIFがないため追加できない -->

## ✨ 特徴

- 🤖 **5種類のAIペルソナ**: Claude、ChatGPT、Gemini、おじさんAI、Aiderがそれぞれの視点で技術を選択
- 📊 **3つの評価指標**:
  - 🛠️ 作りやすさ (0-100)
  - 📚 勉強のしやすさ (0-100)
  - 🚀 仕方なくスペースシャトルのように一部のデータを削除する/年
- 🌀 **カオス度計算**: 技術の相性から自動計算
- 💬 **ユーモラスなコメント**: 技術の組み合わせに応じた面白いコメントを表示

## 🚀 使い方

### インストール
```bash
# リポジトリのクローン
git clone [https://github.com/kakutixyou/Yaminabe_Coding-languages.git](https://github.com/kakutixyou/Yaminabe_Coding-languages.git)

# ディレクトリへ移動
cd Yaminabe_Coding-languages

# 依存関係のインストール (Node.js環境を想定)
npm install

# アプリの起動
npm start

ブラウザで `http://localhost:3000` を開きます。

### 基本的な使い方

1. **AIに選ばせる**: Claude、ChatGPT、Gemini、おじさんAI、Aiderから選択
2. **手動で選ぶ**: 「自分で具材を選ぶ」から技術を選択
3. **おまかせ**: ランダムに6つの技術を選択
4. **AI考察**: 選択した技術スタックをAIが分析

## 📁 プロジェクト構成

```
Yaminabe/
├── public/
│   └── index.html
├── src/
│   ├── components/
│   │   └── TechYaminabe.jsx    # メインコンポーネント
│   ├── data/
│   │   ├── masterData.json      # 技術スタックデータ
│   │   └── Aiselections.json    # AI選択肢とメトリクス
│   ├── App.js
│   └── index.js
├── package.json
└── README.md
```

## 🎨 カスタマイズ

### 新しい技術を追加

`src/data/masterData.json` を編集:

```json
{
  "techStack": {
    "frontend": [
      {
        "name": "新しい技術",
        "specialty": "特徴",
        "compatibility": ["相性の良い技術"],
        "antiCompatibility": ["相性の悪い技術"],
        "difficulty": 3
      }
    ]
  }
}
```

### 新しいAIペルソナを追加

`src/data/Aiselections.json` を編集:

```json
{
  "aiSelections": {
    "newAI": {
      "name": "新AI名",
      "color": "#hexcolor",
      "emoji": "🤖",
      "modes": {
        "mode1": {
          "name": "モード名",
          "description": "説明",
          "techs": ["技術1", "技術2"],
          "comment": "AIのコメント",
          "emoji": "😎",
          "metrics": {
            "buildability": 70,
            "learnability": 65,
            "shuttlesPerYear": 2.5
          }
        }
      }
    }
  }
}
```

## 🤝 コントリビューション

プルリクエスト大歓迎です！以下の流れでお願いします：

1. このリポジトリをフォーク
2. 新しいブランチを作成 (`git checkout -b feature/amazing-feature`)
3. 変更をコミット (`git commit -m 'Add some amazing feature'`)
4. ブランチにプッシュ (`git push origin feature/amazing-feature`)
5. プルリクエストを作成

### 貢献のアイデア

- 新しい技術の追加
- 新しいAIペルソナの追加
- UIの改善
- バグ修正
- 多言語対応

## 📝 ライセンス

このプロジェクトは [MIT License](LICENSE) の下で公開されています。

## 👤 作者

GitHub: @kakutixyou


## 🙏 謝辞

- このプロジェクトはReactで構築されています
- AIペルソナのアイデアは各AIアシスタントの特徴から着想を得ています
- 「闇鍋」という日本の料理文化にインスパイアされました

## ⚠️ 免責事項

このツールはエンターテインメント目的です。  
実際のプロジェクトでの技術選定は、要件や制約を十分に検討した上で行ってください。

---

**楽しい技術闇鍋ライフを！** 🍲✨
「※このアプリの使用による精神的苦痛について、作者は一切の責任を負いません」
