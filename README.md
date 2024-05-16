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

    // Validate player's choice
    if (playerChoice < 0 || playerChoice > 2) {
        cout << "Invalid choice. Please enter a number between 0 and 2.\n";
        return 1;
    }

    // Get computer's choice
    computerChoice = generateComputerChoice();

    // Display choices
    cout << "You chose: " << choices[playerChoice] << endl;
    cout<<"Computer Chose"<<choice[computerChoice]<<endl;

    if(playerchoice==computerchoice){
    cout<<"Ohh !! It's Tie :) !!\n";
    }
    else if ((playerChoice == 0 && computerChoice == 2) ||
               (playerChoice == 1 && computerChoice == 0) ||
               (playerChoice == 2 && computerChoice == 1))
    cout<<"You Win!!\n";
    else{
    cout<<"Computer Wins !!\n";
    }
    return 0;
    }
    
    






