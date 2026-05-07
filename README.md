# TalentShow_AJ.ruj

> A fake Human Benchmark reaction time test website — for entertainment and live show performances.

Built with Vite + React + TypeScript + Tailwind CSS, this app mimics the look and feel of [humanbenchmark.com](https://humanbenchmark.com)'s reaction time test, but with a twist: the displayed reaction time is remotely controlled via an API backend.

## How It Works

The app polls a remote Express API (the [Talentshow Backend](https://github.com/JustDev-08/Talentshow.aj.ruj-Backend-)) every 500ms to fetch two values:

- `script_number` — the "reaction time" (in milliseconds) to display
- `title` — a boolean flag; when `true`, the screen shows an ending slide

During a live show, an operator sends values to the backend via the [Control Client](https://github.com/JustDev-08/Talentshow.aj.ruj-Client-), and the displayed reaction time updates in real time — making it appear as if the subject has an impossibly fast (or pre-determined) reaction.

## Tech Stack

- **Framework:** Vite + React 19
- **Language:** TypeScript
- **Styling:** Tailwind CSS v4
- **Sound:** `use-sound`
- **Icons:** Lucide React

## Getting Started

```bash
npm install
npm run dev
```

The app runs at `http://localhost:5173`.

To change the backend URL, edit the `fetch` call in `src/App.tsx:167`.

## Related Repos

- [Talentshow Backend](https://github.com/JustDev-08/Talentshow.aj.ruj-Backend-) — Express API
- [Talentshow Client](https://github.com/JustDev-08/Talentshow.aj.ruj-Client-) — Control panel to send values

## License

For educational and entertainment purposes.
