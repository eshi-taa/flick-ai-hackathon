# Flickd AI Hackathon — Smart Tagging & Vibe Classification

👋 Hello! I'm **Eshita**, a 3rd-year Computer Science student at SASTRA University.  
This is my submission for the **Flickd AI Hackathon**.

---

## 📦 Project Overview

This project tackles the challenge of:
- 🧠 Vibe classification using natural language
- 🛍️ Product matching from fashion video frames using CLIP + FAISS
- 📄 Outputting structured results in the format specified by Flickd

---

## 🧰 Tech Stack

- Python (CLIP, FAISS, spaCy, NumPy, PIL)
- YOLOv8 (for object detection — run externally)
- CLIP embeddings + cosine similarity
- FAISS IndexFlatIP for fast product lookup

---

## 🗂️ Folder Structure

flickd-ai-hackathon/
├── data/ # keywords.json, vibeslist.json, etc.
├── embeddings/ # product_catalog.npy and product_ids.npy
├── output/ # final_output.json, matched images and results
├── scripts/ # match.py, vibes.py, generate_output.py
├── models/ # (optional) yolov8 weights
├── README.md # ← this file
└── requirements.txt


---

## ✅ How to Run

```bash
# Step 1: Product Matching
python scripts/match.py

# Step 2: Vibe Classification
python scripts/vibes.py

# Step 3: Generate final output
python scripts/generate_output.py
```

## Output will be saved at:

output/final_output.json

## Output Format:

{
  "video_id": "2025-06-02_11-31-19_UTC",
  "vibes": ["Boho", "Y2K"],
  "products": [
    {
      "type": "dress",
      "color": "black",
      "match_type": "Exact Match",
      "matched_product_id": "15003",
      "confidence": 0.91
    }
  ]
}

📹 Demo
🖥️ Loom Demo: [Insert Your Loom Link Here]

🙋 About Me
I’m excited about machine learning, computer vision, and real-world AI applications.
Thanks for the opportunity to contribute to Flickd’s future tech stack! 🌟


---

## 🚀 STEP 2: Push to GitHub

### ✅ If You Haven’t Initialized a Git Repo Yet

1. Open terminal or Git Bash in your project folder  
2. Run:

```bash
git init
git add .
git commit -m "Initial commit - Flickd AI Hackathon"
git branch -M main
git remote add origin https://github.com/eshi-taa/flick-ai-hackathon.git
git push -u origin main

```





