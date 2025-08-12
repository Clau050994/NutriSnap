# NutriSnap 🍽📷
A personal app that estimates calories from a picture of your plate.

## Overview
NutriSnap is a personal project that combines computer vision and nutrition data to help estimate the calories in a meal from a single or dual photo.  
It detects the foods on your plate, classifies them into categories, estimates portions, and calculates calories using a nutrition database.

---

## Features
- 📸 **Snap a photo** of your plate
- 🥗 **Detect foods** with segmentation
- 🏷 **Classify dishes** into known categories
- ⚖ **Estimate portions** using a reference object (optional)
- 🔢 **Calculate calories** via USDA FoodData
- ✏ **Manually adjust** portion sizes and calories
- 💾 **Log results** locally for review

---

## Tech Stack
**Frontend**
- React (Vite or Next.js)
- Axios for API calls

**Backend**
- FastAPI (Python)
- ONNX Runtime for optimized inference
- Pillow & NumPy for image processing

**Data**
- USDA FoodData Central API
- Food-101 / UECFOOD-256 / FoodSeg103 datasets for training

---

## How It Works
1. User uploads or takes a photo of a meal.
2. The backend model performs:
   - Food segmentation
   - Classification of each detected item
   - Portion estimation (via depth or reference object)
3. Nutrition data is retrieved for each food item.
4. Calorie counts are calculated and displayed in the UI.
5. The user can adjust any portion or calorie value.

---

## Future Enhancements
- Monocular depth for portion estimation
- Personal calorie history & trend tracking
- Recipe ingredient breakdown
- Offline inference on mobile

---

## License
This project is for personal and educational use only. Not intended for medical advice.
