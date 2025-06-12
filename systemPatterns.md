# SYSTEM PATTERNS: YourOwn Wallet

## Architectural Patterns

### Core Architecture
- **Pattern**: Clean Architecture with Feature-based Organization
- **State Management**: BLoC (Business Logic Component) Pattern
- **Data Flow**: Unidirectional data flow with Events and States
- **Dependency Management**: Dependency Injection using Provider

### Feature Organization
- **Structure**: lib/features/[feature_name]/
- **Components**: bloc/, components/, widgets/, hooks/
- **Separation**: Each feature is self-contained with clear boundaries
- **Communication**: Features communicate via shared state and events

### Data Patterns
- **Repository Pattern**: Abstract data sources (local/remote)
- **Model-Based**: Shared models in lib/models/shared/
- **GraphQL Integration**: Centralized API layer with code generation
- **Caching Strategy**: Local caching with secure storage

### Security Patterns
- **Secure by Default**: All data encrypted at rest
- **Biometric Gate**: Critical operations require biometric confirmation
- **Token Management**: Secure token storage and refresh
- **Audit Trail**: All financial operations logged

### UI/UX Patterns
- **Design System**: Centralized theme and component library
- **Responsive Design**: Adaptive layouts for different screen sizes
- **Error Handling**: Consistent error states and user feedback
- **Loading States**: Unified loading indicators and shimmer effects

## Established Conventions
- **File Naming**: snake_case for files, PascalCase for classes
- **Feature Structure**: Consistent directory structure across features
- **State Management**: BLoC pattern for all business logic
- **API Integration**: GraphQL with typed code generation
- **Testing Strategy**: Unit tests for business logic, widget tests for UI
