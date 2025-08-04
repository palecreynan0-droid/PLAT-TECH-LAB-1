# PLAT-TECH-LAB-1
Assignment nako kang sir eric



#include <iostream>
#include <string>

using namespace std;
int main() {
    int myChoice;
    string myString;
    
    cout << "[1] List Files " << endl;
    cout << "[2] Create Directory "<< endl;
    cout << "[3] Change Directory  " << endl;
    cout << "[4] Exit " << endl;
    cout << "Enter your Choice here: " << endl;
    cin >> myChoice;
    
    switch (myChoice) {
           case 1: 
              cout << "[1] List All Files" << endl;
              cout << "[2] List by Extension" << endl;
              cout << "[3] List by Pattern " << endl;
              cout << "Enter your Choice here: " << endl;
              cin >> myChoice;
              
              if (myChoice <= 3) {
                 cout << "- example.txt" << endl;
                 cout << "- programm.cpp" << endl;
                 cout << "- data.csv" << endl;
              }
              else {
                 cout << "error" << endl;
              }
              break;
           case 2:
              cout << "Enter Directory Name: " << endl;
              cin >> myString;
              
              
              if (myString == myString) {
              cout << "Directory '" << myString << "'Created Successfully" << endl;
              }
              
              else {
              cout << "Directory '" << myString << "'Already Exist" << endl;
              }
              break;
           case 3:
              cout << "[1] Move to Parent" << endl;   
              cout << "[2] Move to Root" << endl;
              cout << "[3] Enter Custom Path" << endl;
              cout << "Enter you Choice here: " << endl;
              cin >> myChoice; 
              cout << "Enter path: " << endl;
              cin >> myString;
              
              if (myChoice <= 3) {
                 cout << "Current Directory Changed to: " << myString << endl;
              }
              else {
                 cout << "Error: Directory 'invalid path' not found" << endl;
              }
              break;
           case 4:
             cout << "Exit" << endl;
           break;     
    }
      
    
    return 0;
}
