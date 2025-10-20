# React Native + NativeWind Template

A modern React Native template with NativeWind (TailwindCSS) pre-configured and ready to use. This template provides a solid foundation for building cross-platform mobile applications with a utility-first styling approach.

## Features

- ⚡ **React Native** - Build native apps using React
- 🎨 **NativeWind** - TailwindCSS for React Native
- 📱 **Cross-platform** - iOS and Android support
- 🔧 **TypeScript** - Type safety out of the box
- 🎯 **ESLint** - Code linting and formatting
- 📦 **Pre-configured** - Ready to start coding immediately

## Tech Stack

- React Native
- NativeWind v4
- TypeScript
- Metro Bundler
- Babel
- ESLint

## Prerequisites

Before you begin, ensure you have the following installed:

- Node.js (v16 or higher)
- npm or yarn
- React Native development environment ([Setup Guide](https://reactnative.dev/docs/environment-setup))
- For iOS: Xcode and CocoaPods
- For Android: Android Studio and Android SDK

## Using This Template

### Option 1: Use GitHub Template

1. Click the "Use this template" button at the top of the repository
2. Choose "Create a new repository"
3. Name your repository and click "Create repository from template"
4. Clone your new repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   cd YOUR_REPO_NAME
   ```

### Option 2: Clone Directly

```bash
git clone https://github.com/YOUR_USERNAME/react-nativewind-template.git
cd react-nativewind-template
```

## Installation

1. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

2. Install iOS dependencies (macOS only):
   ```bash
   cd ios && pod install && cd ..
   ```

## Running the App

### iOS

```bash
npm run ios
# or
yarn ios
```

### Android

```bash
npm run android
# or
yarn android
```

### Start Metro Bundler

```bash
npm start
# or
yarn start
```

## Project Structure

```
react-nativewind-template/
├── app/                    # Main application code
├── assets/                 # Images, fonts, and other assets
├── components/             # Reusable components
├── constants/              # App constants and configuration
├── hooks/                  # Custom React hooks
├── scripts/                # Build and utility scripts
├── .vscode/               # VSCode settings
├── app.json               # App configuration
├── babel.config.js        # Babel configuration
├── eslint.config.js       # ESLint configuration
├── global.css             # Global styles
├── metro.config.js        # Metro bundler configuration
├── nativewind-env.d.ts    # NativeWind TypeScript definitions
├── tailwind.config.js     # TailwindCSS configuration
├── tsconfig.json          # TypeScript configuration
└── package.json           # Dependencies and scripts
```

## Using NativeWind

NativeWind allows you to use TailwindCSS utility classes in your React Native components:

```tsx
import { View, Text } from 'react-native';

export default function MyComponent() {
  return (
    <View className="flex-1 items-center justify-center bg-blue-500">
      <Text className="text-white text-2xl font-bold">
        Hello, NativeWind!
      </Text>
    </View>
  );
}
```

## Customization

### Tailwind Configuration

Modify `tailwind.config.js` to customize your design system:

```javascript
module.exports = {
  content: ['./app/**/*.{js,jsx,ts,tsx}', './components/**/*.{js,jsx,ts,tsx}'],
  theme: {
    extend: {
      colors: {
        // Add your custom colors
      },
    },
  },
  plugins: [],
};
```

### App Configuration

Edit `app.json` to update your app name, display name, and other settings.

## Scripts

- `npm start` - Start Metro bundler
- `npm run android` - Run on Android
- `npm run ios` - Run on iOS
- `npm run lint` - Run ESLint
- `npm test` - Run tests

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This template is open source and available under the [MIT License](LICENSE).

## Resources

- [React Native Documentation](https://reactnative.dev/)
- [NativeWind Documentation](https://www.nativewind.dev/)
- [TailwindCSS Documentation](https://tailwindcss.com/)
- [TypeScript Documentation](https://www.typescriptlang.org/)

## Support

If you encounter any issues or have questions, please [open an issue](https://github.com/the-bipu/react-nativewind-template/issues) on GitHub.

---

**Happy coding!** 🚀