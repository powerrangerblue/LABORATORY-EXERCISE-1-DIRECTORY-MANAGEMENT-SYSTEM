#include <iostream>
#include <filesystem>
#include <vector>
#include <regex>

namespace fs = std: : filesystem;
using namespace std;

void displayMainMenu();
void handleMainMenuSelection (int choice);
void listFilesMenu();
void listAllFiles();
void listFilesByExtension();
void listFilesByPattern();
void createDirectory();
void changeDirectory();
void diaplayDirectoryMenu();
void handleDirectorySelection (int choice);
void exitProgram();

int main() {
    int choice;
    do {
       displayMainMenu();
       cin >> choice;
       handleMainMenuSelection(choice);
    } while (choice != 4);
    return 0;
}

void diaplayMainMenu() {
      cout << "\nDirectory Management System\n";
      cout << "1. To Display List of Files\n";
      cout << "2. To Create New Directory\n";
      cout << "3. To Change the Working Directory\n";
      cout << "4. Exit\n";
      cout << "Enter your choice: ";
}

void handleMainMenuSelection (int choice) {
    switch (choice) {
        case 1:
            cout << "listFilesMenu()\n";
            break;
        case 2:
            createDirectory()\n;
            break;
        case 3:
            changeDirectory();
            break;
        case 4:
            exitProgram();
            break;
        default:
            cerr << "Invalid choice. Please try again.\n";
    }
}







    
       

