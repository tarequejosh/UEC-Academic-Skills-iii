# FedUA-Net Presentation Slides (IWAIT 2027)

**Presenter:** Md Tareque Jamil Josh\*  
**Supervisor:** Prof. Hiroki Takahashi\*\*  
\* *UEC Exchange Study Program (JUSST Program), The University of Electro-Communications, Tokyo, Japan*  
\*\* *Department of Informatics, Graduate School of Informatics and Engineering, UEC Tokyo*

---

## 1. Overview & Guidelines Compliance

These presentation slides have been crafted in accordance with the guidelines specified in `Slides/Guidance/`:
- **`presentation slides setting.pdf`**:
  - **Clean White Background:** Pure `#FFFFFF` canvas with zero distracting patterns or unrelated clipart.
  - **16:9 Aspect Ratio:** Master coordinates at 1920x1080 with auto-scaling to fit any projector or display.
  - **Color Contrast:** Dark Slate (`#0f172a`) and Dark Blue for body text; Green for improvements/winners; Red for limits/warnings; Purple for conformal theory.
  - **No ALL-CAPS:** Proper Title Case and Sentence Case throughout to maintain legibility.
  - **Font Size & Style:** High-legibility modern Sans-Serif font with bold hierarchy (>24-30pt equivalent for all major content).
  - **Action Titles:** Every content slide has an informative takeaway statement rather than a generic section heading.
  - **1 to 2 Messages per Slide:** Structured visual cards, badges, and comparison tables with highlighted winners rather than walls of text.
  - **Scientific Cover Slide:** Exactly formatted to match the UEC JUSST program guidelines.
  - **Slide Numbering:** Slide counter (`X / 12`) on every content slide footer.
- **`Effective slides and presentation.pdf`**:
  - Paced for a 10–15 minute conference oral talk (12 slides total: ~1 minute per slide).
  - Integrated presenter notes with verbatim speaking cues for every slide.

---

## 2. Slide Deck Structure (12 Slides)

| Slide | Action Title / Topic | Key Visuals & Findings |
|---|---|---|
| **01** | **Title Slide (Cover Packaging)** | Author info, JUSST program, Prof. Takahashi, UEC Tokyo |
| **02** | Hospitals hold distinct imaging modalities, but privacy prevents centralizing data | 3-site breakdown (MRI, US, X-ray) & privacy barrier |
| **03** | Standard federated learning breaks down under disjoint labels, scale imbalance, and overconfidence | 3 numbered bottlenecks |
| **04** | FedUA-Net shares the feature extractor globally while keeping normalization and heads local | Large architecture diagram (`FedUA_Methodology.png`) + shared vs local breakdown |
| **05** | Equal client weighting prevents the X-ray site from dominating ultrasound training | Visual proportion bar ($w_k = 1/3$ vs $w_k = N_k / \sum N_j$) |
| **06** | We evaluate across 29,145 scans in 11 non-overlapping classes against five FL baselines | Booktabs dataset table & protocol |
| **07** | FedUA-Net improves scarce ultrasound accuracy by +3.1% and achieves the lowest raw calibration error | Full-width Table 1 (booktabs style) |
| **08** | Equal weighting recovers +30% ultrasound accuracy and stays resilient down to 100 images | Large `fig2_results.png` + quantitative highlights |
| **09** | Per-site temperature scaling cuts calibration error by 39% without sharing validation data | Equation + 5.04% $\rightarrow$ 3.07% ECE drop |
| **10** | Proposition 1 proves that high coverage forces high referral when accuracy is lower | Formal bound: $\text{Referral Rate} \ge \|c - a\|$ & proof intuition |
| **11** | LAC reaches 98.3% MRI and 97.9% X-ray accuracy on automated singletons | Booktabs Table 2 + `fig3_conformal.png` |
| **12** | FedUA-Net enables safe, balanced collaboration across heterogeneous hospital silos | 3-point summary, GitHub link, Q&A |

---

## 3. How to Present (Interactive Shortcuts)

Open `Slides/index.html` in any modern web browser (Google Chrome, Microsoft Edge, Firefox, Safari):

- **Next Slide:** `Right Arrow`, `Space`, or `Page Down`
- **Previous Slide:** `Left Arrow`, `Backspace`, or `Page Up`
- **First / Last Slide:** `Home` / `End`
- **Toggle Fullscreen:** Press `F`
- **Toggle Presenter Notes:** Press `P` or `S` (displays scripted speech notes for Md Tareque Jamil Josh)
- **Slide Overview / Jump Drawer:** Press `O` (shows grid of all slides to jump instantly)
- **Touch / Mobile:** Swipe left or right

---

## 4. How to Export to PDF

To generate a standalone PDF presentation deck:
1. Open `Slides/index.html` in Google Chrome or Microsoft Edge.
2. Press `Ctrl + P` (or Cmd + P on macOS).
3. Set **Destination:** `Save as PDF`.
4. Set **Layout:** `Landscape`.
5. Set **Margins:** `None`.
6. Under **More settings:** Check `Background graphics`.
7. Click **Save** to export pixel-perfect 16:9 slides.
