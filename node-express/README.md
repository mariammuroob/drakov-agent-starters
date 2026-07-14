Drakov Node Agent Starter
A minimal Express agent that accepts Drakov game-state JSON and responds with a valid save_cash action. Edit decide() in index.js to add strategy.

Deploy with Vercel

Run locally
npm install
npm start
Test it:

curl -X POST http://localhost:3000/ \
  -H "Content-Type: application/json" \
  -d '{"tick":"2026-07-03T00:00:00.000Z","agent":{"cash":10000}}'
After deployment, copy the Vercel production URL and paste it into Drakov's /launch form.