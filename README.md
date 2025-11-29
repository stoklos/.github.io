# Match-3 Auto-Battler Prototype

This repository hosts the early scaffolding for a Match-3 plus auto-battler game prototype. The project blends tile-matching puzzles with automated combat resolution, focusing on quick drafting and dynamic team-building.

## Game Concept
- **Core loop:** Players clear gems on a Match-3 board to generate resources and trigger abilities. Matched sets feed directly into unit actions or energy that fuels special skills.
- **Auto-battler layer:** Units deploy and fight automatically between puzzle turns. Synergies, positioning, and upgrade paths influence how effectively resources convert into combat power.
- **Run structure:** Sessions progress through short encounters, allowing players to draft units, unlock traits, and refine builds based on the puzzles they complete.
- **Pacing goals:** Fast turns with clear feedback, encouraging experimentation with both board strategy and team composition.

## Repository Structure
The repository is organized to separate core gameplay logic, rendering, content, and tooling:
- `src/` – Game logic, simulation systems, rendering layer, and UI components.
- `assets/` – Art, audio, fonts, and other static content.
- `configs/` – Balance data, unit definitions, and tuning tables in JSON/YAML.
- `scripts/` – Developer utilities (linting, formatting, build helpers).
- `tests/` – Automated tests for game logic and utilities.
- `docs/` – Design notes, technical specs, and feature RFCs.
- `build/` – Generated production artifacts (kept out of version control when possible).

## Build and Run Prerequisites
- **Node.js** (LTS) and **npm** or **yarn** for managing dependencies and running build tooling.
- **Git** for cloning and contributing.
- Optional: **TypeScript** type definitions installed globally if you prefer `ts-node`-based workflows.

## Installation
1. Clone the repository: `git clone https://github.com/<your-org>/.github.io.git`
2. Enter the project folder: `cd .github.io`
3. Install dependencies:
   - With npm: `npm install`
   - With yarn: `yarn install`

## Development Workflow
1. Start the development server for rapid iteration:
   - `npm run dev` or `yarn dev`
2. Run tests to validate gameplay systems and utilities:
   - `npm test` or `yarn test`
3. Lint and format code before committing:
   - `npm run lint` / `npm run format` (or the equivalent yarn scripts)
4. Build a production bundle for deployment:
   - `npm run build` or `yarn build`
5. Preview the built site locally if needed (adjust command to your tooling):
   - `npm run preview` or `yarn preview`

## Contributing
- Open an issue to discuss significant changes or feature proposals.
- Create feature branches and keep commits focused and descriptive.
- Include tests or add test cases when modifying gameplay logic or utilities.
- Run linting, formatting, and the full test suite before opening a pull request.
- Provide concise PR descriptions outlining the problem, solution, and validation steps.

## Roadmap Notes
- Implement the Match-3 board interaction layer and resource routing.
- Add the auto-battler combat simulator with unit synergies and positioning rules.
- Integrate UX flows for drafting, upgrading units, and progressing between encounters.
- Expand documentation in `docs/` as features mature.
