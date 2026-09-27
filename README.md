# KrishiOne (कृषि-वन) 🌾🚜
### Next-Gen Kisan Sarathi & Smart Agriculture Digital Portal

A comprehensive, responsive, multilingual web platform designed to empower farmers across India with AI-powered crop diagnostics, live mandi rates, KVK expert consultations, weather advisories, government schemes, logistics freight estimation, and verified farmer profile authentication.

![License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Firebase](https://img.shields.io/badge/Firebase-Auth%20%26%20Firestore-FFCA28?style=flat&logo=firebase&logoColor=black)

---

## 🌟 Key Features

### 1. 🔐 Farmer Authentication & Profile System (New)
- **Rural/Mobile-First Login (`/login`, `#login`)**:
  - Primary mode: Mobile number with 6-digit OTP verification and resend countdown.
  - Fallback toggle: Mobile number + Password.
  - Instant One-Click Demo Login (`Farmer Ramesh Singh`) for quick evaluation.
  - Language selector synchronized with application locale (English, Hindi, Punjabi, Marathi, Telugu, Tamil, Bengali).
- **New Farmer Registration (`/signup`, `#signup`)**:
  - Captures Full Name, Mobile, Village, District, State, Primary Crop (Wheat, Paddy, Mustard, Cotton, Potato, Tomato), Land Size in Acres, and Preferred Language.
  - Verified OTP step to activate account.
- **My Farm Profile & Account Page (`/profile`, `/account`, `#profile`)**:
  - Accessible via top navbar profile avatar and direct route.
  - Displays registered farmer profile with Aadhaar eKYC verification status.
  - Registered Soil Health Card linked to user's plot (NPK breakdown, pH, organic carbon, and recommended fertilizer dosage).
  - Past Kisan Sarathi consultation tickets history with prescription PDFs.
  - In-place profile editor to update land size, crop, location, and language.
- **Selective Data Protection**:
  - General features (Weather, Live Mandi rates, Sarkari Yojana, Logistics calculator, Disease Scanner) remain open and publicly accessible.
  - Personalized farm metrics (custom Soil Health Card, personal KVK tickets, customized PM-KISAN status) display a rural-friendly login prompt card when logged out.

### 2. 🗣️ Multilingual Kisan Sarathi Voice & Text Assistant
- Native multilingual support for **English**, **Hindi (हिंदी)**, and **Punjabi (ਪੰਜਾਬੀ)**.
- Integrated voice assistant and text-to-speech for agricultural advisory queries and guidance.
- Interactive AI chat widget for instantaneous questions regarding crop health, fertilizers, and subsidies.

### 3. 🔬 KVK AI Crop Disease Scanner & Expert Consultation
- **Automated leaf diagnostics**: Detects common crop ailments such as:
  - Yellow Rust (*Puccinia striiformis*) in Wheat
  - Paddy Blast (*Magnaporthe oryzae*) in Rice
  - Late Blight (*Phytophthora infestans*) in Potato
- **Actionable Remedies**: Instant organic remedies, chemical treatments, and Krishi Vigyan Kendra (KVK) guidance.
- **Direct KVK Scientist Ticket Booking**: Generate consultation tickets and forward reports directly to centers like Ludhiana, Karnal, Varanasi, or Pune.
- **Digital Prescriptions**: View and track scientist prescriptions with dosage and instructions.

### 4. 📈 Live Mandi Bhav (APMC Market Rates)
- Real-time commodity market rate tracker across major APMCs (Azadpur, Khanna, Karnal, etc.).
- Crop-wise filtering (Wheat, Paddy, Mustard, Cotton, Potato).
- Visual trend badges for price surges, high demand, and best market prices.

### 5. 🌤️ Hyperlocal Weather & Farming Advisories
- Real-time weather monitoring with temperature, humidity, rainfall probability, and wind speed.
- Smart advisory cues for critical field operations (e.g. ideal conditions for spraying fertilizers or harvesting).

### 6. 🏛️ Central & State Government Schemes Hub
- Direct access and status tracking for major agricultural schemes:
  - **PM-KISAN Samman Nidhi**: Direct financial benefit tracking.
  - **Pradhan Mantri Fasal Bima Yojana (PMFBY)**: Crop insurance claims and coverage.
  - **Kisan Credit Card (KCC)**: Low-interest institutional credit up to ₹3 Lakhs.
  - **SMAM**: Modern farm machinery and tractor subsidies.

### 7. 🚚 Agri Logistics & Freight Rate Estimator
- Instant logistics calculator based on distance (km), cargo weight (quintals), and vehicle type:
  - Tractor Trolley (Short haul)
  - Small Commercial Truck (Tata Ace)
  - Heavy 16-Ton Truck (Long haul)
- On-demand transport dispatch and verified driver notification alerts.

---

## 🚀 Live Demo & Deployment

- **GitHub Repository**: [https://github.com/abhishekhbtu9154-source/krishi-one](https://github.com/abhishekhbtu9154-source/krishi-one)
- **GitHub Pages Live Deployment**: [https://abhishekhbtu9154-source.github.io/krishi-one/](https://abhishekhbtu9154-source.github.io/krishi-one/)
- **Original Netlify URL**: [https://transcendent-starship-ba1b8f.netlify.app/](https://transcendent-starship-ba1b8f.netlify.app/)

---

## ⚙️ Backend & Authentication Configuration

KrishiOne uses a hybrid authentication architecture:
1. **Zero-Configuration Mode (Default)**: Works immediately out-of-the-box with client-side session persistence in `localStorage`, full mock OTP verification (enter `123456` or the generated code), and local ticket state. No API keys required for development or hackathon demos.
2. **Firebase Auth & Firestore (Production Ready)**: Pre-wired with Firebase SDKs (`firebase-app`, `firebase-auth`, `firebase-firestore`).

### Setting up Firebase in Netlify Environment Settings

To connect your own Firebase project for cloud authentication and Firestore synchronization, set up the following environment variables in your Netlify site dashboard (**Site settings > Environment variables**):

| Variable Name | Description | Example Value |
| :--- | :--- | :--- |
| `FIREBASE_API_KEY` | Firebase Web API Key | `AIzaSyB...` |
| `FIREBASE_AUTH_DOMAIN` | Firebase Auth Domain | `krishione.firebaseapp.com` |
| `FIREBASE_PROJECT_ID` | Google Cloud / Firebase Project ID | `krishione` |
| `FIREBASE_STORAGE_BUCKET` | Firebase Storage Bucket | `krishione.appspot.com` |
| `FIREBASE_MESSAGING_SENDER_ID` | Cloud Messaging Sender ID | `123456789012` |
| `FIREBASE_APP_ID` | Firebase Web App ID | `1:123456:web:...` |

Alternatively, you can configure `window.KRISHI_CONFIG` directly in `index.html`:
```javascript
window.KRISHI_CONFIG = {
    firebase: {
        apiKey: "YOUR_API_KEY",
        authDomain: "YOUR_PROJECT.firebaseapp.com",
        projectId: "YOUR_PROJECT_ID",
        storageBucket: "YOUR_PROJECT.appspot.com",
        messagingSenderId: "YOUR_SENDER_ID",
        appId: "YOUR_APP_ID"
    }
};
```

---

## 📂 Project Structure

```text
krishione/
├── index.html        # Main web application & unified portal
├── favicon.ico       # Application favicon
├── _redirects        # Netlify SPA routing rules (/login, /signup, /profile)
├── README.md         # Comprehensive project documentation
├── LICENSE           # MIT License
└── .gitignore        # Git ignore specifications
```

---

## 💻 Getting Started Locally

```bash
# Clone the repository
git clone https://github.com/abhishekhbtu9154-source/krishi-one.git

# Navigate to project
cd krishi-one

# Open directly in browser
start index.html

# Or serve with Python
python -m http.server 8000
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
