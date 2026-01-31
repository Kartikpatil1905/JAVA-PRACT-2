# JAVA-PRACT-2
Code: PROBLEM  STATEMENT 1 : 
class Student {
    String name;
    int marks;

    void setData(String n, int a) {
        name = n;
        age = a;
    }
    void displayData() {
        System.out.println("Student Name: " + name);
        System.out.println("Student Age: " + age);
    }
}


public class Main {
    public static void main(String[] args) {
        Student s1 = new Student();
        s1.setData("Kartik", 20);
        s1.displayData();
    }
}

PROBLEM  STATEMENT 2 : 
  class BankAccount {
    String accountHolderName;
    int accountNumber;
    double balance;

    void getAccountDetails(String name, int accNo, double bal) {
        accountHolderName = name;
        accountNumber = accNo;
        balance = bal;
    }

    void deposit(double amount) {
        balance = balance + amount;
    }

    void withdraw(double amount) {
        if (amount <= balance) {
            balance = balance - amount;
        } else {
            System.out.println("Insufficient Balance");
        }
    }

    void displayDetails() {
        System.out.println("Account Holder Name: " + accountHolderName);
        System.out.println("Account Number: " + accountNumber);
        System.out.println("Current Balance: " + balance);
    }
}
public class Main {
    public static void main(String[] args) {
        BankAccount b1 = new BankAccount();

        b1.getAccountDetails("Kartik", 101, 5000);
        b1.deposit(2000);
        b1.withdraw(1000);
        b1.displayDetails();
    }
}
