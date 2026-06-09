# company_inner_search_app

デプロイ手順
1. GitHub に push（既に完了）
2. Streamlit Community Cloud で新しいアプリを作成。リポジトリ: https://github.com/pmdybpr4ch-sketch/rag-agent-searching-document-ai-app.git
   - ブランチ: `main`
   - メインファイル: `main.py`
3. Advanced settings:
   - Secrets（APIキー）: `OPENAI_API_KEY` をダッシュボードのSecretsに登録
   - Python バージョン: 3.11 を指定（または `requirements.txt` に合わせる）
4. デプロイ後、ログを確認して動作を検証

ローカルで動かす場合（.env に API キーを設定）:
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
export OPENAI_API_KEY="..."
streamlit run main.py
```
