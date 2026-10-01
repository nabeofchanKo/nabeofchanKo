### Kosuke Hosoya

製薬・ゲーム・物流の3業界で約7年。現在はNTU（シンガポール）応用AI修士課程で、LLM・RAG・エージェントを使ったシステムを作っています。出力の根拠を人が検証できる形にすることを重視しています。

**Bilingual (JP/EN).** I build practical AI systems where technical implementation meets domain knowledge — with a focus on making the system's reasoning verifiable, not a black box.

- 🎓 M.S. Applied AI @ NTU Singapore (2026) ｜ 応用AI修士（NTUシンガポール・2026年修了見込）
- 🧭 ex-Pharmacovigilance · Game Analytics · Process Automation ｜ 医薬品の副作用評価・日英翻訳 / ゲームのデータ分析 / 物流業界での業務効率化・自動化
- 🌏 Native Japanese / Business English ｜ 日本語ネイティブ・英語ビジネスレベル

---

#### Selected projects

**[pv-rag-assistant](https://github.com/nabeofchanKo/pv-rag-assistant)** — 副作用報告の一次評価支援 / Pharmacovigilance triage assistant
症例報告を読み、重篤性（ICH E2A）・既知／未知・因果関係の評価案を根拠付きで作成し、担当者が確認・承認するワークフロー。報告漏れにつながる過小評価を出さないことを最優先に設計し、合成症例の評価で過小評価0件。[デモ公開中](https://h4b6m4zyqj.ap-northeast-1.awsapprunner.com/ja/triage)（登録不要）。
Drafts seriousness, expectedness and causality with the evidence behind each verdict, for a human to approve — 0 under-calls on its gold set. [Live demo](https://h4b6m4zyqj.ap-northeast-1.awsapprunner.com/en/triage), no sign-up.
`LangGraph` `FastAPI` `Next.js` `Chroma` `Docker` `AWS App Runner`

**[where-rag-breaks](https://github.com/nabeofchanKo/where-rag-breaks)** — RAGがどこで壊れるかの検証 / A benchmark for where classical RAG breaks
答えが本文テキスト以外（セルの塗り色・グラフ画像・暗号化ファイルなど11チャネル）にある正解ラベル付き合成コーパスで、古典的RAG・エージェント・ハイブリッドの3方式がどこで壊れるかを同条件で比較。コーパス規模を変えた際の挙動の違いまで測っている。
Measures which information channels break classical RAG, using a synthetic corpus with automatically-derived ground truth — and what an agent fixes, what it does not.
`Python` `BM25 + embeddings` `uv` `pytest`

**[equity-research-agent](https://github.com/nabeofchanKo/equity-research-agent)** — MCPベースのリサーチエージェント / MCP-based research agent
3つのMCPサーバーを連携させて株式リサーチレポートを自動生成。データ取得失敗時は副系統へ自動フォールバックし、出典タグを付けて検証可能な形で出力する。
Orchestrates three MCP servers into an equity-research report, with automatic fallback to a secondary data source and source-tagging so the output stays auditable.
`MCP (FastMCP)` `Python` `Plotly` `pytest`

**[applied-ai-sms-spam-pytorch](https://github.com/nabeofchanKo/applied-ai-sms-spam-pytorch)** — NLPをゼロから実装 / NLP from scratch
PyTorchで一から組んだBiLSTMと、ファインチューニングしたDistilBERTを比較。精度だけでなく、誤り方の違いとトレードオフまで検証した。
A BiLSTM baseline built from scratch vs. a fine-tuned DistilBERT, compared on error patterns and trade-offs — not just accuracy.
`PyTorch` `HuggingFace`

---

#### Tech

**Professional / 実務:** VBA · SQL / BigQuery · Power BI

**Personal & academic / 個人・学術:** Python · FastAPI · LangChain / LangGraph · OpenAI API · Chroma (RAG) · MCP (FastMCP) · PyTorch · Next.js / TypeScript · Docker · AWS (App Runner) · Git · pytest
