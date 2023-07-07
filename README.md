# Bank-Application-Project-in-Core-Java
The Core Java Bank Application simulates basic bank functionality, including account creation, fund transfer, balance inquiry, and transaction history. It uses Java collections and exception handling, with a user-friendly interface and secure authentication and encryption features. Regular updates ensure relevance and efficiency.

First, let's create a class called BankAccount that represents a bank account:

public class BankAccount {
    private String accountNumber;
    private String accountHolderName;
    private double balance;

    public BankAccount(String accountNumber, String accountHolderName, double balance) {
        this.accountNumber = accountNumber;
        this.accountHolderName = accountHolderName;
        this.balance = balance;
    }

    public String getAccountNumber() {
        return accountNumber;
    }

    public String getAccountHolderName() {
        return accountHolderName;
    }

    public double getBalance() {
        return balance;
    }

    public void deposit(double amount) {
        balance += amount;
    }

    public void withdraw(double amount) {
        if (balance >= amount) {
            balance -= amount;
        } else {
            System.out.println("Insufficient balance!");
        }
    }
}
