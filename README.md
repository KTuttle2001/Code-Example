# Code-Example

#include <iostream>
using namespace std;

int main() {

   int numOne;
   int numTwo;
   int numThree;
   int numFour;
   int numOdd = 0;
   
   cin >> numOne;
   cin >> numTwo;
   cin >> numThree;
   cin >> numFour;
   
   if(numOne % 2 != 0) {
      numOdd = numOdd + 1;
   }
   
   if(numTwo % 2 != 0) {
      numOdd = numOdd + 1;
   }
   
   if(numThree % 2 != 0) {
      numOdd = numOdd + 1;
   }
   
   if(numFour % 2 != 0) {
      numOdd = numOdd + 1;
   }
   
   cout << numOdd << endl;/* Type your code here. */

   return 0;
}

------------------------------------------------------------------------

#include <iostream>
#include <string>
using namespace std;

int main() {

   string firstString;
   string secondString;
   
   getline(cin, firstString);
   getline(cin, secondString);
   
   if(firstString == secondString) {
      cout << "Both phrases match";
   } else if(secondString.find(firstString) != string::npos) {
      cout << firstString << " is found within " << secondString;
   } else if(firstString.find(secondString) != string::npos) {
      cout << secondString << " is found within " << firstString;
   } else {
      cout << "No matches";
   }
   
   cout << endl;/* Type your code here. */

   return 0;
}
