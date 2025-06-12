# TECHNOLOGY CONTEXT: YourOwn Wallet

## Technology Stack

### Frontend
- **Framework**: Flutter 3.32.0+
- **Language**: Dart 3.8.0+
- **State Management**: flutter_bloc (BLoC pattern)
- **Navigation**: go_router
- **UI Components**: Material Design + Custom Design System
- **Animations**: flutter_animate, lottie

### Backend & Services
- **Backend-as-a-Service**: AWS Amplify
- **Authentication**: AWS Cognito
- **API**: GraphQL (AWS AppSync)
- **Storage**: AWS S3 (amplify_storage_s3)
- **Database**: DynamoDB (via Amplify)

### Financial Integrations
- **Banking**: Plaid Flutter SDK
- **Cryptocurrency**: Custom crypto APIs
- **Payment Processing**: Various financial institution APIs

### Security & Compliance
- **Biometric Auth**: local_auth
- **Secure Storage**: flutter_secure_storage
- **Encryption**: pointycastle, crypto
- **Key Management**: bip32, bip39 (cryptocurrency)

### Development & DevOps
- **CI/CD**: Bitrise, AWS Amplify
- **Analytics**: Firebase Analytics, Sentry
- **Monitoring**: Sentry error tracking
- **Testing**: flutter_test, bloc_test, mocktail

### Platform Support
- **iOS**: Native iOS deployment
- **Android**: Native Android deployment  
- **Web**: Flutter Web support

## Architecture Patterns
- **Clean Architecture**: Feature-based modular structure
- **BLoC Pattern**: State management across the app
- **Repository Pattern**: Data access abstraction
- **Dependency Injection**: Provider pattern
- **Event-Driven**: GraphQL subscriptions for real-time updates
