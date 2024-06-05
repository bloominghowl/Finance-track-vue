# Finance-track-vue
## Finance Tracker - Personal Finance Management App

This repository contains the source code for a Vue.js application designed to help you track your personal finances.  The app allows you to:

- Record income and expenses: Easily add new transactions with text descriptions and amounts.
- Visualize your finances: See your current balance, income, and expenses at a glance.
- Manage transactions: View a list of all your transactions and delete them as needed.

### Features:
- Built with Vue.js for a modern and reactive user interface.
- Clean and intuitive design for easy navigation and data entry.
- Dynamic calculations for total balance, income, and expenses.
- Transaction deletion functionality for managing your financial records.
- Optional local storage integration for persistent data (requires enabling in the code).

### Getting Started
#### 1. Prerequisites:

- Node.js and npm (or yarn) installed on your system.
- Basic understanding of Vue.js concepts is helpful.

### 2. Clone the repository:
```bash
git clone https://github.com/bloominghowl/Finance-track-vue.git
```

### 3. Install dependencies:

```bash
cd client
npm install vue@latest
```
 or
 
```bash
yarn install vue@latest`
```

4. **Run the development server:**

```bash
npm run dev
```
or
```
yarn run dev
```

This will start the development server and open the app in your web browser at http://localhost:8080/.

### Usage

1. Open the app in your web browser at http://localhost:8080/.
2. Use the form in the "Add Transaction" section to enter new transactions with text descriptions and amounts.
3. The app will automatically calculate and display your total balance, income, and expenses.
4. You can view the list of all your transactions in the "History" section.
5. Click the "x" button next to a transaction to delete it.

**Note:** Local storage integration for persistence is currently disabled by default. You may need to modify the code to enable this functionality.

### Project Structure

The project is organized with the following directory structure:
```
src/
App.vue               # Main application component
components/           # Directory for reusable components
Balance.vue         # Component to display balance
Header.vue          # Component for application header
IncomeExpense.vue  # Component to display income and expense
TransactionList.vue # Component to display list of transactions
AddTransaction.vue   # Component for adding new transactions
main.js               # Main application entry point
... (other files)     # Additional files (e.g., styles, utilities)
```
### Author
Angela Ayivi

### Contributing

We currently are not accepting code contributions for this project. However, we welcome bug reports and feature requests.
