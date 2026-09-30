# ⚡ FitBuddy: AI-Powered Fitness & Nutrition Architect

> **Google Cloud Generative AI Track Project**  
> Hyper-personalized workout routines, precision metabolic nutrition blueprints, and conversational fitness coaching powered by **Google Gemini Models**.

---

## 🌟 Overview & Key Highlights

**FitBuddy** is a full-featured intelligent health assistant that bridges the gap between deterministic metabolic science and generative AI. It solves the common flaw of generic workout generators by grounding generative plans in certified sports science formulas (Mifflin-St Jeor BMR, dynamic TDEE, macronutrient ratios, and BMI risk assessments).

### 🚀 Key Features:
1. **Interactive Assessment & Biometric Science Engine**:
   - Computes **BMI** with visual health risk classifications and ideal weight boundaries.
   - Calculates **BMR** (Basal Metabolic Rate) and **TDEE** (Total Daily Energy Expenditure) based on actual activity multipliers.
   - Computes precise daily caloric deficits or surpluses depending on whether the athlete is cutting, bulking, or recomping.
   - Automatically determines exact macronutrient gram targets (**Protein, Carbohydrates, Fats**) and hydration benchmarks.

2. **AI-Powered Custom Workout Architecture**:
   - Structured day-by-day training splits (Upper/Lower, Push/Pull/Legs, or Full Body) matching available days and equipment.
   - Warm-up routines, exercise tables with target sets/reps/rest/form cues, cool-down mobility, and progressive overload rules.
   - Explicit guardrails for physical injuries and joint limitations (e.g. knee pain, lower back fatigue).

3. **Precision Nutrition & Meal Blueprint**:
   - 4 daily meals/snacks customized to dietary preferences (High Protein, Clean Bulking, Vegetarian, Vegan, Keto, etc.).
   - Exact calorie and macronutrient breakdown per meal.
   - Categorized Smart Weekly Grocery Checklist (Proteins, Complex Carbs, Healthy Fats, Veggies, Pantry).

4. **Interactive FitBuddy AI Coach**:
   - Session-aware chatbot powered by Gemini (`gemini-3.8-flash`).
   - One-click prompt starters for exercise modifications, fast protein snacks, and pre-workout meal timing.

5. **Demo / Offline Mode + Live Gemini AI**:
   - Pre-configured athlete personas (Fat Loss, Hypertrophy, Home Workout, Endurance) with instant demo plan previews.
   - Seamlessly connect your Google AI Studio API key in the sidebar for live model generation.

6. **Consolidated Plan Exporter**:
   - One-click download of the complete training & nutrition dossier as Markdown (`.md`) ready to save or print.

---

## 🛠️ Tech Stack & Architecture

- **Runtimes & Framework:** Python 3.10+, [Streamlit](https://streamlit.io/)
- **Generative AI Model:** Google Gemini Models (`gemini-3.8-flash`) via the modern `google-genai` SDK
- **Styling:** Custom dark glassmorphism design system (`Plus Jakarta Sans` & `Outfit` typography, glowing accent cards, responsive macro bars)
- **Deterministic Math:** Mifflin-St Jeor metabolic equations & WHO BMI reference guidelines

---

## 🚀 Quickstart & How to Run

### 1. Navigate to the project directory:
```bash
cd fitbuddy
```

### 2. Install dependencies:
```bash
pip install -r requirements.txt
```

### 3. (Optional) Set your Gemini API Key in `.env`:
```bash
copy .env.example .env
# Edit .env and paste your GEMINI_API_KEY
```
*Note: You can also enter the API key directly in the sidebar input box inside the web UI!*

### 4. Run the Streamlit application:
```bash
streamlit run app.py
```
Open your browser at `http://localhost:8501`.

---

## 📂 Project Structure

```text
fitbuddy/
├── app.py                 # Streamlit UI & application controller
├── calculator.py          # Deterministic health formulas (BMI, BMR, TDEE, Macros)
├── gemini_client.py       # Google GenAI SDK integration & structured prompt engineering
├── sample_data.py         # Athlete persona presets & rich demonstration data
├── styles.py              # Modern dark luxury glassmorphism CSS theme
├── requirements.txt       # Dependencies
├── .env.example           # Environment template for Gemini API key
└── README.md              # Project documentation & presentation guide
```

---

## 🛡️ Medical & Safety Disclaimer
*FitBuddy is an AI-assisted fitness and nutritional design tool. The generated routines and caloric guidelines are designed for educational and informational purposes. Consult a medical professional or certified physical therapist before beginning any new training program.*
