# 💰 uBudget – Smart Budget Tracker App (Prototype)

---

## 📌 Project Overview

**uBudget** is a user-friendly mobile budgeting application designed to help users manage their personal finances efficiently. The app allows users to track expenses, set spending goals, and analyse their financial habits through an intuitive and interactive interface.

This prototype represents the **Build phase** of the development cycle and focuses on implementing all core features, ensuring data persistence, and delivering a stable, functional application.

---

## 👥 Team Members

| Name | Student Number | Role |
|------|----------------|------|
| Mutsawashe Maredza | ST10456212 | Expense Entry & Photo Handling |
| Boluwatife Fayemi | ST10286220 | Dashboard & Reports |
| Washu Mukheli | ST10358940 | User Authentication |
| Raisibe Kwenaitte | ST10248158 | Category & Goal Logic |

---

## 🎯 Purpose of the Application

Managing finances is often stressful and inconsistent. **uBudget** addresses this by:

- ✅ Simplifying expense tracking
- ✅ Providing structured categorisation
- ✅ Encouraging responsible spending through goal setting
- ✅ Offering a clean and intuitive user experience

The app is designed to be **practical**, **engaging**, and **easy to use daily**.

---

## 🛠️ Technologies and Tools Used

| Category | Technologies |
|----------|--------------|
| **Language** | Kotlin |
| **IDE** | Android Studio |
| **Database** | Firebase Realtime Database |
| **Authentication** | Firebase Authentication (Basic Implementation) |
| **UI Design** | XML Layouts |
| **Version Control** | GitHub |
| **CI/CD** | GitHub Actions (Automated build and testing) |

---

## 🧩 Core Features Implemented

### 🔐 1. User Authentication
- Users can securely log in using a username and password
- Firebase Authentication is used to manage user sessions
- Input validation ensures:
  - No empty fields
  - Correct format handling

### 📂 2. Category Management
- Users can create and manage custom expense categories
- Categories are stored in Firebase and linked to the user account
- Examples include:
  - Groceries
  - Transport
  - Entertainment

### 💸 3. Expense Tracking
Users can create detailed expense entries including:
- Amount
- Date
- Start and end time
- Description
- Selected category

All entries are:
- Stored in Firebase
- Linked to the logged-in user
- Retrieved dynamically when needed

### 📸 4. Receipt Image Attachment
- Users can optionally attach a receipt image to an expense
- Images are stored and referenced within Firebase
- Users can view images when browsing expense history

### 🎯 5. Budget Goals
- Users can define:
  - Minimum spending goal
  - Maximum spending limit
- Goals are stored per user and used to guide spending behaviour

### 📊 6. Expense History (Filtered View)
- Users can view all expenses within a selected date range
- Features include:
  - Chronological listing
  - Category display
  - Image preview access

### 📈 7. Category-Based Spending Summary
- Users can view total spending per category
- Data is calculated dynamically from Firebase
- Helps users understand spending patterns

---

## 🔄 Application Workflow

```
User logs into uBudget
    ↓
User creates categories
    ↓
User sets budget goals
    ↓
User adds expense entries
    ↓
Data is stored in Firebase
    ↓
User views:
    • Expense history
    • Category totals
```

---

## 🗄️ Database Structure (Firebase)

The Firebase Realtime Database is structured as follows:

```
users
 └── userId
      ├── categories
      │     └── categoryId
      ├── expenses
      │     └── expenseId
      └── goals
```

### Key Design Considerations:
- Data is **user-specific** for privacy
- Structured for **efficient retrieval**
- Supports **scalability** for future features

---

## 🎨 User Interface Design

The UI was designed with a focus on:
- Simplicity
- Readability
- Ease of navigation

### Key UI Features:
- Clean layouts using XML
- Consistent colour scheme
- Logical screen flow
- Responsive input handling

### Main Screens:
| Screen | Purpose |
|--------|---------|
| Login Screen | User authentication |
| Dashboard | Overview of finances |
| Add Category Screen | Create custom categories |
| Add Expense Screen | Record expenses |
| Expense List Screen | View transaction history |
| Reports Screen | Spending analysis |

---

## ⚠️ Error Handling & Validation

The application includes robust validation mechanisms:

