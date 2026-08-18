<p align="center">
  <img src="docs/screenshots/marsa_app_icon.png" width="120" alt="Marsa App Icon">
</p>

<h1 align="center">
  ⚓ Marsa
</h1>

<h3 align="center">
  Discover, book, and manage your vacation stays — all in one place.
</h3>

<p align="center">
  Flutter • Dart • Clean Architecture • Cubit • REST API • Shorebird
</p>

<p align="center">
  <a href="#-features">✨ FEATURES</a>
  &nbsp; • &nbsp;
  <a href="#-screenshots">📸 SCREENSHOTS</a>
  &nbsp; • &nbsp;
  <a href="#-architecture">🏗 ARCHITECTURE</a>
  &nbsp; • &nbsp;
  <a href="#-tech-stack">🛠 TECH STACK</a>
  &nbsp; • &nbsp;
  <a href="#-author">👨‍💻 CONTACT</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Flutter-3.x-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter">
  <img src="https://img.shields.io/badge/Dart-3.x-0175C2?style=flat-square&logo=dart&logoColor=white" alt="Dart">
  <img src="https://img.shields.io/badge/Clean%20Architecture-1A435E?style=flat-square" alt="Clean Architecture">
  <img src="https://img.shields.io/badge/Cubit%20%2F%20BLoC-6C63FF?style=flat-square" alt="Cubit BLoC">
  <img src="https://img.shields.io/badge/Dio-00A98F?style=flat-square" alt="Dio">
  <img src="https://img.shields.io/badge/Shorebird-OTA%20Updates-1D9E75?style=flat-square" alt="Shorebird">
</p>

<p align="center">
  🏠 Unit Discovery
  &nbsp; • &nbsp;
  📅 Booking
  &nbsp; • &nbsp;
  💳 Payment
  &nbsp; • &nbsp;
  ❤️ Favorites
  &nbsp; • &nbsp;
  👤 Profile
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

<p align="center">

<img src="https://img.shields.io/badge/Flutter-3.x-02569B?style=for-the-badge&logo=flutter&logoColor=white">
<img src="https://img.shields.io/badge/Dart-3.x-0175C2?style=for-the-badge&logo=dart&logoColor=white">
<img src="https://img.shields.io/badge/BLoC%20%2F%20Cubit-6C63FF?style=for-the-badge">
<img src="https://img.shields.io/badge/Dio-00A98F?style=for-the-badge">
<img src="https://img.shields.io/badge/GetIt-Dependency%20Injection-8E44AD?style=for-the-badge">
<img src="https://img.shields.io/badge/Clean%20Architecture-1A435E?style=for-the-badge">

</p>

### 🏗 Architecture & State

<p>
<img src="https://img.shields.io/badge/Clean%20Architecture-1A435E?style=flat-square">
<img src="https://img.shields.io/badge/BLoC%20%2F%20Cubit-6C63FF?style=flat-square">
<img src="https://img.shields.io/badge/GetIt-Dependency%20Injection-8E44AD?style=flat-square">
<img src="https://img.shields.io/badge/Dartz-Functional%20Programming-0D8ABC?style=flat-square">
</p>

### 🌐 Networking & Data

<p>
<img src="https://img.shields.io/badge/Dio-REST%20API-00A98F?style=flat-square">
<img src="https://img.shields.io/badge/JSON-JsonSerializable-F39C12?style=flat-square">
<img src="https://img.shields.io/badge/SharedPreferences-Local%20Storage-795548?style=flat-square">
<img src="https://img.shields.io/badge/Flutter%20Secure%20Storage-Secure%20Storage-607D8B?style=flat-square">
</p>

### 🎨 UI & User Experience

<p>
<img src="https://img.shields.io/badge/ScreenUtil-Responsive%20UI-2196F3?style=flat-square">
<img src="https://img.shields.io/badge/Skeletonizer-Loading-607D8B?style=flat-square">
<img src="https://img.shields.io/badge/Shimmer-Loading-9C27B0?style=flat-square">
<img src="https://img.shields.io/badge/Cached%20Network%20Image-Images-009688?style=flat-square">
<img src="https://img.shields.io/badge/Easy%20Localization-i18n-FF9800?style=flat-square">
</p>

### 🧩 Features & Utilities

<p>
<img src="https://img.shields.io/badge/Table%20Calendar-Calendar-3F51B5?style=flat-square">
<img src="https://img.shields.io/badge/Image%20Picker-Image%20Upload-795548?style=flat-square">
<img src="https://img.shields.io/badge/Persistent%20Bottom%20Nav-Navigation-1A435E?style=flat-square">
<img src="https://img.shields.io/badge/Lottie-Animations-00BFA5?style=flat-square">
<img src="https://img.shields.io/badge/Flutter%20Animate-Animations-E91E63?style=flat-square">
</p>

### 🚀 Release & Updates

<p>
<img src="https://img.shields.io/badge/Shorebird-OTA%20Updates-00A86B?style=for-the-badge">
</p>

---

## ⚙️ Engineering Highlights

### 🏗 Architecture & State Management

- **Clean Architecture** with feature-based modular structure
- **Cubit** for predictable and reactive state management
- **Repository Pattern** with clear domain-level contracts
- **Dependency Injection** using GetIt
- Separation of presentation, domain, and data responsibilities

### 🌐 Networking & Data

- **RESTful API** integration using Dio
- Centralized API error handling
- JSON serialization and model mapping
- Secure authentication token management
- Persistent authentication sessions
- Multipart requests for payment receipt uploads

### 🎨 UI & User Experience

- Responsive layouts using **Flutter ScreenUtil**
- Light / Dark theme support
- Arabic / English localization with RTL support
- Reusable custom UI components
- Cached network images
- Skeleton loading and shimmer effects
- Smooth loading, empty, failure, and success states
- Pull-to-refresh interactions
- Form validation and user input handling

### 📅 Booking & Business Logic

- Multi-step booking workflow
- Date selection and availability handling
- Booking summary and price calculation
- Payment receipt submission
- Booking status tracking
- Favorites management

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


## 🐦 Shorebird

Marsa is integrated with **Shorebird** for over-the-air Flutter updates.

This allows eligible Flutter code changes to be delivered through patches without requiring a full application release for every update.


## 🗺 Roadmap

| Completed | Planned |
|:---|:---|
| ✅ Authentication | 🔜 Push notifications |
| ✅ Home & unit discovery | 🔜 Additional payment integrations |
| ✅ Unit details | 🔜 Further performance improvements |
| ✅ Favorites | 🔜 Google Play release |
| ✅ Multi-step booking flow | 🔜 Apple App Store release |
| ✅ Payment receipt upload | |
| ✅ Booking status tracking | |
| ✅ Profile management | |
| ✅ Arabic / English localization | |
| ✅ Light / Dark theme | |
| ✅ Skeleton & shimmer loading | |
| ✅ Shorebird integration | |

## 👨‍💻 Author

**Karim Tamer**

Flutter Developer

<p align="center">
  <a href="https://github.com/KarimTamer74">
    <img src="https://img.shields.io/badge/GitHub-KarimTamer74-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
  </a>
  <a href="https://www.linkedin.com/in/karim-tamer74">
    <img src="https://img.shields.io/badge/LinkedIn-Karim%20Tamer-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
  </a>
</p>

## 📄 License

This project is currently intended for portfolio and demonstration purposes.