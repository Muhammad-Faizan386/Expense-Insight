# 💰 Expense Insight

**Expense Insight** is a cross-platform personal finance management application built with **Flutter and Dart**. It allows users to record and manage expenses, review recent transactions, and visualize their weekly spending through an interactive chart.

The project was developed to strengthen practical software engineering skills in **Flutter application development, state management, data processing, form validation, responsive UI design, and reusable widget architecture**.

---

## 📱 Project Overview

Managing daily expenses can become difficult when spending information is scattered across different places.

Expense Insight provides a simple interface for recording expenses and understanding recent spending patterns through a **7-day expense visualization**.

The application supports:

* Adding new expenses
* Viewing recorded transactions
* Removing transactions
* Selecting transaction dates
* Calculating total spending
* Filtering recent transactions
* Visualizing weekly spending
* Responsive layouts across supported platforms

---

## ✨ Features

### 💳 Transaction Management

* Add new expenses with title, amount, and date
* View transactions in a scrollable list
* Delete existing transactions
* Automatically generate unique transaction IDs
* Validate user input before adding transactions

### 📊 Expense Visualization

* 7-day spending analysis
* Dynamic chart bars
* Percentage-based spending visualization
* Automatic chart updates when transactions change
* Calculation of total spending for recent transactions

### 📱 Responsive UI

* Adaptive layouts
* Responsive chart sizing
* Material Design 3 interface
* Custom typography
* Empty-state handling
* Bottom-sheet transaction form
* Mobile and desktop-friendly layouts

### 🧩 Reusable Components

The application is divided into reusable widgets such as:

* Transaction list
* Transaction form
* Chart
* Chart bar
* Transaction model

This makes the application easier to maintain and extend.

---

## 🛠️ Tech Stack

| Technology     | Purpose                              |
| -------------- | ------------------------------------ |
| **Flutter**    | Cross-platform application framework |
| **Dart**       | Programming language                 |
| **Material 3** | UI design system                     |
| **intl**       | Date formatting and localization     |
| **DateTime**   | Date and transaction processing      |
| **Git**        | Version control                      |

The application is designed to compile for **Android, iOS, Web, and Windows**.

---

## 🏗️ Architecture & Code Organization

Expense Insight follows a **component-based Flutter architecture** with separation between data models, reusable UI components, and application logic.

```text
User Action
     ↓
Transaction Form
     ↓
Input Validation
     ↓
Transaction Model
     ↓
Application State
     ↓
Transaction List + Chart
     ↓
Updated UI
```

The application uses Flutter's built-in `setState()` approach for reactive state updates.

---

## 📂 Project Structure

```text
lib/
│
├── models/
│   └── transaction.dart
│
├── widgets/
│   ├── chart.dart
│   ├── chart_bar.dart
│   ├── new_transaction.dart
│   └── transaction_list.dart
│
└── main.dart
```

### `models/`

Contains the application's data models, including the `Transaction` model.

### `widgets/`

Contains reusable UI components responsible for displaying and interacting with transaction data.

### `main.dart`

Contains the application's entry point and primary application logic.

---

## 🔄 Application Flow

The application follows this general workflow:

```text
                    ┌─────────────────┐
                    │   Launch App    │
                    └────────┬────────┘
                             ↓
                    ┌─────────────────┐
                    │ View Expenses   │
                    └────────┬────────┘
                             ↓
              ┌──────────────┴──────────────┐
              ↓                             ↓
       Add Transaction                 Delete Transaction
              ↓                             ↓
       Validate Input                 Remove Transaction
              ↓                             ↓
       Create Transaction             Update Application State
              └──────────────┬──────────────┘
                             ↓
                    ┌─────────────────┐
                    │ Update Chart    │
                    └─────────────────┘
```

---

## 📊 Weekly Expense Calculation

Expense Insight processes transaction data to generate a visual representation of spending over the previous seven days.

The application:

