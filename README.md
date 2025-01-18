# Android Calculator App

A modern calculator application built with Jetpack Compose implementing a clean MVVM architecture. The app provides standard arithmetic operations with a sleek, Material Design 3 interface.


## Features

- Material Design 3 UI with Jetpack Compose
- Basic arithmetic operations (addition, subtraction, multiplication, division)
- Decimal number support
- Delete and clear functionalities
- Edge-to-edge design
- Error handling for division by zero
- Number length limitation to prevent overflow
- Clean Architecture using MVVM pattern

## Tech Stack

- **Language**: Kotlin
- **UI Framework**: Jetpack Compose
- **Architecture**: MVVM (Model-View-ViewModel)
- **State Management**: Compose State
- **Lifecycle**: ViewModel from Android Architecture Components

## Project Structure

```
com.example.calculatorapp/
├── ui/
│   ├── components/
│   │   ├── Calculator.kt       # Main calculator composable
│   │   └── CalculatorButton.kt # Reusable button component
│   └── theme/                  # Theme configurations
├── CalculatorAction.kt         # Actions sealed class
├── CalculatorOperation.kt      # Operations sealed class
├── CalculatorState.kt          # State data class
├── CalculatorViewModel.kt      # Business logic
└── MainActivity.kt             # Entry point
```

## Key Components

### Calculator UI
- Built with Jetpack Compose
- Responsive grid layout
- Custom circular buttons
- Real-time calculation display
- Support for portrait orientation

### ViewModel
- Handles all calculator operations
- Manages state using `mutableStateOf`
- Implements number input validation
- Processes arithmetic operations
- Handles decimal points and number deletion

### State Management
- Immutable state using data classes
- State updates through ViewModel
- Clean separation of concerns

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/calculator-app.git
```

2. Open the project in Android Studio

3. Run the app on an emulator or physical device

## Usage

The calculator provides a familiar interface with the following features:

- Numeric keypad (0-9)
- Basic operations (+, -, ×, ÷)
- Clear button (AC)
- Delete button (Del)
- Decimal point
- Equal button (=)

Operations follow standard calculator logic:
1. Enter the first number
2. Select an operation
3. Enter the second number
4. Press equals to see the result
