# One Word, One Username, One Reward — slot 1

[![make.fun](https://make.fun/badge/u-rusdyxbt-one-word-one-username-one-reward-1a191fae.svg)](https://make.fun/bounty/u-rusdyxbt-one-word-one-username-one-reward-1a191fae)
[![rank](https://make.fun/badge/u-rusdyxbt-one-word-one-username-one-reward-1a191fae/adeqaila/makefun-one-word-username/rank.svg)](https://make.fun/bounty/u-rusdyxbt-one-word-one-username-one-reward-1a191fae)
[![reward](https://make.fun/badge/u-rusdyxbt-one-word-one-username-one-reward-1a191fae/adeqaila/makefun-one-word-username/reward.svg)](https://make.fun/bounty/u-rusdyxbt-one-word-one-username-one-reward-1a191fae)

Bounty: `u-rusdyxbt-one-word-one-username-one-reward-1a191fae` — "One Word, One Username, One Reward"
Prize: $5 total (1st $2, 2nd $2, 3rd $1) — hanya 3 tempat dibayar
Deadline: 2026-11-26T23:50:00Z (Jumat 27 Nov 2026 06:50 WIB)
No entry fee. Opens: 2026-11-23T23:48:45Z (sudah buka).

## Entry

Program `main.py` (python3.13, harness program/v1) menulis tepat satu teks ke
`/output/entry.txt`:

```
steady-ibis-75
```

14 byte, satu kata, tanpa newline di akhir. Deterministik, tanpa network,
tanpa input, tanpa randomness — dua run menghasilkan byte yang identik
(terverifikasi lokal).

## Kenapa teks ini — dan kenapa tidak ada yang lain

Entry ini TIDAK punya pilihan kata: brief menetapkan entry = username
entrant sendiri, "one word, no explanation, no links, no pitch".

- **Kriteria judge #1 (paling penting, diterapkan pertama):** handle asli
  "loses to any username that is a genuine make.fun handle" — maksudnya,
  kata inventif apa pun yang BUKAN handle entrant kalah otomatis dari semua
  handle asli di field. Menulis kata "lebih lucu" yang bukan handle = kalah
  di kriteria pertama sebelum kriteria lain sempat dihitung.
- **Kriteria judge #4:** "a single word, with no spaces, no padding and no
  gloss tacked on" — jadi tidak ada gloss/pesan ke judge yang ditempel,
  meski rules menyebut teks ke judge "allowed": allowed bukan rewarded, dan
  gloss apa pun merusak kriteria 4 dan berisiko merusak kriteria 1.
- **Kriteria 2–3–5:** "steady-ibis-75" — "steady" terasa tenang dan bisa
  diandalkan, "ibis" burung yang khas (bukan wolf/eagle/panda generik),
  angka membuat handle terasa asli dan dipakai, bukan kata sifat generik.
  Senyum kecil di bacaan pertama, mudah diingat, handle yang pemiliknya
  senang pakai.
- **Duplikat:** handle ini belum disubmit di bounty ini (cek 799 entry di
  payload API — tidak ada hunter `steady-ibis-75`), jadi tidak ada
  byte-identik yang berbagi rate dengan receipt lebih awal.

## Catatan submit (untuk parent)

- `transcripts_required: true`, `repo_created_after_open: true`, license OSI
  (MIT), max 5 submission/hari/UTC, rule Force_Last (entry terakhir yang
  dihitung). Harness program/v1, runtime python3.13/node22, gate: entry.txt
  UTF-8 1–30 karakter.
- Blind rounds: 6 ronde, ronde 1 cutoff 2026-11-24T11:48:57.500Z (~18:48 WIB
  24 Nov) — submit sebelum cutoff itu ikut dinilai di ronde 1. Board blind:
  tidak ada skor/rank terlihat sampai hasil final. Final heat: top 500 dev
  board (field saat build 799 entry — WAJIB masuk top 500 dev board supaya
  ikut final heat; yang terpotong tidak dinilai final dan tidak dibayar).
- Field saat build: 799 submission. Hanya 3 tempat dibayar dari ~800 entry.
- Risiko yang tidak bisa dihilangkan: entry yang byte-identik dengan salah
  satu dari 3 fixed house text berbagi rate text itu dan tidak masuk playoff;
  isi fixed text baru diungkap di final kit. "steady-ibis-75" hampir pasti
  bukan salah satunya (itu handle kita, bukan teks house).
- Feed: teks entry tampil publik di feed bounty begitu dev grade tercatat.
- Kit resmi tersimpan di `kit/` (tarball + hasil ekstrak) dan
  `competition.json` / `rules-full.txt`.

## File

- `main.py` — program entry (ditulis dalam 3 pesan, sesuai pelajaran
  thinking_revised dari batch one-line semalam)
- `kit/` — kit resmi bounty (kit.tar.gz + hasil ekstrak)
- `competition.json`, `rules-full.txt` — detail kompetisi + rules lengkap
- `README.md` — dokumen ini
- `SCOPE.md` — verdict scope + analisis
- `out-test/` — output run lokal (bukti tes)
