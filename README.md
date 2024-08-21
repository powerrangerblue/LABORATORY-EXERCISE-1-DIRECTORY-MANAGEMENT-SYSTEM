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
          listFilesMenu();
            break;
        case 2:
           createDirectory();
            break;
        case 3:
           changeDirectory();
            break;
        case 4:
            exit();
            break;
            default:
             cout << "Invalid choice. Please try again.\n";    
    }
}

void listFilesMenu() {
    int choice;
    cout << "\nList Files Menu\n";
    cout << "1. List all files in the current directory\n";
    cout << "2. List files based on a specific extension\n";
    cout << "3. List files based on a pattern\n";
    cout << "Enter your choice: ";
    cin >> choice;
    
switch (choice) {
        case 1:
           cout << "listAllFiles()\n";
            break;
        case 2:
              cout << "listFilesByExtension()\n";
            break;
        case 3:
             cout <<  listFilesByPattern()\n";
            break;
        default:
            cout << "Invalid choice. Returning to main menu.\n";
    }
}







    
       

