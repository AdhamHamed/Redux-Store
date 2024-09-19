# The Redux Store

A simple web application built with React and Redux, where users can log in with a username and password to access a mock banking dashboard. The dashboard includes actions such as deposit, withdraw, request loan, and pay loan, with real-time updates on the user's balance. This project showcases how Redux and Redux Toolkit are used for state management, handling asynchronous actions, and updating the UI based on user interactions.

## Features
- Simple login page (username and password).
- User account dashboard with multiple financial actions: withdraw, deposit, request loan, and pay loan.
- A dynamically updating balance that reflects changes from all actions.

## Skills Demonstrated
### 1. Redux State Management
- The app uses Redux to manage global state for the user balance and financial transactions.
- Redux Toolkit's createSlice is used to create slices for handling login and account actions.

### 2. Asynchronous Actions with Thunks
- Redux Toolkit’s createAsyncThunk is used to handle asynchronous logic, such as simulating the loan request process or transactions that might require server communication.

### 3. Login State Management
- A simple slice manages user authentication and login state.
-- The login action simulates user authentication and controls access to the user dashboard.

### 4. Using Redux Store with useSelector and useDispatch
- Components use useSelector to access the global state (e.g., displaying the current balance) and useDispatch to trigger actions (e.g., deposit, withdraw).

### 5. Real-Time Balance Updates
- The current balance is dynamically updated as users perform actions like depositing or withdrawing money. This demonstrates how Redux can manage and sync state across the application.

### 6. Redux DevTools Support
- Redux DevTools is integrated to help with debugging and tracking state changes in real-time during development.

## Usage
1. On the login page, enter a username and password to log in.
2. Once logged in, the dashboard will display the current balance and available actions:
- Deposit: Add money to the balance.
- Withdraw: Remove money from the balance.
- Request Loan: Request a loan, which will add money to both the loan amount and the balance.
- Pay Loan: Pay off the entire loan amount, deducted from the balance.
3. The balance is updated instantly as actions are performed.

## Core Libraries and Tools
- React: For building the user interface.
- Redux/Redux Toolkit: For managing global state and handling user actions.
- Redux Thunk: For handling asynchronous logic, such as making API calls.
- React-Redux: To connect Redux to React components using hooks like useSelector and useDispatch.
