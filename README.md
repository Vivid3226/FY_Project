# FY_Project
We've have developed group project which contains rock,paper and scissor game using C++ language .. 👍

#include <iostream>
#include <ctime>
using namespace std;

int generateComputerChoice() {
    return rand() % 3; 
}

int main() {
    srand(time(nullptr));
    
    string choices[] = {"Rock", "Paper", "Scissors"};

    int playerChoice, computerChoice;

    cout << "Welcome to Rock, Paper, Scissors!\n";
    cout << "Enter your choice:\n";
    cout << "0: Rock\n";
    cout << "1: Paper\n";
    cout << "2: Scissors\n";
    cin >> playerChoice;






