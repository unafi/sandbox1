# Mermaid 全種類サンプル集

---

## 1. フローチャート（Flowchart）

```mermaid
flowchart TD
    A[開始] --> B{条件}
    B -->|Yes| C[処理1]
    B -->|No| D[処理2]
    C --> E[終了]
    D --> E[終了]
```

---

## 2. シーケンス図（Sequence Diagram）

```mermaid
sequenceDiagram
    participant User
    participant System
    User->>System: リクエスト送信
    System-->>User: レスポンス返却
```

---

## 3. クラス図（Class Diagram）

```mermaid
classDiagram
    class User {
        +string name
        +string email
        +login()
    }

    class Order {
        +int id
        +date createdAt
        +calculateTotal()
    }

    User "1" --> "*" Order : places
```

---

## 4. 状態遷移図（State Diagram）

```mermaid
stateDiagram
    [*] --> Idle
    Idle --> Active : start
    Active --> Idle : stop
    Active --> Error : fail
    Error --> Idle : reset
```

---

## 5. ER 図（Entity Relationship Diagram）

```mermaid
erDiagram
    USER ||--o{ ORDER : places
    ORDER ||--|{ ORDER_ITEM : contains
    PRODUCT ||--o{ ORDER_ITEM : included_in
```

---

## 6. ガントチャート（Gantt Chart）

```mermaid
gantt
    title プロジェクト計画
    dateFormat  YYYY-MM-DD

    section 設計
    要件定義 :a1, 2025-01-01, 5d
    基本設計 :after a1, 5d

    section 開発
    実装 :2025-01-15, 10d
    テスト :2025-01-25, 7d
```

---

## 7. パイチャート（Pie Chart）

```mermaid
pie title 市場シェア
    "A社" : 40
    "B社" : 35
    "C社" : 25
```

---

## 8. Git グラフ（Git Graph）

```mermaid
gitGraph
    commit
    commit
    branch feature
    checkout feature
    commit
    checkout main
    merge feature
```

---

## 9. Journey（ユーザージャーニー図）

```mermaid
journey
    title ユーザー体験
    section 購入プロセス
      商品検索: 3: User
      比較検討: 4: User
      購入: 5: User
```

---

## 10. Mindmap（マインドマップ）

```mermaid
mindmap
  root(計画)
    目標
      売上向上
      顧客満足度
    手段
      広告
      改善
        UI改善
        FAQ強化
```

---

## 11. Timeline（タイムライン）

```mermaid
timeline
    title プロジェクトの歴史
    2024 : 構想開始
    2025 : 開発開始
    2026 : リリース
```

---

## 12. Quadrant Chart（象限チャート）

```mermaid
quadrantChart
    title 優先度マトリクス
    x-axis 低い --> 高い
    y-axis 緊急 --> 非緊急

    "重要かつ緊急" : [0.8, 0.2]
    "重要だが非緊急" : [0.8, 0.8]
    "緊急だが重要でない" : [0.2, 0.2]
    "重要でも緊急でもない" : [0.2, 0.8]
```

---

# ✅ PNG 画像埋め込みサンプル

```md
![サンプル画像](sample.png)
```

---

# ✅ ASCII アート図（Markdown 純正）

```
+-------+
| Start |
+-------+
    |
    v
+----------+
| Process  |
+----------+
```

