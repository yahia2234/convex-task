# Convex Energy – Trade Reconciliation Case Study

This repository contains my solution to the trade reconciliation case study provided by Convex Energy as part of the application process.

## 📊 Problem Summary

Convex provided two datasets:
- **Internal Trade Data**: Records of internal power trades including monthly and quarterly contracts.
- **Clearer Trade Data**: Monthly settled trades as reported by the clearing house.

### Objective

The goal is to **reconcile the internal and clearer trade data** at a monthly level by:
1. **Decomposing** (cascading) the quarterly internal trade into three monthly components.
2. **Combining** any overlapping monthly trades (e.g., April and May appear in both monthly and quarterly trades).
3. **Netting and comparing** the internal monthly positions with those reported by the clearer.

---

## ✅ Steps Performed in the Notebook

1. **Loaded the data** using `pandas`.
2. **Identified the quarterly contract** (`Q225`) and decomposed it into equal monthly trades for April, May, and June.
3. **Merged** monthly internal trades with decomposed quarterly legs.
4. **Netted** internal monthly positions by summing quantities and computing weighted average prices.
5. **Compared** the internal monthly summary to the clearer data.
6. **Highlighted mismatches**, if any, in quantity or price.

---

## 📁 Files

- `Yahia_Rady_Convex_Reconciliation.ipynb`: The Jupyter notebook with all steps, code, and explanations.

---

## 🧑‍💻 Author

**Yahia Rady**  
Email: yahiaradi78@gmail.com 
Date: June 2025

---