- ✅ Prevents empty or invalid inputs
- ✅ Handles incorrect login attempts
- ✅ Avoids crashes through exception handling
- ✅ Displays user-friendly error messages

---

## 🧪 Testing & Continuous Integration

### ✅ Unit Testing
Core logic tested:
- Data creation
- Data retrieval
- Input validation

### ⚙️ GitHub Actions
Automated workflows configured to:
- Build the app
- Run tests on every push
- Ensure code reliability and consistency

---

## 📹 Demonstration Video

🔗 **YouTube URL:** [https://youtu.be/h9zb5pQJQGU](https://youtu.be/h9zb5pQJQGU)

The video demonstrates:
- Login process
- Category creation
- Expense entry
- Data retrieval from Firebase
- App navigation

---

## 🧾 Project Structure

```
/app
 ├── activities/
 │     ├── LoginActivity.kt
 │     ├── MainActivity.kt
 │     ├── AddExpenseActivity.kt
 │     ├── CategoryActivity.kt
 │     └── ReportsActivity.kt
 │
 ├── firebase/
 │     └── FirebaseHelper.kt
 │
 ├── models/
 │     ├── User.kt
 │     ├── Expense.kt
 │     └── Category.kt
 │
 ├── adapters/
 ├── utils/
 └── MainActivity.kt
```

---

## 🔧 Version Control (GitHub)

- ✅ Repository initialized correctly
- ✅ Regular commits showing progress
- ✅ Meaningful commit messages
- ✅ Integration with GitHub Actions

---

## 🚧 Known Limitations

| Limitation | Description |
|------------|-------------|
| Limited data visualisation | Graphs to be added in final phase |
| Basic authentication | Can be enhanced with security rules |
| UI refinements | Further polish possible |

---

## 🚀 Future Enhancements

- 📊 Advanced analytics and graphs
- 🎮 Gamification (badges, rewards)
- 🔔 Notifications for overspending
- 📡 Offline support with sync
- ✨ Improved UI/UX animations

---

## 📌 Conclusion

The **uBudget prototype** successfully meets all the functional requirements of **Part 2**. The application demonstrates:

- ✅ Strong implementation of Android development principles
- ✅ Effective use of Firebase for real-time data storage
- ✅ A user-friendly and stable interface
- ✅ Clean and maintainable code structure

The app is **fully functional** and provides a solid foundation for further enhancements in the final development phase.

---

## 📚 Reference List

1. The Independent Institute of Education (IIE), 2026. *Programming 3C/Open Source Coding (Introduction) [PROG7313/OPSC6311/OPSC7311 Module Manual]*. The Independent Institute of Education: Unpublished.

2. Android Developers, 2026. *Intents and intent filters.* [online] Available at: https://developer.android.com/guide/components/intents-filters [Accessed 22 April 2026].

3. Android Developers, 2026. *Layouts in views.* [online] Available at: https://developer.android.com/guide/topics/ui/declaring-layout [Accessed 22 April 2026].

4. Android Developers, 2025. *Save simple data with SharedPreferences.* [online] Available at: https://developer.android.com/training/data-storage/shared-preferences [Accessed 22 April 2026].

5. W3Schools, n.d. *W3Schools online web tutorials.* Available at: https://www.w3schools.com [Accessed 20 April 2026].

6. GeeksforGeeks, n.d. *GeeksforGeeks: A computer science portal for geeks.* Available at: https://www.geeksforgeeks.org [Accessed 20 April 2026].

7. Jemerov, D. and Isakova, S., 2017. *Kotlin in action.* Shelter Island, NY: Manning Publications.

8. Android Developers, n.d. *Activity.* [online] Available at: https://developer.android.com/reference/android/app/Activity#startActivityForResult(android.content.Intent,%20int) [Accessed 25 April 2026].

9. Android Developers, n.d. *ArrayAdapter.* [online] Available at: https://developer.android.com/reference/android/widget/ArrayAdapter [Accessed 26 April 2026].

10. Android Developers, n.d. *Drawable resources.* [online] Available at: https://developer.android.com/guide/topics/resources/drawable-resource#Shape [Accessed 25 April 2026].

11. Android Developers, n.d. *Take photos.* [online] Available at: https://developer.android.com/media/camera/camera-deprecated/photobasics [Accessed 26 April 2026].

12. Kotlin, 2025. *Object declarations and expressions.* [online] Available at: https://kotlinlang.org/docs/object-declarations.html [Accessed 25 April 2026].

13. Android Developers, 2024. *Define data using Room entities.* [online] Available at: https://developer.android.com/training/data-storage/room/defining-data [Accessed 28 April 2026].

14. Android Developers, 2024. *Access data using Room DAOs.* [online] Available at: https://developer.android.com/training/data-storage/room/accessing-data [Accessed 28 April 2026].

15. Android Developers, 2024. *ViewModel overview.* [online] Available at: https://developer.android.com/topic/libraries/architecture/viewmodel [Accessed 28 April 2026].

16. Android Developers, 2024. *App architecture guide.* [online] Available at: https://developer.android.com/topic/architecture [Accessed 28 April 2026].

17. Firebase, 2024. *Get started with Cloud Firestore.* [online] Available at: https://firebase.google.com/docs/firestore/quickstart [Accessed 28 April 2026].

18. Firebase, 2024. *Firebase Authentication.* [online] Available at: https://firebase.google.com/docs/auth [Accessed 28 April 2026].

19. GitHub Marketplace, 2025. *Automated Build Android App with GitHub Action.* [online] Available at: https://github.com/marketplace/actions/automated-build-android-app-with-github-action [Accessed 03 November 2025].

---

## 📊 Assignment Status

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/I9fmLyAI)

