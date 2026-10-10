# lean = ponytail + antislop

Satu skill, ~550 token. Kode minimal (reuse dulu, tulis baru terakhir) + tulisan tanpa pola khas AI.
Format standar SKILL.md, jadi jalan di semua agent yang mendukung Agent Skills.

## Instalasi

| Tool | Caranya |
|---|---|
| Semua agent (skills CLI) | `npx skills add TaufikArsandi/lean` |
| Claude.ai / app | Zip folder `skills/lean` lalu upload di pengaturan Skills |
| Claude Code (semua project) | Salin `skills/lean` ke `~/.claude/skills/lean/` |
| Claude Code (satu project) | Salin `skills/lean` ke `.claude/skills/lean/` lalu commit, tim ikut dapat |
| Cursor | Salin isi SKILL.md ke `.cursor/rules/lean.mdc` |
| Windsurf / Cline | `.windsurf/rules/lean.md` / `.clinerules/lean.md` |
| Codex & agent lain | Tempel isi SKILL.md ke `AGENTS.md` |

Mau selalu aktif di Claude Code (bukan hanya saat cocok)? Tambahkan satu baris di `CLAUDE.md`: `Always follow the lean skill.`

## Pakai

- Otomatis saat ngoding/menulis, atau panggil `/lean`
- Ganti mode: `lean lite`, `lean full`, `lean ultra`
- Matikan: `stop lean`
