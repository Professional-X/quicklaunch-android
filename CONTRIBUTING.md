# Contributing to QuickLaunch

Thank you for your interest in contributing to QuickLaunch! This document provides guidelines and instructions for contributing to this project.

## 📋 Code of Conduct

By participating in this project, you agree to maintain a respectful and inclusive environment for everyone.

## 🚀 How to Contribute

### Reporting Bugs

1. **Search first** - Check if the bug has already been reported
2. **Use issue templates** - Fill out the bug report template
3. **Include details**:
   - Device model and manufacturer
   - Android version
   - Steps to reproduce
   - Expected vs actual behavior
   - Screenshots or screen recordings

### Suggesting Features

1. **Search existing issues** - Check if the feature has been requested
2. **Describe the use case** - Explain why this feature would be useful
3. **Provide examples** - Show how it would work in practice

### Pull Requests

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Make your changes** following the coding standards
4. **Write tests** for new functionality
5. **Commit with clear messages**: `git commit -m 'Add amazing feature'`
6. **Push to your branch**: `git push origin feature/amazing-feature`
7. **Open a Pull Request**

## 💻 Development Setup

### Prerequisites

- Android Studio Hedgehog (2023.1.1) or later
- JDK 17 or later
- Android SDK 34
- Git

### Setup Instructions

```bash
# Clone the repository
git clone https://github.com/quicklaunch/quicklaunch-android.git

# Navigate to project directory
cd quicklaunch-android

# Open in Android Studio
# File -> Open -> Select the project folder

# Build and run on emulator or device
```

### Building

```bash
# Using Gradle
./gradlew assembleDebug

# Using Android Studio
# Build -> Build APK
```

### Testing

```bash
# Run unit tests
./gradlew test

# Run instrumented tests (on device/emulator)
./gradlew connectedAndroidTest
```

## 📐 Coding Standards

### Kotlin Style Guide

- Follow [Kotlin Coding Conventions](https://kotlinlang.org/docs/coding-conventions.html)
- Use meaningful variable and function names
- Add documentation comments for public APIs
- Keep functions small and focused

### Architecture

- Follow Clean Architecture principles
- Use MVVM pattern for presentation layer
- Implement repository pattern for data layer
- Use dependency injection with Hilt

### Code Organization

```
com.quicklaunch/
├── data/           # Data layer
│   ├── local/      # Local data sources
│   ├── repository/ # Repository implementations
│   └── source/     # Data providers
├── di/             # Dependency injection
├── domain/         # Business logic
│   ├── model/      # Domain models
│   └── repository/ # Repository interfaces
└── presentation/   # UI layer
    └── ui/         # Activities, ViewModels, Composables
```

## 🧪 Testing Guidelines

- Write unit tests for business logic
- Write UI tests for critical user flows
- Test edge cases and error scenarios
- Maintain test coverage for new features

## 📝 Documentation

- Update README.md for new features
- Add inline documentation for complex code
- Create guide documentation for user-facing features
- Update API documentation when needed

## 🔍 Code Review Process

1. All submissions require review from maintainers
2. Reviewers may request changes
3. Address feedback and push updates
4. Once approved, maintainers will merge

## 📜 License

By contributing, you agree that your contributions will be licensed under the MIT License.

## 📞 Getting Help

- **GitHub Issues**: [Open an issue](https://github.com/quicklaunch/quicklaunch-android/issues)
- **Discussions**: [GitHub Discussions](https://github.com/quicklaunch/quicklaunch-android/discussions)
- **Email**: support@quicklaunch.app

---

Thank you for making QuickLaunch better! 🎉
