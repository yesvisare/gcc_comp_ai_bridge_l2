# Bridge: M4.1 → M4.2 Validation

## Purpose

This bridge validates your readiness to move from:
- **M4.1:** Model Cards & AI Governance
- **M4.2:** Vendor Risk Assessment

**Type:** Readiness Validation

---

## What This Bridge Validates

### Readiness Checks (4 total)

1. **Model Card Artifacts**
   - Pass Criteria: Model card exists, contains required sections (metadata, performance, bias_assessment, intended_use), bias metrics documented, governance approval recorded
   - Purpose: Confirms completion of M4.1 model documentation system

2. **Governance Framework Documentation**
   - Pass Criteria: Governance committee charter exists, cross-functional roles included, NIST AI RMF mapping exists, EU AI Act alignment exists
   - Purpose: Validates governance structure and compliance framework from M4.1

3. **Conceptual Understanding**
   - Pass Criteria: Can explain model cards, describe bias metrics (demographic parity, equalized odds), explain HITL workflows, articulate NIST vs EU AI Act differences
   - Purpose: Ensures understanding of M4.1 governance concepts before extending to vendors

4. **Environment Setup for M4.2**
   - Pass Criteria: Python 3.9+ installed, required packages available (pandas, requests, json), Jupyter functional, file I/O permissions verified
   - Purpose: Confirms Python environment is ready for vendor risk assessment tools

---

## How to Run

### Prerequisites
- Completed M4.1
- Python 3.9+
- Jupyter Notebook

### Steps

**Windows (PowerShell):**
```powershell
cd Bridge_L3_M4_1_to_M4_2
$env:PYTHONPATH = "$PWD"
jupyter notebook
```

**Mac/Linux:**
```bash
cd Bridge_L3_M4_1_to_M4_2
export PYTHONPATH="$PWD"
jupyter notebook
```

**Then:**
1. Open `Bridge_L3_M4_1_to_M4_2_Readiness.ipynb`
2. Run all cells (`Cell → Run All`)
3. Check results

---

## Pass Criteria

**To proceed to M4.2, you must:**
- ✓ All 4 checks pass
- ✓ No critical gaps (✗)
- ✓ Understand concepts covered

**If checks fail:**
1. Read failure messages (they include fixes)
2. Complete missing work from M4.1
3. Re-run bridge

---

## Common Issues

### Issue: Missing artifacts
**Symptoms:** `✗ Missing: model_cards/rag_model_card.json`
**Fix:** Re-run M4.1 model card exercise to generate artifact

### Issue: Missing governance docs
**Symptoms:** `✗ Missing: Governance committee charter`
**Fix:** Complete M4.1 governance documentation exercise

### Issue: Environment not set up
**Symptoms:** `✗ pandas missing`
**Fix:** `pip install pandas`

### Issue: Conceptual gaps
**Symptoms:** Can't answer readiness questions
**Fix:** Review M4.1 conceptual materials (model cards, bias detection, HITL, compliance frameworks)

---

## Time Estimate

- **First time:** 20-30 minutes
- **If all checks pass:** 10-15 minutes
- **If rework needed:** 30-60 minutes

---

## Support

**If stuck:**
- Review M4.1 materials
- Check failure messages (they include fixes)
- Reach out: support@techvoyagehub.com

---

## Next Steps

**After passing all checks:**
→ Proceed to **M4.2: Vendor Risk Assessment**

**Module M4.2 will cover:**
- **Vendor Evaluation Matrix** — Weighted scoring across 5 categories (Security 30%, Privacy 25%, Compliance 20%, Reliability 15%, Data Residency 10%)
- **Automated DPA Review Tool** — Validates 12 essential GDPR Article 28 clauses
- **Subprocessor Tracking System** — Maps vendor dependency chains
- **Continuous Vendor Monitoring** — Tracks certification expiration, uptime, incidents, term changes
