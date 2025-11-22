# kyushi-ronbun
Dataset of essay questions from Japan's former bar examination (the Conventional Bar Examination, 旧司法試験), 1949–2010.

## Overview

This repository provides a dataset of essay questions (論文式試験, *ronbun shiki shiken*) from the Conventional Bar Examination (旧司法試験, *kyu shiho shiken*), administered from 1949 (Showa 24) to 2010 (Heisei 22).

The texts have been carefully digitized, collated, and manually corrected using multiple printed sources to ensure accuracy, although minor discrepancies in punctuation, spacing, or formatting may remain compared to the original exam papers.

Cited article numbers and legal provisions reflect the statutes in effect **at the time of the examination**. Please be aware that they may differ from current laws due to subsequent amendments.

## File format

- **Encoding:** UTF-8
- **Line endings:** Unix (LF)
- **Content language:** Japanese
- **File format:** plain text (`.txt`)

Paragraph breaks in the original printed questions (often indicated by a one-character indentation at the beginning of a line) are normalized to plain newline characters.

## File naming convention

Filenames follow the pattern:

`kyushi_[subject]_[year]_[era]_[question_number].txt`

where:

- `subject`: abbreviated subject name
  - `gyoseiho`      – Administrative Law (行政法)
  - `hasanho`       – Bankruptcy Law (破産法)
  - `keiho`         – Criminal Law (刑法)
  - `keijiseisaku`  – Criminal Policy (刑事政策)
  - `keisoho`       – Code of Criminal Procedure (刑事訴訟法)
  - `kenpo`         – Constitution (憲法)
  - `kokusaikoho`   – Public International Law (国際公法)
  - `kokusaishiho`  – Private International Law (国際私法)
  - `minpo`         – Civil Law (民法)
  - `minsoho`       – Code of Civil Procedure (民事訴訟法)
  - `rodoho`        – Labor Law (労働法)
  - `shoho`         – Commercial Law (商法)
- `year`: Gregorian calendar year, e.g. `1949`, `2010`
- `era`: Japanese era code in the form `[s|h][nn]`, e.g.
  - `s24` for Showa 24 (1949)
  - `h01` for Heisei 1 (1989)
  - `h22` for Heisei 22 (2010)
- `question_number`: question index within a given subject and year, e.g. `q1`, `q2`

Example:

`kyushi_minpo_1949_s24_q1.txt` (昭和24年度 旧司法試験 論文式試験問題 民法 第1問)
