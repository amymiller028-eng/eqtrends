# EQ Research & Insights

Redesign concept for **talentsmarteq.com/research-insights**, opening with an
interactive "how does your EQ compare?" tool built on the 2021–2026 norm.

**Live:** https://amymiller028-eng.github.io/eqtrends/

| File | What it is |
|---|---|
| `index.html` | The page. Header, hero, the tool, three article cards. |
| `explorer.html` | The tool on its own, no page chrome. Embeddable. |

Both HTML files are self-contained — the data is embedded, nothing is fetched
at runtime, and the only external request is Google Fonts.

The underlying CSV tables are **deliberately not published here**. The full
level x function x industry table has 1,078 cells containing a single person,
where the cell average is that person's exact score next to their job level,
function and industry. Those tables stay internal, in
`OneDrive - TalentSmart6-EQTrends-Norms\`.

## The norm

720,271 Emotional Intelligence Appraisal **Self Edition** assessments,
2021–2026. Re-Assessment retakes excluded. Book-code and online pooled.
Scored on all 28 items, `raw total / 168 × 100`.

n = 720,271 · mean **74.48** · median **75.00** · mode **76.19** · SD **9.40**
· skew −0.382.

## The two findings

**Job level.** EQ climbs the ladder then turns down at the very top.
Employee/Associate 73.40 → Supervisor 74.93 → Manager 75.92 → Director 76.74 →
**Executive/VP 76.91 (peak)** → Senior Executive 76.86 → C Level 76.67 →
**President or CEO 75.35**. Owner/Founder (72.01) and Independent Consultant
(71.81) sit lowest, but those are self-employed rather than more senior — a
separate pattern, not the top of the same ladder.

This revises the 2003 technical manual, which reported EQ declining from
director level upward. Director now sits near the peak; the decline starts at
President/CEO.

**Job function.** **Sales averages 75.91, +1.43 above the norm, 3rd highest of
25 functions**, against Finance/Accounting 74.19 and IT 73.76. The 2003 manual
reported sales as not significantly different from those two.

## Read the differences as small

All eight demographic fields together explain **5.9%** of the variation in EQ
scores. At this n almost every gap is significant; spread across job levels is
about 5 points, across functions about 4 — roughly half of one SD. These are
unadjusted slices with nothing held constant between groups.

## Open items

- **Fonts are placeholders.** Archivo + IBM Plex Sans stand in for the real
  talentsmarteq.com faces, which could not be read off the site. They are
  `--font-display` and `--font-body` at the top of each file — a two-line swap.
- **Article images are original SVG artwork** in brand colors, not photography.
  Placeholders for layout feel.
- **Cards 2 and 3** reuse titles from the current Research & Insights page and
  should be swapped for the real companion articles.
- **Codebook versions inferred** from observed code ranges — Job Level v2 (11),
  Job Function v3/v5 (25), Industry v3 (30). Each matches exactly, but worth a
  confirm with the data team.
