# ebook-audio · 變更日誌

---

## v3.0.2 — 2026-09-07

> v3.0.2 Fleet Alignment Upgrade by **Sean 10-repo-fleet** Worker

### Added
- `PRD/SPEC.md` 由 root `SPEC.md` rename + 升級 v2.2.1 → v3.0.2
- `PRD/SPEC.md` 頂部 v3.0.2 banner（維護者 = Sean 10-repo-fleet）
- `PRD/SPEC.md` §1–§9 補完 9 個標準章節（取代 v2.2.1 佔位符「詳見 §15」）
  - §1 產品概述（5 個子節，含 5 tier personas + 商業目標 + Non-Goals）
  - §2 使用者流程（mermaid + 4 場景）
  - §3 FR 表（8 個 FR，P0/P1/P2 三層）
  - §4 NFR（Performance / Security / Privacy / Accessibility）
  - §5 技術架構 + Module Map + 環境變數 + 降級策略
  - §6 DoD 6 條
  - §7 部署契約
  - §8 Out of Scope 5 條
  - §9 指向 CHANGELOG
- `PRD/SPEC.md` §16 部署契約（Pages 4-job CI + TTS 引擎降級策略 + BYOK）
- `PRD/SPEC.md` §17 監控（4 jobs + Lighthouse + TTS API 健康度）
- `PRD/SPEC.md` §18 維運（Patch/Minor/Major SOP + Release Checklist 含 4 引擎煙霧測試）
- `PRD/SPEC.md` §19 安全（EPUB 個資 + OWASP + 著作權 + 法規 + 免責聲明）
- `PRD/CHANGELOG.md` — 本檔
- `.github/workflows/ci.yml` — 4-job CI（link-check / no-op lint / no-op test / deploy → Pages）

### Preserved
- v2.2.1 §15 深度市調完整保留（6 個變現 tier ARR 預估、競品分析 7 家、quadrantChart 定位、Unit Economics LTV/CAC=21、4 維評分 78/100）
- `dashboard.html`（14.7 KB 主程式）— 一字不改

### Notes
- 預設分支 = `main`
- 部署目標 = GitHub Pages（純靜態 HTML，無需 npm build）
- Pages URL: `https://openclawsean024-create.github.io/ebook-audio/`
- 純前端 BYOK 模式（4 個 TTS 引擎：Web Speech / Edge TTS / ElevenLabs / Azure）
- 無需後端 secret / Vercel token
- Sprint 2 啟動時程：2026-10-19

---

## v2.2.1 — 2026-07-11

- Sophia CPO 撰寫規格書
- §1-§13 為佔位符（指向 §15）
- §15 深度市調完整（最終商業化評分 78/100）
- 對接技術：Alan (CTO) + Hermes Agent
- Demo：TBD（待 Sprint 1 部署）

---

## v2.0 — 2026-XX-XX

- 4 個 TTS 引擎選型確認
- 5 個變現 tier 初步規劃

---

## v1.0 — 2026-XX-XX

- 純前端 EPUB → MP3 工具初版
- Web Speech API 單一引擎
