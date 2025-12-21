# ATM-Interface 

import  java.util.Scanner;
 class BankAccount {
    private double balance;

    BankAccount (double balance){
        this.balance = balance;
    }
     void deposit (double amount ){
        if(amount > 0){
            balance += amount ;
            System.out.println("Amount deposited sucessfully.");
        } else{
            System.out.println("Invalid deposit amount.");
        }
    }
    void withdraw(double amount){
        if(amount > 0 && amount <= balance ){
            balance -= amount;
            System.out.println("Please collect your cash");
        }else {
            System.out.println("Insufficient balance or invalid amount.");
        }
    }