---

*© 2026 The Independent Institute of Education (Pty) Ltd — PROG7313 Group Assignment*

---

## ✅ README Validation Checklist

| Requirement | Status |
|-------------|--------|
| Project Overview | ✅ |
| Team Members | ✅ |
| Purpose Statement | ✅ |
| Technologies Used | ✅ |
| Core Features (1-7) | ✅ |
| Application Workflow | ✅ |
| Database Structure | ✅ |
| UI Design Description | ✅ |
| Error Handling | ✅ |
| Testing & CI | ✅ |
| Video Demonstration Link | ✅ |
| Project Structure | ✅ |
| Version Control | ✅ |
| Known Limitations | ✅ |
| Future Enhancements | ✅ |
| Conclusion | ✅ |
| Reference List (19 sources) | ✅ |

---

This README is now **complete, professional, and ready for submission**! 🎉# 💰 uBudget – Smart Budget Tracker App (Prototype)

[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)](https://github.com/features/actions)

---

## 📌 Project Overview

**uBudget** is a user-friendly mobile budgeting application designed to help users manage their personal finances efficiently. The app allows users to track expenses, set spending goals, and analyse their financial habits through an intuitive and interactive interface.

This prototype represents the **Build phase** of the development cycle and focuses on implementing all core features, ensuring data persistence, and delivering a stable, functional application.

---

## 👥 Team Members

| Name | Student Number | Role |
|------|----------------|------|
| Mutsawashe Maredza | ST10456212 | Expense Entry & Photo Handling |
| Boluwatife Fayemi | ST10286220 | Dashboard & Reports |
| Washu Mukheli | ST10358940 | User Authentication |
| Raisibe Kwenaitte | ST10248158 | Category & Goal Logic |

---

## 🎯 Purpose of the Application

Managing finances is often stressful and inconsistent. **uBudget** addresses this by:

- ✅ Simplifying expense tracking
- ✅ Providing structured categorisation
- ✅ Encouraging responsible spending through goal setting
- ✅ Offering a clean and intuitive user experience

The app is designed to be **practical**, **engaging**, and **easy to use daily**.

---

## 🛠️ Technologies and Tools Used

| Category | Technologies |
|----------|--------------|
| **Language** | Kotlin |
| **IDE** | Android Studio |
| **Database** | Firebase Realtime Database |
| **Authentication** | Firebase Authentication (Basic Implementation) |
| **UI Design** | XML Layouts |
| **Version Control** | GitHub |
| **CI/CD** | GitHub Actions (Automated build and testing) |

---

## 🧩 Core Features Implemented

### 🔐 1. User Authentication
- Users can securely log in using a username and password
- Firebase Authentication is used to manage user sessions
- Input validation ensures:
  - No empty fields
  - Correct format handling

### 📂 2. Category Management
- Users can create and manage custom expense categories
- Categories are stored in Firebase and linked to the user account
- Examples include:
  - Groceries
  - Transport
  - Entertainment

### 💸 3. Expense Tracking
Users can create detailed expense entries including:
- Amount
- Date
- Start and end time
- Description
- Selected category

All entries are:
- Stored in Firebase
- Linked to the logged-in user
- Retrieved dynamically when needed

### 📸 4. Receipt Image Attachment
- Users can optionally attach a receipt image to an expense
- Images are stored and referenced within Firebase
- Users can view images when browsing expense history

### 🎯 5. Budget Goals
- Users can define:
  - Minimum spending goal
  - Maximum spending limit
- Goals are stored per user and used to guide spending behaviour

### 📊 6. Expense History (Filtered View)
- Users can view all expenses within a selected date range
- Features include:
  - Chronological listing
  - Category display
  - Image preview access

### 📈 7. Category-Based Spending Summary
- Users can view total spending per category
- Data is calculated dynamically from Firebase
- Helps users understand spending patterns

---

## 🔄 Application Workflow

```
User logs into uBudget
    ↓
User creates categories
    ↓
User sets budget goals
    ↓
User adds expense entries
    ↓
Data is stored in Firebase
    ↓
User views:
    • Expense history
    • Category totals
```

---

## 🗄️ Database Structure (Firebase)

The Firebase Realtime Database is structured as follows:

```
users
 └── userId
      ├── categories
      │     └── categoryId
      ├── expenses
      │     └── expenseId
      └── goals
```

### Key Design Considerations:
- Data is **user-specific** for privacy
- Structured for **efficient retrieval**
- Supports **scalability** for future features

---

## 🎨 User Interface Design

The UI was designed with a focus on:
- Simplicity
- Readability
- Ease of navigation

### Key UI Features:
- Clean layouts using XML
- Consistent colour scheme
- Logical screen flow
- Responsive input handling

### Main Screens:
| Screen | Purpose |
|--------|---------|
| Login Screen | User authentication |
| Dashboard | Overview of finances |
| Add Category Screen | Create custom categories |
| Add Expense Screen | Record expenses |
| Expense List Screen | View transaction history |
| Reports Screen | Spending analysis |

---

## ⚠️ Error Handling & Validation

The application includes robust validation mechanisms:

- ✅ Prevents empty or invalid inputs
- ✅ Handles incorrect login attempts
- ✅ Avoids crashes through exception handling
- ✅ Displays user-friendly error messages

---

## 🧪 Testing & Continuous Integration

### ✅ Unit Testing
Core logic tested:
- Data creation
- Data retrieval
- Input validation

### ⚙️ GitHub Actions
Automated workflows configured to:
- Build the app
- Run tests on every push
- Ensure code reliability and consistency

---

## 📹 Demonstration Video

🔗 **YouTube URL:** [https://youtu.be/h9zb5pQJQGU](https://youtu.be/h9zb5pQJQGU)

The video demonstrates:
- Login process
- Category creation
- Expense entry
- Data retrieval from Firebase
- App navigation

---

## 🧾 Project Structure

```
/app
 ├── activities/
 │     ├── LoginActivity.kt
 │     ├── MainActivity.kt
 │     ├── AddExpenseActivity.kt
 │     ├── CategoryActivity.kt
 │     └── ReportsActivity.kt
 │
 ├── firebase/
 │     └── FirebaseHelper.kt
 │
 ├── models/
 │     ├── User.kt
 │     ├── Expense.kt
 │     └── Category.kt
 │
 ├── adapters/
 ├── utils/
 └── MainActivity.kt
```

---

## 🔧 Version Control (GitHub)

- ✅ Repository initialized correctly
- ✅ Regular commits showing progress
- ✅ Meaningful commit messages
- ✅ Integration with GitHub Actions

---

## 🚧 Known Limitations

| Limitation | Description |
|------------|-------------|
| Limited data visualisation | Graphs to be added in final phase |
| Basic authentication | Can be enhanced with security rules |
| UI refinements | Further polish possible |

---

## 🚀 Future Enhancements

- 📊 Advanced analytics and graphs
- 🎮 Gamification (badges, rewards)
- 🔔 Notifications for overspending
- 📡 Offline support with sync
- ✨ Improved UI/UX animations

---

## 📌 Conclusion

The **uBudget prototype** successfully meets all the functional requirements of **Part 2**. The application demonstrates:

- ✅ Strong implementation of Android development principles
- ✅ Effective use of Firebase for real-time data storage
- ✅ A user-friendly and stable interface
- ✅ Clean and maintainable code structure

The app is **fully functional** and provides a solid foundation for further enhancements in the final development phase.

---

## 📚 Reference List

1. The Independent Institute of Education (IIE), 2026. *Programming 3C/Open Source Coding (Introduction) [PROG7313/OPSC6311/OPSC7311 Module Manual]*. The Independent Institute of Education: Unpublished.

2. Android Developers, 2026. *Intents and intent filters.* [online] Available at: https://developer.android.com/guide/components/intents-filters [Accessed 22 April 2026].

3. Android Developers, 2026. *Layouts in views.* [online] Available at: https://developer.android.com/guide/topics/ui/declaring-layout [Accessed 22 April 2026].

4. Android Developers, 2025. *Save simple data with SharedPreferences.* [online] Available at: https://developer.android.com/training/data-storage/shared-preferences [Accessed 22 April 2026].

5. W3Schools, n.d. *W3Schools online web tutorials.* Available at: https://www.w3schools.com [Accessed 20 April 2026].

6. GeeksforGeeks, n.d. *GeeksforGeeks: A computer science portal for geeks.* Available at: https://www.geeksforgeeks.org [Accessed 20 April 2026].

7. Jemerov, D. and Isakova, S., 2017. *Kotlin in action.* Shelter Island, NY: Manning Publications.

8. Android Developers, n.d. *Activity.* [online] Available at: https://developer.android.com/reference/android/app/Activity#startActivityForResult(android.content.Intent,%20int) [Accessed 25 April 2026].

9. Android Developers, n.d. *ArrayAdapter.* [online] Available at: https://developer.android.com/reference/android/widget/ArrayAdapter [Accessed 26 April 2026].

10. Android Developers, n.d. *Drawable resources.* [online] Available at: https://developer.android.com/guide/topics/resources/drawable-resource#Shape [Accessed 25 April 2026].

11. Android Developers, n.d. *Take photos.* [online] Available at: https://developer.android.com/media/camera/camera-deprecated/photobasics [Accessed 26 April 2026].

12. Kotlin, 2025. *Object declarations and expressions.* [online] Available at: https://kotlinlang.org/docs/object-declarations.html [Accessed 25 April 2026].

13. Android Developers, 2024. *Define data using Room entities.* [online] Available at: https://developer.android.com/training/data-storage/room/defining-data [Accessed 28 April 2026].

14. Android Developers, 2024. *Access data using Room DAOs.* [online] Available at: https://developer.android.com/training/data-storage/room/accessing-data [Accessed 28 April 2026].

15. Android Developers, 2024. *ViewModel overview.* [online] Available at: https://developer.android.com/topic/libraries/architecture/viewmodel [Accessed 28 April 2026].

16. Android Developers, 2024. *App architecture guide.* [online] Available at: https://developer.android.com/topic/architecture [Accessed 28 April 2026].

17. Firebase, 2024. *Get started with Cloud Firestore.* [online] Available at: https://firebase.google.com/docs/firestore/quickstart [Accessed 28 April 2026].

18. Firebase, 2024. *Firebase Authentication.* [online] Available at: https://firebase.google.com/docs/auth [Accessed 28 April 2026].

19. GitHub Marketplace, 2025. *Automated Build Android App with GitHub Action.* [online] Available at: https://github.com/marketplace/actions/automated-build-android-app-with-github-action [Accessed 03 November 2025].

[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Kotlin-0095D5?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org)
[![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)](https://firebase.google.com)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)](https://github.com/features/actions)

---

## 📊 Assignment Status

[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/I9fmLyAI)

---

*© 2026 The Independent Institute of Education (Pty) Ltd — PROG7313 Group Assignment*
"# interactive-to-do-list123" 
