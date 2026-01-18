# AuditX - Financial Security & Inclusion App

AuditX is a revolutionary mobile application designed to transform the way Indians interact with financial services. Built with cutting-edge AI technology, AuditX combines intelligent fraud detection, instant loan processing, and comprehensive financial tools to create a safer, more accessible banking experience for everyone.

The app addresses critical challenges in India's financial ecosystem - from protecting users against increasing digital fraud to providing instant access to credit for underserved populations. With support for multiple Indian languages and advanced SMS-based transaction monitoring, AuditX makes sophisticated financial security accessible to users across all demographics and technical backgrounds.

Whether you're a first-time borrower looking for quick loans, a security-conscious user wanting fraud protection, or someone seeking to improve their financial health, AuditX provides the tools and insights you need in one comprehensive, user-friendly platform.

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Dakshmulundkar/Auditx.git
cd Auditx
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
```bash
cp .env.example .env
# Configure your environment variables in the .env file
```

## Run Commands

```bash
# Start the development server
npm start

# Run on Android device/emulator
npm run android

# Run on iOS device/simulator
npm run ios

# Run in web browser
npm run web

# Build for production
npm run build
```

## Features

### 🛡️ Smart Security & Fraud Protection
- **Automatic fraud detection** - The app watches your transactions 24/7 and alerts you instantly if something looks suspicious
- **SMS message analysis** - Automatically reads your bank SMS messages to track spending and catch unusual activity
- **Instant WhatsApp alerts** - Get immediate notifications on WhatsApp when fraud is detected, even when the app is closed
- **Scam call protection** - Check if a phone number is safe before answering unknown calls
- **Message safety scanner** - Paste any suspicious text message to check if it's a scam before clicking links

### 💰 Quick & Easy Loans
- **Instant loan approval** - Get approved for loans up to ₹3,00,000 in minutes, not days
- **Simple application** - Fill out forms on your phone and upload documents with your camera
- **Smart credit scoring** - Get loans even with limited credit history using your transaction patterns
- **Multiple loan options** - Choose from personal loans, business loans, and emergency funds
- **Transparent rates** - See exact interest rates and EMI amounts before applying

### 📊 Smart Financial Tools
- **Credit score improvement** - Get personalized tips to boost your credit score from 750 to 800+
- **Investment suggestions** - Receive recommendations on where to invest your savings for better returns
- **Easy regulation guide** - Understand complex banking rules, tax benefits, and government schemes in simple language
- **Multi-language support** - Use the app in English, Hindi, Telugu, Marathi, or Bengali
- **Spending insights** - See where your money goes with automatic expense categorization

### 👤 User-Friendly Experience
- **Personal dashboard** - View all your financial information in one place with easy-to-understand charts
- **Fingerprint login** - Secure access using your fingerprint or face recognition
- **Real-time monitoring** - Watch your transactions happen live with instant notifications
- **Privacy controls** - Decide exactly what information you want to share and with whom
- **24/7 support** - Get help anytime through in-app chat and WhatsApp support

## System Architecture

The app is built with a modern, scalable architecture that ensures fast performance and reliable security:

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Mobile App    │    │   Backend API   │    │   AI Services   │
│  (React Native) │◄──►│   (Node.js)     │◄──►│   (Gemini AI)   │
└─────────────────┘    └─────────────────┘    └─────────────────┘
         │                       │                       │
         ▼                       ▼                       ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   SMS Parser    │    │    Database     │    │ Notification    │
│   (Local AI)    │    │   (Firebase)    │    │ Service (Twilio)│
└─────────────────┘    └─────────────────┘    └─────────────────┘
```

### Key Components:
- **Mobile App**: Cross-platform React Native application for iOS and Android
- **Backend API**: Secure Node.js server handling all business logic and data processing
- **AI Services**: Gemini AI for fraud detection, risk assessment, and personalized recommendations
- **SMS Parser**: Local AI that analyzes bank messages to extract transaction information
- **Database**: Firebase for secure user data storage and real-time synchronization
- **Notification Service**: Twilio integration for WhatsApp alerts and SMS communications

## Configuration

### Environment Variables
Create a `.env` file in the root directory with the following variables:

```env
# Firebase Configuration (for user authentication and data storage)
FIREBASE_API_KEY=your_firebase_api_key
FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
FIREBASE_PROJECT_ID=your_firebase_project_id
FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
FIREBASE_APP_ID=your_firebase_app_id

# Gemini AI (for fraud detection and financial insights)
GEMINI_API_KEY=your_gemini_api_key

# Twilio Configuration (for WhatsApp notifications)
TWILIO_ACCOUNT_SID=your_twilio_account_sid
TWILIO_AUTH_TOKEN=your_twilio_auth_token
TWILIO_WHATSAPP_NUMBER=your_twilio_whatsapp_number

# App Configuration
APP_ENV=development
API_BASE_URL=your_api_base_url
```

### Required Permissions
The app requires the following permissions to function properly:
- **SMS Read Permission**: To analyze bank transaction messages
- **Camera Permission**: For document scanning during loan applications
- **Notification Permission**: For fraud alerts and transaction notifications
- **Biometric Permission**: For secure fingerprint/face login

### Setup Instructions
1. Create accounts on Firebase, Google AI Studio (for Gemini), and Twilio
2. Configure your Firebase project with authentication and Firestore database
3. Enable SMS and WhatsApp services in your Twilio account
4. Add your API keys to the `.env` file
5. Test the configuration by running the app in development mode

## Tech Stack

### Frontend Development
- **React Native** - Cross-platform mobile app framework for iOS and Android
- **Expo** - Development platform with built-in tools and services
- **TypeScript** - Adds type safety to JavaScript for better code quality
- **React Navigation** - Handles screen navigation and tab management
- **React Native Paper** - Material Design components for consistent UI

### Backend & Cloud Services
- **Node.js** - JavaScript runtime for server-side development
- **Express.js** - Web framework for building REST APIs
- **Firebase Authentication** - Secure user login and registration
- **Firestore Database** - Real-time NoSQL database for user data
- **Firebase Storage** - Cloud storage for documents and images

### AI & Machine Learning
- **Gemini AI** - Google's AI for fraud detection and financial insights
- **Natural Language Processing** - For analyzing SMS messages and user queries
- **Machine Learning Models** - Custom models for risk assessment and credit scoring

### Communication & Notifications
- **Twilio** - SMS and WhatsApp messaging platform
- **Push Notifications** - Real-time alerts for security and transactions
- **Email Services** - For account verification and important updates

### Development & Testing Tools
- **ESLint** - Code quality and style checking
- **Prettier** - Automatic code formatting
- **Jest** - Unit testing framework
- **Detox** - End-to-end testing for mobile apps
- **Metro** - JavaScript bundler for React Native

## Contributing

We welcome contributions from the community! Please read our contributing guidelines and submit pull requests for any improvements.

## Support

For technical support or questions, please:
- Open an issue on GitHub
- Contact us through the in-app support chat
- Email us at support@auditx.com

## License

Copyright © 2024 Daksh Mulundkar. All rights reserved.