1. Filters transactions from the recent seven-day period.
2. Groups spending according to the relevant day.
3. Calculates daily spending totals.
4. Determines the relative percentage for each day.
5. Generates chart bars based on those values.
6. Updates the visualization whenever transactions change.

This provided practical experience with Dart collection operations such as:

```dart
where()
fold()
map()
generate()
```

and with date calculations using:

```dart
DateTime
Duration
```

---

## 🧠 Key Software Engineering Concepts

This project demonstrates practical implementation of:

* Object-oriented programming
* Data modeling
* State management
* Component-based architecture
* Separation of concerns
* Form validation
* User input handling
* CRUD-style operations
* Collection processing
* Date manipulation
* Data aggregation
* Conditional rendering
* Responsive UI development
* Reusable widgets
* Cross-platform application development

---

## 🎨 UI & UX

The interface follows **Material Design 3** principles with a focus on simplicity and readability.

Key UI elements include:

* Custom application theme
* Responsive transaction list
* Bottom-sheet transaction form
* Dynamic expense chart
* Empty-state illustration
* Consistent spacing and typography
* Responsive sizing using Flutter layout widgets

The project also uses custom fonts and an application asset for the empty-state experience.

---

## 📸 Screenshots

Add application screenshots to showcase the UI directly on GitHub.

Recommended structure:

```text
screenshots/
├── home-screen.png
├── add-expense.png
├── expense-list.png
└── weekly-chart.png
```

Then display them in the README:

```markdown
## 📸 Screenshots

![Home Screen](screenshots/home-screen.png)

![Add Expense](screenshots/add-expense.png)

![Weekly Expense Chart](screenshots/weekly-chart.png)
```

---

## 🚀 Getting Started

### Prerequisites

Make sure the following are installed:

* Flutter SDK
* Dart SDK
* Android Studio or VS Code
* Android Emulator or physical device
* Git

### 1. Clone the Repository

```bash
git clone https://github.com/Muhammad-Faizan386/Expense-Insight.git
```

### 2. Navigate to the Project

```bash
cd Expense-Insight
```

### 3. Install Dependencies

```bash
flutter pub get
```

### 4. Verify Flutter Setup

```bash
flutter doctor
```

### 5. Run the Application

```bash
flutter run
```

---

## 🧪 Testing

Run Flutter's test suite with:

```bash
flutter test
```

Potential test cases include:

* Adding a valid transaction
* Rejecting invalid amounts
* Handling empty input fields
* Deleting transactions
* Calculating weekly spending
* Rendering the expense chart
* Handling an empty transaction list

---

## 🔮 Future Improvements

The current application provides the core expense-tracking experience. Potential future improvements include:

* [ ] Persistent local database storage
* [ ] Edit existing transactions
* [ ] Expense categories
* [ ] Category-based analytics
* [ ] Monthly spending reports
* [ ] Income tracking
* [ ] Budget limits and alerts
* [ ] Search and filter transactions
* [ ] Dark mode
* [ ] Advanced state management with Provider/Riverpod/Bloc
* [ ] Unit and widget testing
* [ ] Cloud synchronization
* [ ] Authentication and user accounts

---

## 🧠 What I Learned

Building Expense Insight gave me practical experience developing a complete Flutter application rather than focusing only on individual UI screens.

Through this project, I strengthened my understanding of:

* Flutter widget composition
* Dart programming
* Application state management
* Data modeling
* Form validation
* Collection manipulation
* Date and time operations
* Data aggregation
* Interactive data visualization
* Responsive layouts
* Reusable components
* Cross-platform development
* Clean and maintainable code organization

The project also helped me understand how application state flows through a Flutter application and how changes in underlying data can be reflected dynamically in multiple UI components.

---

## 📌 Project Status

**Status:** Completed — portfolio project

The application currently demonstrates the core expense tracking and visualization workflow, with additional features planned for future development.

---

## 👨‍💻 Author

**Muhammad Faizan**

Computer Science Student | Flutter Developer | Associate Software Engineer Aspirant

GitHub: **Muhammad-Faizan386**

---

## 📄 License

This project was developed for educational and portfolio purposes.
