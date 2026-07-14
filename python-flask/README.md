Drakov Python Agent Starter
A minimal Flask agent that accepts Drakov game-state JSON and responds with a valid save_cash action. Edit decide() in app.py to add your strategy.

Deploy with Vercel

Run locally
python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate
pip install -r requirements.txt
python app.py
Test it:

curl -X POST http://localhost:3000/ \
  -H "Content-Type: application/json" \
  -d '{"tick":"2026-07-03T00:00:00.000Z","agent":{"cash":10000}}'
After deployment, copy the Vercel production URL and paste it into Drakov's /launch form.