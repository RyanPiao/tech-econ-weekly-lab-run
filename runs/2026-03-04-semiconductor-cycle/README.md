# Run: 2026-03-04 Semiconductor Cycle (Mon–Wed)

This run completes Monday/Tuesday/Wednesday portions of the 7-day research cadence.

## Completed
- **Day 1 (Mon):** `docs/DAY1_problem_framing.md`
- **Day 2 (Tue):** `docs/DAY2_data_extraction_spec.md`, `docs/DAY2_preanalysis_lock.md`, `scripts/day2_ingest_build_panel.py`
- **Day 3 (Wed):** `scripts/day3_eda.py`, `docs/DAY3_eda_note.md`, outputs in `outputs/`

## Core data
- `IPG3344S` (semiconductor/electronic component production index)
- `USINFO` (all employees: information)
- `PAYEMS` (total nonfarm payroll)

## Main Day 3 signals
- Corr(chip_yoy, software_emp_yoy) = **0.3534**
- Strongest lag (0..6): **3 months**, corr = **0.3860**

## Re-run
```bash
python3 scripts/day2_ingest_build_panel.py
python3 scripts/day3_eda.py
```
