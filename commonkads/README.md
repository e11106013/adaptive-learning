## CommonKADS

### 設計重點說明
- SKILL.md 觸發描述 刻意列出多個同義詞（KBS、知識工程、專家系統...），因為 CommonKADS 用語不普遍，需要積極觸發。
- 漸進式載入（Progressive Disclosure） SKILL.md 只保留六模型的骨架與導引，細節全部在 references/ 子文件中。
- LLM 只有在需要某個模型的深度分析時，才讀取對應文件，避免把大量內容一次塞進記憶體。
- 工作表驅動 CommonKADS 本身就是工作表方法論，skill 設計也完全遵循這個邏輯——每個分析步驟都有對應的填寫範本，讓 Claude 能引導用戶系統地完成分析而不遺漏。

### 目錄結構
```
commonkads/
├── SKILL.md                          ← 主觸發文件（常駐記憶體）
└── references/
    ├── organization-model.md         ← OM 工作表 OM-1~OM-6 詳細指引
    ├── task-agent-model.md           ← TM + AM 詳細指引
    ├── knowledge-model.md            ← KM + RM 建模指引
    └── templates/
        └── worksheet.md             ← 完整分析工作表（可直接填寫）
```          

### 使用方式(下載至語言模型對應 skills 目錄)
```
git clone <repo-url> .[claude/codex/gemini/]skills/commonkads
```

### 在 Claude Code / Codex / Gemini CLI 中使用 `/` 指令：

```
/commonkads | "完整的說明你要的需求與遭遇到的工程問題"

```
### 執行過程與結果
[https://github.com/e11106013/adaptive-learning/edit/main/commonkads/result.md
](https://github.com/e11106013/adaptive-learning/blob/main/commonkads/results.md)

## License
MIT
