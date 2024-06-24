Bank System
Overview
This project is a comprehensive bank system implemented in Python, featuring core banking functionalities such as account management, transaction handling, and balance inquiries. Additionally, the system includes interfaces for ATMs and bank branches, providing multiple points of interaction for users.

Features
1. Account Management:
Create and manage bank accounts with initial deposits and balance tracking.
2. Transaction Handling:
Deposit and withdraw funds, ensuring accurate balance updates and handling insufficient funds.
Maintain a detailed transaction history with type, amount, date, and post-transaction balance.
3. Balance Inquiry:
Real-time balance checks through both ATMs and branches.
4. ATM Interface:
Perform deposits, withdrawals, and balance checks via ATMs.
5. Branch Interface:
Create new accounts, manage existing ones, and provide comprehensive account services.

# Example usage in Python code
bank_system = BankSystem()
branch_1 = Branch("B001", bank_system)
atm_1 = ATM("A001", bank_system)

branch_1.create_account("12345", "Alice", 1000)
branch_1.create_account("67890", "Bob", 500)

atm_1.deposit("12345", 200)
atm_1.withdraw("67890", 100)
atm_1.check_balance("12345")
atm_1.check_balance("67890")

branch_1.print_transaction_history("12345")
branch_1.print_transaction_history("67890")
Project Structure
perl
Copy code
bank-system/
├── bank_system.py     # Main script
├── README.md          # Project documentation

Contributing
Fork the repository.
Create a new branch:
bash
Copy code
git checkout -b feature/your-feature-name
Make your changes and commit them:
bash
Copy code
git commit -m 'Add your commit message'
Push to the branch:
bash
Copy code
Open a pull request.
