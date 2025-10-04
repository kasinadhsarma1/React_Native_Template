# React Native Template

A modern React Native template built with Expo, Clerk authentication, and React Native Reusables components. Features comprehensive UI components, type safety with TypeScript, and cross-platform compatibility (iOS, Android, Web).

## 📋 Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Running the Application](#running-the-application)
- [Technology Stack](#technology-stack)
- [Features](#features)
- [Development](#development)
- [Components](#components)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This is a production-ready React Native template that includes:
- **React Native with Expo**: Cross-platform mobile development
- **Clerk Authentication**: Complete auth solution with OAuth providers
- **React Native Reusables**: shadcn/ui-style components for React Native
- **TypeScript**: Full type safety across the application
- **NativeWind**: Tailwind CSS for React Native styling
- **Expo Router**: File-based routing for React Native

This template is designed to help you quickly bootstrap production-ready mobile applications with modern tools and best practices.

## 📁 Project Structure

```
React_Native_Template/
├── frontend/               # React Native Expo application
│   ├── app/               # Expo Router directory
│   │   ├── _layout.tsx    # Root layout component
│   │   ├── index.tsx      # Home page component
│   │   ├── +html.tsx      # Web HTML template
│   │   ├── +not-found.tsx # 404 page
│   │   └── (auth)/        # Authentication routes
│   │       ├── sign-in.tsx
│   │       ├── forgot-password.tsx
│   │       ├── reset-password.tsx
│   │       └── sign-up/
│   │           ├── _layout.tsx
│   │           ├── index.tsx
│   │           └── verify-email.tsx
│   ├── components/        # React components
│   │   ├── ui/           # React Native Reusables component library
│   │   │   ├── button.tsx
│   │   │   ├── card.tsx
│   │   │   ├── input.tsx
│   │   │   ├── avatar.tsx
│   │   │   ├── dialog.tsx
│   │   │   └── ... (30+ more components)
│   │   ├── sign-in-form.tsx
│   │   ├── sign-up-form.tsx
│   │   ├── user-menu.tsx
│   │   └── social-connections.tsx
│   ├── lib/              # Utility functions
│   │   ├── utils.ts      # Tailwind utilities and helpers
│   │   └── theme.ts      # Theme configuration
│   ├── assets/           # Static assets
│   │   └── images/       # App icons and images
│   ├── .env              # Environment variables
│   ├── app.json          # Expo configuration
│   ├── babel.config.js   # Babel configuration
│   ├── components.json   # React Native Reusables configuration
│   ├── metro.config.js   # Metro bundler configuration
│   ├── package.json      # Node.js dependencies
│   ├── tailwind.config.js # Tailwind CSS configuration
│   └── tsconfig.json     # TypeScript configuration
├── LICENSE               # MIT License
└── README.md             # Project documentation
```

## 🔧 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v18 or higher) - Required for React Native development
- **npm** (v9 or higher) or **yarn** (v1.22 or higher) or **pnpm** (v8 or higher)
- **Expo CLI** - Install with `npm install -g @expo/cli`
- **React Native development environment**:
  - For iOS: Xcode (Mac only) or use Expo Go app
  - For Android: Android Studio or use Expo Go app
  - For Web: Modern web browser

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/kasinadhsarma1/React_Native_Template.git
cd React_Native_Template
```

### 2. Frontend Setup

```bash
cd frontend

# Install dependencies (choose one)
npm install
# or
yarn install
# or (recommended for speed)
pnpm install
```

### 3. Environment Configuration

Create a `.env` file in the frontend directory:

```env
# Clerk Authentication
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=pk_test_your_publishable_key_here

# App Configuration
EXPO_PUBLIC_APP_NAME=React Native Template
```

⚠️ **Important**: Get your Clerk publishable key from [Clerk Dashboard](https://dashboard.clerk.com/last-active?path=api-keys)

### 4. Clerk Setup

1. [Create a Clerk account](https://go.clerk.com/blVsQlm)
2. In the instance setup, leave the default option selected: **Email, phone, username**
3. Enable OAuth providers (Apple, GitHub, Google) under SSO Connections
4. Copy your `EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY` from [your API keys](https://go.clerk.com/u8KAui7)

## 🚀 Running the Application

### Start the Development Server

```bash
cd frontend

# Start Expo development server
npx expo start

# Or with specific platforms
npx expo start --ios      # iOS simulator
npx expo start --android  # Android emulator  
npx expo start --web      # Web browser
```

The Expo development server will start and show you a QR code. You can:

- **iOS**: Press `i` to open iOS simulator (Mac only) or scan QR with Camera app
- **Android**: Press `a` to open Android emulator or scan QR with Expo Go app
- **Web**: Press `w` to open in web browser
- **Physical Device**: Install [Expo Go](https://expo.dev/go) app and scan the QR code

The application will be available at:
- **iOS/Android**: Expo Go app or simulators
- **Web**: `http://localhost:8081`

## 🛠️ Technology Stack

### Frontend (React Native)
- **React Native** - Cross-platform mobile development framework
- **Expo** - Development platform and tools for React Native
- **Expo Router** - File-based routing for React Native apps
- **TypeScript** - Type-safe JavaScript for better development experience
- **React Native Reusables** - shadcn/ui-style components for React Native
- **NativeWind** - Tailwind CSS for React Native styling
- **RN Primitives** - Universal Radix UI primitives for React Native
- **React Native Reanimated** - Smooth, native performance animations
- **Lucide React Native** - Beautiful icon library

### Authentication & Backend Services
- **Clerk** - Complete authentication solution
- **OAuth Providers** - Apple, GitHub, Google sign-in
- **Expo Secure Store** - Secure token storage
- **Expo Auth Session** - OAuth flow handling

### Development Tools
- **TypeScript** - Static type checking
- **ESLint** - Code linting and formatting
- **Prettier** - Code formatting
- **Metro** - React Native bundler

## ✨ Features

- ✅ **React Native with Expo** - Cross-platform mobile development
- ✅ **TypeScript** for type-safe development
- ✅ **Expo Router** - File-based routing for React Native
- ✅ **Clerk Authentication** - Complete auth solution with OAuth
- ✅ **React Native Reusables** - 30+ production-ready UI components
- ✅ **NativeWind** - Tailwind CSS for React Native
- ✅ **Cross-platform** - iOS, Android, and Web support
- ✅ **Hot Reload** for instant development feedback
- ✅ **Type-safe** components and utilities
- ✅ **Responsive design** that works on all screen sizes
- ✅ **OAuth Integration** - Apple, GitHub, Google sign-in
- ✅ **Protected routes** using Clerk authentication
- ✅ **Beautiful UI** with consistent design system
- ✅ **Expo Go** compatible for easy testing
- ✅ **Production-ready** project structure

### Authentication Features
- **Sign In/Sign Up** - Email, phone, username options
- **OAuth Providers** - Apple, GitHub, Google
- **Forgot Password** - Password reset flow
- **Email Verification** - Secure email verification
- **Protected Routes** - Authenticated route protection
- **User Profile** - User menu and profile management
- **Secure Storage** - Token storage with Expo Secure Store

## 💻 Development

### Adding New Components

```bash
cd frontend

# Add specific React Native Reusables component
npx @react-native-reusables/cli@latest add button

# Add multiple components
npx @react-native-reusables/cli@latest add card dialog input

# List all available components
npx @react-native-reusables/cli@latest add --help
```

### Development Commands

```bash
cd frontend

# Start development server
npm run dev

# Start for specific platforms
npm run ios       # iOS development
npm run android   # Android development  
npm run web       # Web development

# Clean project
npm run clean     # Remove .expo and node_modules
```

### Code Quality

```bash
cd frontend

# Format code with Prettier
npx prettier --write .

# Check TypeScript
npx tsc --noEmit

# Lint code
npx eslint .
```

## � Components

The template includes 30+ React Native Reusables components:

### Layout & Navigation
- **Accordion** - Collapsible content sections
- **Card** - Flexible content container
- **Tabs** - Tabbed navigation interface
- **Separator** - Visual content dividers

### Forms & Input
- **Button** - Interactive button component
- **Input** - Text input with validation
- **Checkbox** - Boolean selection input
- **Radio Group** - Single selection from options
- **Select** - Dropdown selection component
- **Switch** - Toggle switch component
- **Label** - Form field labels

### Feedback & Overlays
- **Alert** - Important message display
- **Alert Dialog** - Confirmation dialogs
- **Dialog** - Modal dialog component
- **Tooltip** - Contextual information overlay
- **Progress** - Progress indication
- **Avatar** - User profile images

### Navigation & Menus
- **Context Menu** - Right-click context menus
- **Dropdown Menu** - Dropdown navigation
- **Hover Card** - Hover-triggered content
- **Menubar** - Horizontal menu bar
- **Popover** - Floating content panels

### Advanced Components
- **Collapsible** - Expandable content sections
- **Toggle** - Binary state toggle
- **Toggle Group** - Multiple toggle options
- **Badge** - Status and category indicators

### Key Differences from Web shadcn/ui

- **NativeWind Integration** - Tailwind-like styling for React Native
- **RN Primitives** - Radix UI primitives ported for React Native
- **Portal Support** - Proper modal/overlay handling on mobile
- **No Cascading Styles** - Direct element styling approach
- **Reanimated Integration** - Smooth native animations
- **Platform-specific Adaptations** - iOS and Android optimizations

## 🤝 Contributing

Contributions are welcome! Please read our [Contributing Guidelines](CONTRIBUTING.md) for details on how to submit pull requests, report issues, and contribute to the project.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

## 👥 Author

**kasinadhsarma1**
- GitHub: [@kasinadhsarma1](https://github.com/kasinadhsarma1)

## 🙏 Acknowledgments

- [React Native](https://reactnative.dev/) - Cross-platform mobile development framework
- [Expo](https://expo.dev/) - Platform for universal React applications
- [React Native Reusables](https://reactnativereusables.com/) - shadcn/ui for React Native
- [Clerk](https://clerk.com/) - Complete authentication solution
- [NativeWind](https://www.nativewind.dev/) - Tailwind CSS for React Native
- [RN Primitives](https://rnprimitives.com/) - Radix UI primitives for React Native
- [TypeScript](https://www.typescriptlang.org/) - Typed superset of JavaScript
- [React Native Reanimated](https://docs.swmansion.com/react-native-reanimated/) - Native animations
- [Lucide React Native](https://lucide.dev/) - Beautiful icon library

## 📞 Support

If you have any questions or issues, please:
- Open an issue on GitHub
- Check existing issues and discussions