# Data Repository Guide for Journal Submission

## 📋 What the Journal Needs

The journal asks for: **"DOI or URL at which your data is deposited"**

You need to upload your supplementary materials to a public data repository and provide the DOI/URL.

---

## 🎯 **Recommended Option: Zenodo** (Most Common for Academic Papers)

### **Why Zenodo?**
✅ **Free** and widely used in academia  
✅ **Provides DOI** automatically (required by journals)  
✅ **Permanent** archive (data won't disappear)  
✅ **Unlimited storage** for datasets <50GB  
✅ **Integrates** with GitHub (optional)  
✅ **Accepted** by all journals including AAI

---

## 🚀 **Step-by-Step: Upload to Zenodo**

### **Step 1: Create Zenodo Account**
1. Go to https://zenodo.org
2. Click "Sign Up" (or log in with GitHub/ORCID)
3. Verify your email

### **Step 2: Create New Upload**
1. Click "Upload" button (top right)
2. Click "New Upload"

### **Step 3: Upload Files**
Upload these 3 files:
- ✅ `bangladesh_sme_final_with_split.csv` (your dataset)
- ✅ `bd_sme_credit_pipeline_enhanced.ipynb` (your notebook)
- ✅ `README.txt` (plain text version, better for non-technical viewers)

**Optional:** Also upload `requirements.txt` for easy installation

### **Step 4: Fill Metadata**

**Upload type:** Dataset

**Title:** 
```
Supplementary Materials: When Machine Learning Fails - Establishing Boundary Conditions for Applied AI in SME Credit Risk Assessment
```

**Authors:** (Add all three with ORCID IDs)
```
Anmita Das (0009-0000-1401-0494)
Sushanta Paul (0009-0007-8071-6971)
Shoumya Chowdhury (0009-0005-5552-1094) [Corresponding]
```

**Description:** (Copy from README or use this)
```
This dataset contains anonymized data and reproducible code for the paper "When Machine Learning Fails: Establishing Boundary Conditions for Applied AI in SME Credit Risk Assessment" submitted to Applied Artificial Intelligence.

Contents:
- Dataset: 200 Bangladesh SME loan applications with 27 features
- Notebook: Complete analysis pipeline demonstrating ML failure modes under data constraints
- Documentation: Comprehensive README with reproduction instructions

Key Finding: Despite rigorous methodology (leakage prevention, cross-validation, regularization), all models achieve near-random performance (ROC-AUC 0.44-0.49), establishing empirical boundary conditions for ML applicability in credit risk.

Citation: Das, A., Paul, S., & Chowdhury, S. (2026). When Machine Learning Fails: Establishing Boundary Conditions for Applied AI in SME Credit Risk Assessment. Applied Artificial Intelligence (In review).
```

**Keywords:** (Add 5-10)
```
machine learning, credit risk, SME finance, boundary conditions, negative results, data quality, cross-validation, emerging markets, Bangladesh, responsible AI
```

**License:** 
```
Creative Commons Attribution Non Commercial 4.0 International (CC BY-NC 4.0)
```

**Access:** Public (immediately open access)

### **Step 5: Reserve DOI**
- Click "Reserve DOI" before publishing
- This generates a DOI you can use in your paper submission **immediately**
- Format: `10.5281/zenodo.XXXXXXX`

### **Step 6: Publish**
- Click "Publish"
- Your files are now permanently archived with a DOI!

### **Step 7: Get Your DOI/URL**
After publishing, you'll get:
- **DOI:** `https://doi.org/10.5281/zenodo.XXXXXXX`
- **URL:** `https://zenodo.org/record/XXXXXXX`

**Use the DOI in your journal submission!**

---

## 📝 **What to Enter in Journal Submission Form**

When the journal asks for **"DOI or URL at which your data is deposited"**, enter:

```
https://doi.org/10.5281/zenodo.XXXXXXX
```

(Replace XXXXXXX with your actual Zenodo DOI number)

**Example:**
```
https://doi.org/10.5281/zenodo.7654321
```

---

## 🔄 **Alternative Options** (If You Don't Want Zenodo)

### **Option 2: Figshare**
- Similar to Zenodo (free, provides DOI)
- Website: https://figshare.com
- Steps: Similar to Zenodo
- Also widely accepted

### **Option 3: Open Science Framework (OSF)**
- Free, provides DOI
- Website: https://osf.io
- Good for large projects
- Steps: Create project → Upload files → Generate DOI

### **Option 4: GitHub + Zenodo**
- Upload to GitHub repository
- Connect to Zenodo for DOI
- Good if you want version control
- Guide: https://guides.github.com/activities/citable-code/

### **Option 5: Institutional Repository**
- Check if University of Melbourne has a data repository
- May provide DOI
- Contact: research-data@unimelb.edu.au (example)

---

## ⚠️ **What NOT to Do**

❌ **Don't use:** Google Drive, Dropbox, personal websites
- No DOI (journals require DOI)
- Not permanent (links can break)
- Not archival (files can be deleted)

❌ **Don't use:** GitHub alone (without Zenodo)
- GitHub doesn't provide DOIs by default
- Files can be deleted/changed
- But GitHub + Zenodo integration is perfect!

---

## 📦 **Files to Upload (Checklist)**

Essential (upload these 3):
- [ ] `bangladesh_sme_final_with_split.csv` (dataset)
- [ ] `bd_sme_credit_pipeline_enhanced.ipynb` (notebook)
- [ ] `README.txt` or `README_SUPPLEMENTARY_MATERIALS.md` (documentation)

Optional but recommended:
- [ ] `requirements.txt` (for easy installation)
- [ ] Output figures (if generated): `calibration_analysis.png`, `roc_pr_curves.png`, etc.

Do NOT upload:
- ❌ Paper manuscript (that goes to journal separately)
- ❌ Cover letter
- ❌ Old/test versions of files

---

## ✅ **After Uploading**

### **1. Update Your Paper**
Add a "Data Availability" statement in your manuscript:

```latex
\section*{Data Availability Statement}

The dataset and code supporting this study are openly available at Zenodo: 
\url{https://doi.org/10.5281/zenodo.XXXXXXX}
```

### **2. Add to Your CV**
```
Dataset: Das, A., Paul, S., & Chowdhury, S. (2026). 
Supplementary Materials: When Machine Learning Fails. 
Zenodo. https://doi.org/10.5281/zenodo.XXXXXXX
```

### **3. Share the Link**
- Twitter/LinkedIn: "Our paper + reproducible code now available!"
- Research Gate: Add to your publications
- Email to collaborators

---

## 🎓 **Example Zenodo Entries (For Reference)**

Good examples of data deposits:
1. https://doi.org/10.5281/zenodo.3873835 (ML dataset)
2. https://doi.org/10.5281/zenodo.4562349 (Credit risk data)
3. https://doi.org/10.5281/zenodo.5579087 (Code + data)

These show best practices for:
- Clear titles
- Complete metadata
- Good documentation

---

## ⏱️ **Time Estimate**

- **Zenodo account creation:** 5 minutes
- **File upload:** 5 minutes (files are small)
- **Metadata entry:** 10 minutes
- **Review and publish:** 2 minutes

**Total: ~20-25 minutes**

---

## 🆘 **Troubleshooting**

### **Q: What if upload fails?**
A: Files are small (<10MB total), should work fine. Check internet connection.

### **Q: Can I update files after publishing?**
A: You can create a new version with updated DOI. Original version stays archived.

### **Q: What if reviewers request changes?**
A: Create new version in Zenodo, update DOI in revised manuscript.

### **Q: Is this really free?**
A: Yes! Zenodo is funded by CERN and EU, completely free for academic use.

### **Q: What if I don't have ORCID?**
A: Create one at https://orcid.org (takes 2 minutes, free, essential for academics)

---

## 📧 **Need Help?**

- **Zenodo Support:** https://zenodo.org/support
- **Zenodo FAQ:** https://help.zenodo.org
- **University Research Data Office:** Check your institution's support

---

## ✅ **Quick Summary**

1. ✅ Go to https://zenodo.org
2. ✅ Create account
3. ✅ Upload 3 files (CSV + notebook + README.txt)
4. ✅ Fill metadata (title, authors, description, keywords, license)
5. ✅ Publish
6. ✅ Copy DOI
7. ✅ Paste DOI into journal submission form

**You'll have your DOI in ~25 minutes!**

---

**Good luck with your data deposit!** 🚀

After you get your Zenodo DOI, just paste it into the journal submission form when they ask for "DOI or other location of your data."
