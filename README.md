# ⚓ Marsa

<p align="center">
  <img src="docs/screenshots/marsa_app_icon.png" width="120" alt="Marsa App Icon">
</p>

<h3 align="center">
  A modern Flutter booking platform for discovering and reserving vacation units.
</h3>

<p align="center">
  Flutter • Dart • Clean Architecture • BLoC/Cubit • REST API
</p>

<p align="center">
  <a href="#-screenshots">📸 View Screenshots</a>
  &nbsp; • &nbsp;
  <a href="#-features">✨ Features</a>
  &nbsp; • &nbsp;
  <a href="#-architecture">🏗 Architecture</a>
</p>

---

## 📱 About

**Marsa** is a Flutter-based mobile booking platform designed to make discovering and reserving vacation units simple and intuitive.

Users can explore different types of units, view detailed information, check availability, complete a multi-step booking process, submit payment receipts, and track their reservations.

The application is built with a focus on **clean architecture, maintainable code, reusable components, reliable API integration, and a polished user experience.**

> 🚧 **Status:** In Development

---

## ✨ Features

### 🔐 Authentication

- User registration
- User login
- Form validation
- Password confirmation validation
- Secure token storage
- Persistent authentication session
- API error handling
- Loading, success, and failure states

---

### 🏠 Home & Discovery

The home screen provides multiple sections to help users discover available units:

- **All Units**
- **Featured Units**
- **Units Under 1000 EGP**
- Quick category filtering
- Search
- Responsive unit cards
- Skeleton loading
- Shimmer loading states

Users can quickly filter units by categories such as:

- Chalet
- Villa
- And other available unit types

---

### 🏡 Unit Details

Each unit has a dedicated details screen containing:

- Unit images
- Unit name
- Location
- Description
- Amenities / features
- Category
- Capacity
- Price per night
- Rating
- Reviews count
- Booking action

The details screen provides users with the information they need before starting a reservation.

---

# 📅 Booking Flow

Marsa provides a **4-step booking experience**.

### 1. Date Selection

Users select:

- Check-in date
- Check-out date

The application handles the selected booking period and availability calendar.

### 2. Booking Summary

Users can review:

- Selected unit
- Check-in date
- Check-out date
- Number of nights
- Price details
- Coupon information
- Final booking price

### 3. Payment

The application supports manual payment through:

- InstaPay
- Wallet transfer

Users can upload their payment transfer receipt as part of the booking process.

### 4. Booking Confirmation

After submitting the booking, users can:

- Review their booking information
- View the submitted payment information
- Track the current booking status

---

## ❤️ Favorites

Users can save units for later through the favorites system.

Features include:

- Add / remove favorites
- Dedicated favorites screen
- Favorite state synchronization
- Empty state handling
- Loading states
- Failure and retry states
- Pull-to-refresh

---

## 📋 My Appointments

Users can manage their reservations from the **My Appointments** section.

Each booking displays:

- Unit information
- Location
- Booking dates
- Booking status
- Final price
- Booking ID
- Booking details

Appointments are organized by booking status to make reservation tracking easier.

---

## 👤 Profile

The profile section allows users to manage their account.

Features include:

- View profile information
- Update profile information
- Theme switching
- Arabic / English localization
- Logout
- Persistent authentication session

---

# 🎨 UI / UX

Marsa focuses on providing a clean, responsive, and consistent mobile experience.

### Implemented UI Features

- Responsive layouts
- Light / Dark theme
- Arabic / English localization
- RTL support
- Reusable widgets
- Custom UI components
- Empty states
- Failure states
- Loading states
- Skeleton loading
- Shimmer effects
- Cached network images
- Smooth animations
- Custom splash screen
- Custom application icon
- Pull-to-refresh interactions

---

# 📸 Screenshots

> Screenshots showcase the main application flows, UI states, booking experience, and user features.

## 🔐 Authentication

| Login | Register |
|:---:|:---:|
| <img src="docs/screenshots/login_light.png" width="250"> | <img src="docs/screenshots/register_light.png" width="250"> |

---

## 🏠 Home & Discovery

| Loading | Home | Units |
|:---:|:---:|:---:|
| <img src="docs/screenshots/home_loading_light.png" width="250"> | <img src="docs/screenshots/home4_light.png" width="250"> | <img src="docs/screenshots/home3_light.png" width="250"> |

### 🔎 Filtering

<p align="center">
  <img src="docs/screenshots/filter1_light.png" width="250">
  <img src="docs/screenshots/filter_dark.png" width="250">
  <img src="docs/screenshots/filter3_light.png" width="250">
</p>

---

## 🏡 Unit Details

<p align="center">
  <img src="docs/screenshots/details1_dark.png" width="250">
  <img src="docs/screenshots/details2_dark.png" width="250">
  <img src="docs/screenshots/details3_light.png" width="250">
</p>

---

## 📅 Booking Flow

| Date Selection | Date Selection | Booking Summary |
|:---:|:---:|:---:|
| <img src="docs/screenshots/date_step_light.png" width="250"> | <img src="docs/screenshots/date_step2_dark.png" width="250"> | <img src="docs/screenshots/summary_step_dark.png" width="250"> |

| Payment | Confirmation | Booking Status |
|:---:|:---:|:---:|
| <img src="docs/screenshots/payment_step2_dark.png" width="250"> | <img src="docs/screenshots/appointment_done_light.png" width="250"> | <img src="docs/screenshots/appointment_done2_dark.png" width="250"> |

---

## 👤 User Features

### ❤️ Favorites

| Empty State | Loading State | Favorites List |
|:---:|:---:|:---:|
| <img src="docs/screenshots/fav_empty.png" width="250"> | <img src="docs/screenshots/fav_loading.png" width="250"> | <img src="docs/screenshots/fav_dark.png" width="250"> |

