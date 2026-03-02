# PetChain Mobile App

 **Open Source Week - We Need Your Help!**

The PetChain Mobile App is a companion application for pet owners, designed to provide easy access to their pets' medical records, medication schedules, and vet appointments. By scanning a QR code or logging into their account, pet owners can view and manage their pets' health information on the go.

This app integrates seamlessly with the PetChain Web Platform (for vet hospitals) and PetChain Smart Contracts (for secure, decentralized data storage on Stellar blockchain).

---

## Important Note for Contributors

**UI/UX designs are not available yet.** We're focusing exclusively on backend logic, API integration, and infrastructure during this phase. All available issues are in the `backend/ folder.
 Please do not work on UI components or screens at this time.

**IMPORTANT: THIS IS CLIENT-SIDE MOBILE APP CODE, NOT SERVER-SIDE BACKEND CODE.** The "backend" folder name refers to the app's logic layer (services, models, utilities) that runs on the mobile device and communicates with the actual NestJS backend API. All code will be written in **TypeScript** for React Native.

---

##  Current Status: Backend & Logic Phase

**Focus: Building the core logic and backend integration first!** We're intentionally skipping UI work until the foundation is solid.

### What We Need:
- **Backend Integration**: API services, authentication, data sync
- **Core Logic**: Business logic, data models, utilities
- **Infrastructure**: Testing, CI/CD, project setup
- **Documentation**: API docs, architecture guides


## Features (Planned)

- **QR Code Scanning**: Scan your pet's QR code to instantly access their medical records
- **Pet Profile Management**: View and update your pet's information (name, breed, age, medical history)
- **Medication Tracking**: Keep track of medication schedules and receive reminders
- **Appointment Management**: View upcoming vet appointments and schedule new ones
- **Emergency Contacts**: Access emergency vet contacts and nearby clinics
- **Offline Mode**: Access basic pet information even without an internet connection
- **Secure Authentication**: Protect your data with secure login and encryption
- **Scannable Pet Tags**: Each pet gets a unique QR code linked to its medical history
- **Blockchain Integration**: Tamper-proof records stored on Stellar blockchain

## How to Contribute

###  Available Issues

**Check the `backend/` folder for 27 available issues!** Each issue file contains:
- Clear description and requirements
- File path to create
- Acceptance criteria
- Tech stack needed

Pick any issue that interests you and start contributing!

### Priority: Backend & Logic Only 💻

**NO UI WORK - Focus on logic, services, and infrastructure:**

#### High Priority:
1. **Project Setup**
   - Initialize React Native project structure
   - Configure TypeScript, ESLint, Prettier
   - Set up environment variables (.env)

2. **API Integration**
   - Create API service layer (Axios setup)
   - Implement authentication service (JWT)
   - Build API interceptors for token refresh
   - Create error handling middleware
   - Define API endpoints and types

3. **Data Layer**
   - Set up offline storage (AsyncStorage/SQLite)
   - Create data models and TypeScript interfaces
   - Implement data sync logic (online/offline)
   - Build caching strategies

4. **Business Logic**
   - Pet profile management logic
   - Medication tracking algorithms
   - Appointment scheduling logic
   - QR code generation/validation

5. **Testing & CI/CD**
   - Write unit tests for services
   - Integration tests for API calls
   - Set up GitHub Actions
   - Configure code coverage

#### Medium Priority:
- State management setup (Redux/Context)
- Push notification service integration
- Blockchain integration helpers
- Logging and monitoring setup
- Security utilities (encryption, validation)
- API documentation

### Getting Started

**Prerequisites:**
- Node.js (v18 or higher)
- npm or yarn
- Git
- (Optional) Android Studio or Xcode for mobile development

**Setup:**
```bash
# Clone the repository
git clone <repo-url>
cd PetChain-MobileApp

# Install dependencies
npm install
# or
yarn install

# Copy environment variables
cp .env.example .env

# Run tests
npm test
# or
yarn test

# Lint code
npm run lint
# or
yarn lint
```

**Note:** This project is currently in the backend/logic phase. Mobile app compilation (iOS/Android) will be set up after core services are implemented.

## Tech Stack

- **Framework**: React Native
- **Navigation**: React Navigation
- **State Management**: Redux Toolkit or Context API
- **API Integration**: Axios
- **QR Code Scanning**: react-native-camera or expo-camera
- **Authentication**: JWT (integrates with backend)
- **Offline Storage**: AsyncStorage or SQLite
- **Styling**: Styled Components or React Native Paper
- **Blockchain**: Stellar (via backend API)
- **Smart Contracts**: Rust (Stellar)
- **Testing**: Jest and React Native Testing Library

## Project Structure

```
PetChain-MobileApp/
├── src/
│   ├── services/       # API calls, authentication, blockchain
│   ├── models/         # Data models and TypeScript interfaces
│   ├── utils/          # Helper functions, validators, formatters
│   ├── config/         # App configuration, constants
│   ├── types/          # TypeScript type definitions
│   └── hooks/          # Custom React hooks
├── backend/            # Issue files for contributors
│   ├── services/       # Issues for API services
│   ├── models/         # Issues for data models
│   ├── utils/          # Issues for utilities
│   ├── config/         # Issues for configuration
│   ├── types/          # Issues for TypeScript types
│   ├── middleware/     # Issues for middleware
│   └── tests/          # Issues for testing
├── __tests__/          # Unit and integration tests
├── .github/            # GitHub Actions workflows
└── App.tsx             # Main app entry point
```

## Related Repositories

- **Web App**: [PetChain Web Platform](link-to-webapp)
- **Backend**: [PetChain Backend](link-to-backend)
- **Smart Contracts**: [PetChain Contracts](link-to-contracts)

## Contributing Guidelines

1. **Fork** the repository
2. **Create a branch** for your feature (`git checkout -b feature/amazing-feature`)
3. **Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **Push** to your branch (`git push origin feature/amazing-feature`)
5. **Open a Pull Request** with a clear description

### Contribution Ideas (Backend/Logic Only)

- [ ] Initialize React Native project structure
- [ ] Set up TypeScript configuration
- [ ] Create API service layer with Axios
- [ ] Build authentication service (login, logout, token refresh)
- [ ] Implement offline storage with AsyncStorage/SQLite
- [ ] Create data models and interfaces
- [ ] Build data sync logic (online/offline)
- [ ] Add error handling middleware
- [ ] Write unit tests for services
- [ ] Set up CI/CD pipeline with GitHub Actions
- [ ] Implement push notification service
- [ ] Create logging and monitoring utilities
- [ ] Write API integration documentation
- [ ] Build security utilities (encryption, validation)

## Questions?

Open an issue or join our community discussions. We're here to help!

**Note**: This project is part of PetChain, a decentralized platform on Stellar that securely manages pet medical records. Check out the main repository for more context.
