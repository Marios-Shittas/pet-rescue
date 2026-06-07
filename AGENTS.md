# Expo HAS CHANGED

Read the exact versioned docs at https://docs.expo.dev/versions/v56.0.0/ before writing any code.

## Agent Usage

Purpose: concise guidance for AI coding agents working in this repository.

- **Workspace root**: operate from the repository root.
- **Common run commands**: use the project's npm scripts in `package.json`:
	- `npm start` → starts the Metro/Expo dev server (`expo start`)
	- `npm run ios` → build & run on iOS (`expo run:ios`) — requires macOS + Xcode
	- `npm run android` → build & run on Android (`expo run:android`) — requires emulator or device
	- `npm run web` → start web (`expo start --web`)
	- `npm run reset-project` → repo-specific reset script (`scripts/reset-project.js`)

- **Where to look first**:
	- App entry and routing: `src/app` (Expo Router)
	- Project configuration: `app.json`, `tsconfig.json`, `package.json`
	- Native build files: `android/` and `ios/` (avoid changing without explicit instruction)

- **Agent behavioral guidelines**:
	- Prefer linking to existing docs (README, this file, CLAUDE.md) rather than copying large sections.
	- Make minimal, focused PRs. Explain rationale for any native changes and ask before altering `android/` or `ios/`.
	- When recommending commands to the user, include exact npm scripts (e.g., `npm start`).

If you need more specific agent instructions (scoped to tests, CI, or native builds), ask and I will add a targeted customization file.
