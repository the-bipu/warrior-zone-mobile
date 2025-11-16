# Warrior Zone Mobile 🎯

A modern React Native mobile application where users can share their experiences, confessions, and stories with the community. Built with React Native and NativeWind (TailwindCSS), Warrior Zone provides a platform for authentic expression and community engagement.

## 📱 About the App

Warrior Zone is a social platform designed for users to:
- Share their personal experiences and confessions
- Explore stories from other community members
- Engage with content through likes and interactions
- Connect with others in a supportive environment

## ✨ Features

- 🏠 **Home Feed** - Browse latest posts and experiences from the community
- 📖 **About** - Learn about the Warrior Zone mission and values
- 💭 **Confession** - View individual confessions and experiences
- 📝 **Confess** - Share your own story anonymously or publicly
- 🔍 **Explore** - Discover trending and popular content
- 📧 **Contact** - Get in touch with the Warrior Zone team
- ❤️ **Like System** - Show support for posts you relate to
- 📱 **Cross-platform** - Works seamlessly on iOS and Android

## 🛠️ Tech Stack

- ⚡ **React Native** - Build native apps using React
- 🎨 **NativeWind** - TailwindCSS for React Native styling
- 📱 **Cross-platform** - iOS and Android support
- 🔧 **TypeScript** - Type safety and better developer experience
- 🎯 **ESLint** - Code quality and consistency
- 📦 **Metro Bundler** - Fast, scalable bundling

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- **Node.js** (v16 or higher)
- **npm** or **yarn** package manager
- **React Native development environment** ([Setup Guide](https://reactnative.dev/docs/environment-setup))
- **For iOS Development:**
  - macOS
  - Xcode (latest version)
  - CocoaPods
- **For Android Development:**
  - Android Studio
  - Android SDK
  - JDK (Java Development Kit)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/the-bipu/warrior-zone-mobile.git
cd warrior-zone-mobile
```

### 2. Install Dependencies

```bash
npm install
# or
yarn install
```

### 3. Install iOS Dependencies (macOS only)

```bash
cd ios && pod install && cd ..
```

### 4. Start Metro Bundler

```bash
npm start
# or
yarn start
```

### 5. Run the Application

**For iOS:**
```bash
npm run ios
# or
yarn ios
```

**For Android:**
```bash
npm run android
# or
yarn android
```

## 📁 Project Structure

```
warrior-zone-mobile/
├── app/                    # Main application screens and navigation
│   ├── home/              # Home feed screen
│   ├── about/             # About page
│   ├── confession/        # Individual confession view
│   ├── confess/           # Create confession screen
│   ├── explore/           # Explore content screen
│   └── contact/           # Contact page
├── assets/                # Images, fonts, and static resources
├── components/            # Reusable UI components
├── constants/             # App constants and configuration
├── hooks/                 # Custom React hooks
├── scripts/               # Build and utility scripts
├── .vscode/               # VSCode settings
├── app.json               # App configuration
├── babel.config.js        # Babel configuration
├── eslint.config.js       # ESLint configuration
├── global.css             # Global styles
├── metro.config.js        # Metro bundler configuration
├── tailwind.config.js     # TailwindCSS configuration
├── tsconfig.json          # TypeScript configuration
└── package.json           # Dependencies and scripts
```

## 🎨 Styling with NativeWind

Warrior Zone uses NativeWind for styling, which brings TailwindCSS utility classes to React Native:

```tsx
import { View, Text } from 'react-native';

export default function PostCard() {
  return (
    <View className="p-4 bg-white rounded-lg shadow-md mb-4">
      <Text className="text-xl font-bold text-gray-800">
        User Experience
      </Text>
      <Text className="text-gray-600 mt-2">
        Share your story here...
      </Text>
    </View>
  );
}
```

### Customizing Styles

Edit `tailwind.config.js` to customize your design system:

```javascript
module.exports = {
  content: [
    './app/**/*.{js,jsx,ts,tsx}',
    './components/**/*.{js,jsx,ts,tsx}'
  ],
  theme: {
    extend: {
      colors: {
        warrior: {
          primary: '#your-color',
          secondary: '#your-color',
        },
      },
    },
  },
  plugins: [],
};
```

## 📱 App Screens

### Home
The main feed where users can see the latest posts and experiences from the community.

### About
Information about Warrior Zone, its mission, and community guidelines.

### Confession
Detailed view of individual confessions with likes and engagement options.

### Confess
Form for users to submit their own experiences and stories.

### Explore
Discover trending content, categories, and popular posts.

### Contact
Get in touch with the Warrior Zone team for support or feedback.

## 🔧 Available Scripts

- `npm start` - Start Metro bundler
- `npm run android` - Run on Android device/emulator
- `npm run ios` - Run on iOS simulator
- `npm run lint` - Run ESLint for code quality checks
- `npm test` - Run tests

## 🔐 Environment Configuration

Create a `.env` file in the root directory (if needed for backend integration):

```env
API_URL=your_api_url_here
API_KEY=your_api_key_here
```

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

Please make sure to update tests as appropriate and follow the existing code style.

## 📝 Code Style

This project uses ESLint for code quality. Run the linter before committing:

```bash
npm run lint
```

## 🐛 Troubleshooting

### Metro Bundler Issues
```bash
npm start -- --reset-cache
```

### iOS Build Issues
```bash
cd ios
pod deintegrate
pod install
cd ..
```

### Android Build Issues
```bash
cd android
./gradlew clean
cd ..
```

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🔗 Resources

- [React Native Documentation](https://reactnative.dev/)
- [NativeWind Documentation](https://www.nativewind.dev/)
- [TailwindCSS Documentation](https://tailwindcss.com/)
- [TypeScript Documentation](https://www.typescriptlang.org/)

## 💬 Support

If you encounter any issues or have questions:
- Open an issue on [GitHub](https://github.com/the-bipu/warrior-zone-mobile/issues)
- Contact the development team through the app's Contact page

## 🙏 Acknowledgments

Thank you to all contributors and the community for making Warrior Zone a supportive platform for sharing experiences.

---

**Built with ❤️ by the Warrior Zone Team**

Happy coding! 🚀
