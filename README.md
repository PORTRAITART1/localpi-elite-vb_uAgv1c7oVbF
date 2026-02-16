# LocalPi_Elite
Secure P2P marketplace. Buy and sell locally with KYC-verified Pioneers.
# README - LocalPi Elite

## 📱 Project Overview

**LocalPi Elite** is a mobile marketplace application for second-hand items integrated into the Pi Network ecosystem. It allows Pioneers to buy, sell, and exchange items locally using Pi cryptocurrency as a secure payment method via an escrow system.

---

## ✨ Key Features

### 👤 User Management
- Authentication via Pi Network account
- Customizable profile with editable avatar
- Real statistics for sales/purchases/exchanges
- Precise location (manual or GPS)
- Displayed registration date

### 🏷️ Listings Management
- Create listings with photos (up to 5 images)
- Geolocation on Google Maps
- Instant publication visible to all users
- Proximity filtering

### 💬 Communication
- Integrated buyer-seller messaging
- Item-related conversations
- Real-time notifications

### 💰 Transactions
- Secure payment via Pi
- Integrated escrow system
- Transparent transaction history
- Functional action buttons (Buy, Share, Like)

### 📋 Organization
- Personalized favorites
- Active listings management
- Ongoing transaction tracking

---

## 🛠️ Technical Architecture

### Tech Stack
```
Frontend: React Native / Expo
Backend: Node.js / Express
Database: MongoDB / PostgreSQL
API: RESTful + WebSockets
Payment: Pi Network SDK
Mapping: Google Maps API
```

### Project Structure
```
localpi-elite/
├── src/
│   ├── components/         # Reusable components
│   ├── screens/            # Application screens
│   │   ├── auth/           # Authentication
│   │   ├── home/           # Home and news feed
│   │   ├── profile/        # User profile
│   │   ├── sell/           # Listing creation
│   │   ├── messages/       # Messaging
│   │   └── transactions/   # Escrow and payments
│   ├── services/           # Services (API, Pi SDK)
│   ├── utils/              # Utilities
│   ├── hooks/              # Custom hooks
│   └── constants/          # Configuration
├── assets/                 # Images, icons
├── backend/                 # API server
└── docs/                   # Documentation
```

---

## 🚀 Installation

### Prerequisites
- Node.js v16+
- npm / yarn
- Expo CLI
- Pi Network developer account
- Google Maps API key

### Installation Steps

1. **Clone the repository**
```bash
git clone https://github.com/PORTRAITART1/localpi-elite.git
cd localpi-elite
```

2. **Install dependencies**
```bash
npm install
# or
yarn install
```

3. **Configure environment variables**
```bash
cp .env.example .env
```
Fill in the variables:
- `PI_API_KEY`: Pi Network API key
- `GOOGLE_MAPS_KEY`: Google Maps API key
- `API_URL`: Backend URL
- `DATABASE_URL`: Database connection

4. **Launch the application**
```bash
expo start
# or
npm start
```

---

## 📋 Prioritized Development Plan

### Phase 1: ✅ Core Foundation
- [ ] Pi Network authentication
- [ ] Navigation structure
- [ ] User database
- [ ] Basic profile

### Phase 2: 🔧 Core Features
- [ ] Messaging system
- [ ] Listing creation with photos
- [ ] Avatar upload
- [ ] Geolocation

### Phase 3: 💳 Transactions
- [ ] Pi payment integration
- [ ] Escrow system
- [ ] Real statistics
- [ ] Transaction history

### Phase 4: 🎨 UX/UI
- [ ] Favorites
- [ ] Sharing
- [ ] Notifications
- [ ] Performance optimization

### Phase 5: 🐛 Corrections & Testing
- [ ] Bug fixes from list
- [ ] User testing
- [ ] Cache/image optimization
- [ ] Deployment

---

## 🔗 Pi Network Integration

### SDK Configuration
```javascript
import Pi from 'pi-network-sdk';

Pi.init({
  apiKey: process.env.PI_API_KEY,
  network: 'testnet' // or 'mainnet' in production
});
```

### Pi Payment
```javascript
const payment = await Pi.createPayment({
  amount: 10,
  memo: "Purchase item XYZ",
  metadata: { articleId: "123" }
});
```

---

## 🐛 Priority Corrections (Issues List)

| Problem | Priority | Solution |
|---------|----------|----------|
| Item photos not displaying | 🔴 High | Check CDN/permissions |
| Missing app logo | 🔴 High | Fix asset path |
| Fake statistics | 🟠 Medium | Connect to real API |
| Logout not working | 🟠 Medium | Clear session/token |
| Imprecise location | 🟢 Low | Improve Maps API |
| Messages not readable | 🔴 High | Debug WebSockets |

---

## 📱 Screenshots (coming soon)
- [ ] Home page
- [ ] Listing creation
- [ ] Messaging
- [ ] User profile
- [ ] Pi payment

---

## 🤝 Contribution

1. Fork the project
2. Create a branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Code Standards
- ESLint + Prettier
- Required unit tests
- Component documentation

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📞 Contact

- **Developer:** Abdelouhhab CHARBAK
- **Email:** TOPSNOOP10@GMAIL.COM
- **Pi Network:** @portraitart
- **GitHub:** [https://github.com/portraitart1/localpi-elite](https://github.com/portraitart1/localpi-elite)

---

## 🙏 Acknowledgments
- Pi Network Core Team
- Pioneers Community
- Open source contributors

---

**Project Status:** 🚧 Active development - Alpha Version 0.1.0
