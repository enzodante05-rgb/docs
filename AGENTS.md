# CryptoBot documentation — agent instructions

## About this project

This is the documentation site for **CryptoBot**, a TypeScript-based automated cryptocurrency trading bot.

- Docs are built with [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Run `mint dev` to preview locally at `http://localhost:3000`

## Bot infrastructure

| Resource | Value |
|---|---|
| VPS IP | `178.156.149.251` |
| SSH access | `ssh root@178.156.149.251` |
| VPS codebase | `/opt/cryptobot/` |
| Local mirror | `~/Documents/_cryptobot_vps/` |
| Deploy command | `cd ~/Documents/_cryptobot_vps && ./deploy.sh` |
| pm2 process | `cryptobot` |
| Logs | `/root/.pm2/logs/cryptobot-out.log` |

## Bot dev rules (never violate these)

- Edit `.ts` files in `~/Documents/_cryptobot_vps/` — never in `dist/`
- Deploy with `./deploy.sh` after any change
- Restart: `pm2 restart cryptobot --update-env`
- Check status: `pm2 logs cryptobot --lines 50 --nostream`

## Docs structure

| File | Purpose |
|---|---|
| `index.mdx` | Introduction and overview |
| `quickstart.mdx` | Connect to VPS and verify bot |
| `development.mdx` | Edit and deploy source changes |
| `deployment.mdx` | pm2 operations and log access |
| `docs.json` | Site config (name, colors, navigation) |

## Style preferences

- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Terminology

- Say "bot" not "daemon" or "service"
- Say "deploy" not "push" when referring to `./deploy.sh`
- Say "VPS" not "server" or "remote"
- Say "source files" not "TypeScript files" (though TypeScript is fine in technical contexts)
