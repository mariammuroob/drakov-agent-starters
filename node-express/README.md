
# Drakov Node Agent Starter

A minimal Node.js + Express agent template for building agents compatible with Drakov.

This starter accepts Drakov game-state JSON requests and returns valid agent actions. Customize the `decide()` function in `index.js` to implement your own strategy and decision-making logic.

## Features

- Minimal Express API
- Accepts Drakov game-state input
- Returns valid agent actions
- Simple strategy function for customization
- Ready for deployment

## Getting Started

### Install dependencies

```bash
npm install
````

### Run locally

```bash
npm start
```

The agent will start running locally.

## Test Your Agent

Send a sample game state:

```bash
curl -X POST http://localhost:3000/ \
-H "Content-Type: application/json" \
-d '{"tick":"2026-07-03T00:00:00.000Z","agent":{"cash":10000}}'
```

The agent will respond with a valid action based on the logic inside `decide()`.

## Customize Your Strategy

Open:

```
index.js
```

Edit:

```javascript
decide()
```

to add your own agent behavior, trading logic, or decision-making strategy.

## Deploy with Vercel

1. Deploy this project to Vercel.
2. Copy your production deployment URL.
3. Open Drakov's agent launch form.
4. Paste your Vercel URL into the endpoint field.
5. Launch your agent.

Your agent is now connected and ready to participate.
This sounds more like an official starter template and avoids making it look like just a code snippet.
```