---

### 📋 My Appointments

| All Appointments | Completed | Cancelled |
|:---:|:---:|:---:|
| <img src="docs/screenshots/all_appointments_dark.png" width="250"> | <img src="docs/screenshots/my_appointments_completed_dark.png" width="250"> | <img src="docs/screenshots/my_appointments_canceld_light.png" width="250"> |

---

### 👤 Profile

| Profile | Edit Profile | Theme |
|:---:|:---:|:---:|
| <img src="docs/screenshots/profile_light.png" width="250"> | <img src="docs/screenshots/edit_profile_light.png" width="250"> | <img src="docs/screenshots/theme_light.png" width="250"> |

---

# 🏗 Architecture

Marsa follows **Clean Architecture** with a feature-based project structure.

The application is organized into three main layers:

```text
┌──────────────────────────────┐
│        Presentation          │
│                              │
│  Screens • Widgets • Cubit   │
│        • UI States           │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│            Domain            │
│                              │
│ Entities • Use Cases         │
│ Repository Contracts         │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│             Data             │
│                              │
│ API • Models • Data Sources  │
│ Repository Implementations   │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│           REST API           │
└──────────────────────────────┘
```

Each feature is organized around its own business responsibility, keeping the codebase modular, maintainable, and easier to scale.

---

## 🛠 Tech Stack

| Category | Technology |
|:---|:---|
| Framework | Flutter |
| Language | Dart |
| Architecture | Clean Architecture |
| State Management | BLoC / Cubit |
| Networking | Dio |
| Dependency Injection | GetIt |
| Local Storage | SharedPreferences |
| Secure Storage | Flutter Secure Storage |
| Serialization | JSON / JsonSerializable |
| Functional Programming | Dartz |
| Localization | Easy Localization |
| Responsive UI | Flutter ScreenUtil |
| UI Loading | Skeletonizer / Shimmer |
| Calendar | Table Calendar |
| Image Handling | Cached Network Image / Image Picker |
| Navigation | Persistent Bottom Navigation Bar |
| Animations | Flutter Animate / Animate Do / Lottie |
| Release Updates | Shorebird |

---

## ⚙️ Engineering Highlights

- Feature-based Clean Architecture
- Cubit-based state management
- Repository pattern with clear domain contracts
- Dependency injection using GetIt
- RESTful API integration using Dio
- Centralized API error handling
- Secure authentication token storage
- Persistent authentication sessions
- JSON serialization and model mapping
- Arabic / English localization
- Light / Dark theme support
- Responsive layouts using ScreenUtil
- Skeleton loading and shimmer effects
- Cached network images
- Reusable custom UI components
- Form validation and user input handling
- Multi-step booking workflow
- Payment receipt image upload
- Booking status tracking
- Pull-to-refresh interactions
- Empty / Loading / Failure / Success states

---

## 🔐 Security & Persistence

Authentication credentials are handled using secure local storage.

Implemented:

- Secure access token storage
- Persistent authentication sessions
- Authentication state restoration
- Secure logout flow
- Local user data persistence

---

## 🌍 Localization & Theming

Marsa supports a localized and customizable user experience.

### Localization

- Arabic 🇪🇬
- English 🇬🇧
- Localized validation messages
- Localized UI text
- RTL support for Arabic

### Theming

- Light Mode
- Dark Mode
- Centralized color system
- Centralized typography
- Reusable theme components

---

## ⚡ Loading & Error Handling

Marsa provides dedicated UI states for different application conditions:

- Skeleton loading
- Shimmer effects
- Empty states
- Failure states
- Retry actions
- Pull-to-refresh
- Loading indicators
- API error feedback
- Form validation feedback

---

## 📂 Project Structure

The project follows a feature-based structure with shared application infrastructure inside `core`.

```text
lib/
├── core/
│   ├── common/
│   ├── constants/
│   ├── cubit/
│   ├── entities/
│   ├── extensions/
│   ├── helpers/
│   ├── routing/
│   ├── services/
│   ├── theme/
│   └── utils/
│
├── features/
│   ├── auth/
│   ├── booking/
│   ├── favorites/
│   ├── profile/
│   ├── units/
│   ├── onboarding/
│   └── splash/
│
└── main.dart
```

Each feature is organized around its own business responsibility and can contain:

```text
feature/
├── data/
├── domain/
└── presentation/
```

This structure keeps business logic separated from UI implementation and external data sources, making the application easier to maintain and extend.

## 🚀 Getting Started

### Prerequisites

- Flutter SDK
- Dart SDK
- Android Studio / VS Code
- Android Emulator or physical device

### Installation

```bash
git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
cd marsa
flutter pub get
flutter run
```

---

## 🐦 Shorebird

Marsa is integrated with **Shorebird** for over-the-air Flutter updates.

This allows eligible Flutter code changes to be delivered through patches without requiring a full application release for every update.


## 🗺 Roadmap

### Completed

- [x] Authentication
- [x] Home & unit discovery
- [x] Unit details
- [x] Favorites
- [x] Multi-step booking flow
- [x] Payment receipt upload
- [x] Booking status tracking
- [x] Profile management
- [x] Arabic / English localization
- [x] Light / Dark theme
- [x] Skeleton & shimmer loading
- [x] Shorebird integration

### Planned

- [ ] Push notifications
- [ ] Additional payment integrations
- [ ] Further performance improvements

## 👨‍💻 Author

**Karim Tamer**

Flutter Developer

- GitHub: [KarimTamer74](https://github.com/KarimTamer74)
- LinkedIn: [LinkedIn](http://www.linkedin.com/in/karim-tamer74)

## 📄 License

This project is currently intended for portfolio and demonstration purposes.