<!-- # random-number-taking-from-the-user-game
game of taking random number from the computer -->

#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;
int
main ()
{

  int number, guess, ngusses = 1;
  //  ngusses will count your atttepts ;
  // guess : you have to guess  an interger number ;
  srand (time (0));
  /* it will take some time for giving a
     random number or for generating a number */
  number = rand () % 100 + 1;
  // it will show a random number ;
  cout << " Enter a number  between 1 to 100" << endl;
  do
    {

      cin >> guess;

      if (guess > number)
	cout << " please enter lower number" << endl;
      else if (guess < number)
	cout << " please enter higher number " << endl;

      else
	cout << " You won the game in " << endl;
      cout << ngusses << " attempts" << endl;
      ngusses++;
    }

  while (guess != number);


  return 0;

}

    //  aaya mja game khelne me ?

