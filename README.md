#include <iostream>
#include <filesystem>
#include <vector>
#include <regex>

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

