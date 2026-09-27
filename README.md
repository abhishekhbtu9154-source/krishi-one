# KrishiOne (कृषि-वन) 🌾🚜
### Next-Gen Kisan Sarathi & Smart Agriculture Digital Portal

A comprehensive, responsive, multilingual web platform designed to empower farmers across India with AI-powered crop diagnostics, live mandi rates, KVK expert consultations, weather advisories, government schemes, and logistics freight estimation.

![License](https://img.shields.io/badge/license-MIT-green)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## 🌟 Key Features

### 1. 🗣️ Multilingual Kisan Sarathi Voice & Text Assistant
- Native multilingual support for **English**, **Hindi (हिंदी)**, and **Punjabi (ਪੰਜਾਬੀ)**.
- Integrated voice assistant and text-to-speech for agricultural advisory queries and guidance.
- Interactive AI chat widget for instantaneous questions regarding crop health, fertilizers, and subsidies.

### 2. 🔬 KVK AI Crop Disease Scanner & Expert Consultation
- **Automated leaf diagnostics**: Detects common crop ailments such as:
  - Yellow Rust (*Puccinia striiformis*) in Wheat
  - Paddy Blast (*Magnaporthe oryzae*) in Rice
  - Late Blight (*Phytophthora infestans*) in Potato
- **Actionable Remedies**: Instant organic remedies, chemical treatments, and Krishi Vigyan Kendra (KVK) guidance.
- **Direct KVK Scientist Ticket Booking**: Generate consultation tickets and forward reports directly to centers like Ludhiana, Karnal, Varanasi, or Pune.
- **Digital Prescriptions**: View and track scientist prescriptions with dosage and instructions.

### 3. 📈 Live Mandi Bhav (APMC Market Rates)
- Real-time commodity market rate tracker across major APMCs (Azadpur, Khanna, Karnal, etc.).
- Crop-wise filtering (Wheat, Paddy, Mustard, Cotton, Potato).
- Visual trend badges for price surges, high demand, and best market prices.

### 4. 🌤️ Hyperlocal Weather & Farming Advisories
- Real-time weather monitoring with temperature, humidity, rainfall probability, and wind speed.
- Smart advisory cues for critical field operations (e.g. ideal conditions for spraying fertilizers or harvesting).

### 5. 🏛️ Central & State Government Schemes Hub
- Direct access and status tracking for major agricultural schemes:
  - **PM-KISAN Samman Nidhi**: Direct financial benefit tracking.
  - **Pradhan Mantri Fasal Bima Yojana (PMFBY)**: Crop insurance claims and coverage.
  - **Kisan Credit Card (KCC)**: Low-interest institutional credit up to ₹3 Lakhs.
  - **SMAM**: Modern farm machinery and tractor subsidies.

### 6. 🚚 Agri Logistics & Freight Rate Estimator
- Instant logistics calculator based on distance (km), cargo weight (quintals), and vehicle type:
  - Tractor Trolley (Short haul)
  - Small Commercial Truck (Tata Ace)
  - Heavy 16-Ton Truck (Long haul)
- On-demand transport dispatch and verified driver notification alerts.

---

## 🚀 Live Demo & Preview

- **Live URL**: [https://transcendent-starship-ba1b8f.netlify.app/](https://transcendent-starship-ba1b8f.netlify.app/)

---

## 🛠️ Technology Stack

- **Markup & Layout**: Clean Semantic HTML5
- **Styling**: [Tailwind CSS CDN](https://tailwindcss.com/) with customized color palettes (`brand`, `sunshine`, `kvk`)
- **Typography**: Google Fonts ([Inter](https://fonts.google.com/specimen/Inter) and [Hind](https://fonts.google.com/specimen/Hind))
- **Iconography**: [Font Awesome 6](https://fontawesome.com/)
- **Interactivity**: Pure Vanilla Modern JavaScript (no bulky build steps required)

---

## 📂 Project Structure

```text
krishione/
├── index.html        # Main web portal application
├── favicon.ico       # Application favicon
├── README.md         # Comprehensive project documentation
└── .gitignore        # Git ignore specifications
```

---

## 💻 Getting Started Locally

Because KrishiOne is a client-side web application, running it locally is straightforward:

### Option 1: Direct File Open
Double click `index.html` or open it with any modern web browser:
```bash
# On Windows
start index.html

# On macOS
open index.html

# On Linux
xdg-open index.html
```

### Option 2: Using a Local HTTP Server

**Using Python:**
```bash
python -m http.server 8000
```
Open [http://localhost:8000](http://localhost:8000) in your browser.

**Using Node.js (`npx serve`):**
```bash
npx serve .
```

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
