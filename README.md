# SmartBank Mobile App

A modern mobile banking application built with React Native and Expo, featuring a beautiful UI and seamless user experience.

## Features

- User authentication (login, signup, email confirmation)
- Account type selection
- Phone number verification with OTP
- Passcode creation and confirmation
- Responsive and modern UI with a clean design
- Cross-platform (iOS and Android) compatibility

## Tech Stack

- **React Native**: Core framework for building the mobile application
- **Expo**: Development platform for React Native
- **Expo Router**: File-based routing system
- **React Hook Form**: Form validation and handling
- **Zod**: Schema validation
- **Supabase**: Backend authentication and database
- **Tailwind CSS (NativeWind)**: Styling

## Getting Started

### Prerequisites

- Node.js (v14 or newer)
- Bun or npm
- Expo CLI
- Android Studio (for Android development) or Xcode (for iOS development)
- Physical device or emulator

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```

2. Install dependencies:
   ```bash
   bun install
   # or
   npm install
   ```

3. Start the development server:
   ```bash
   bun start
   # or
   npm start
   ```

4. Follow the instructions in the terminal to open the app on your device or emulator:
   - Press `a` to open on Android
   - Press `i` to open on iOS
   - Scan the QR code with the Expo Go app on your physical device

### Development Build

To create a development build:

1. Install EAS CLI:
   ```bash
   npx expo install eas-cli
   ```

2. Log in to your Expo account:
   ```bash
   npx eas login
   ```

3. Build for Android:
   ```bash
   npx eas build --platform android --profile development
   ```

4. Build for iOS:
   ```bash
   npx eas build --platform ios --profile development
   ```

## Project Structure

```
smartbank/
├── src/
│   ├── app/                  # Main application code
│   │   ├── (onboarding)/     # Onboarding screens
│   │   ├── (unauthenticated)/# Authentication screens
│   │   └── _layout.tsx       # Root layout
│   ├── components/           # Reusable components
│   ├── supabase/             # Supabase client configuration
│   └── utils/                # Utility functions
├── app.json                  # Expo configuration
├── eas.json                  # EAS Build configuration
└── package.json              # Dependencies
```

## Navigation Flow

The app follows a structured navigation flow:

1. **Welcome Screen** → User chooses to login or sign up
2. **Login/Sign Up** → User enters credentials
3. **Choose Account Type** → User selects account type
4. **Phone Verification** → User verifies phone number with OTP
5. **Create Passcode** → User creates a secure passcode
6. **Confirm Passcode** → User confirms the passcode
7. **Setup Complete** → User enters the main app

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Acknowledgments

- Design inspiration from modern banking applications
- Expo team for the excellent development tools
- React Native community for the comprehensive ecosystem
