# ⚓ Marsa

<p align="center">
  <img src="assets/images/marsa_app_icon.png" width="120" alt="Marsa App Icon">
</p>

<h3 align="center">
  A modern Flutter booking platform for discovering and reserving vacation units.
</h3>

<p align="center">
  Flutter • Dart • Clean Architecture • BLoC/Cubit • REST API
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

### 🏠 Home

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
- Localization
- Logout
- Persistent authentication session

---

# 🎨 UI / UX

Marsa focuses on providing a clean, responsive, and consistent mobile experience.

### Implemented UI features

- Responsive layouts
- Light / Dark theme
- Arabic / English localization
- Reusable widgets
- Custom UI components
- Empty states
- Failure states
- Loading states
- Skeleton loading
- Shimmer effects
- Smooth animations
- Custom splash screen
- Custom application icon

---

# 📸 Screenshots

> Add your application screenshots inside `docs/screenshots/` and update the filenames below if needed.

## Authentication

| Login | Register |
|:---:|:---:|
| <img src="docs/screenshots/login.png" width="250"> | <img src="docs/screenshots/register.png" width="250"> |

---

## Home & Discovery

| Home | Categories |
|:---:|:---:|
| <img src="docs/screenshots/home.png" width="250"> | <img src="docs/screenshots/categories.png" width="250"> |

| Featured Units | Units Under 1000 |
|:---:|:---:|
| <img src="docs/screenshots/featured.png" width="250"> | <img src="docs/screenshots/priced_units.png" width="250"> |

---

## Unit Details

<p align="center">
  <img src="docs/screenshots/unit_details.png" width="280">
</p>

---

## Booking Flow

| Date Selection | Booking Summary |
|:---:|:---:|
| <img src="docs/screenshots/booking_dates.png" width="250"> | <img src="docs/screenshots/booking_summary.png" width="250"> |

| Payment | Confirmation |
|:---:|:---:|
| <img src="docs/screenshots/payment.png" width="250"> | <img src="docs/screenshots/booking_confirmation.png" width="250"> |

---

## User Features

| Favorites | My Appointments |
|:---:|:---:|
| <img src="docs/screenshots/favorites.png" width="250"> | <img src="docs/screenshots/appointments.png" width="250"> |

| Profile | Dark Mode |
|:---:|:---:|
| <img src="docs/screenshots/profile.png" width="250"> | <img src="docs/screenshots/dark_mode.png" width="250"> |

---

# 🏗 Architecture

Marsa follows **Clean Architecture** with a feature-based project structure.

The application is separated into three main layers:

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
│           Domain             │
│                              │
│ Entities • Use Cases         │
│ Repository Contracts         │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│            Data              │
│                              │
│ API • Models • Data Sources  │
│ Repository Implementations   │
└──────────────┬───────────────┘
               │
               ▼
┌──────────────────────────────┐
│          REST API            │
└──────────────────────────────┘
