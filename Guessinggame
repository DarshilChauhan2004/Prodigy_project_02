#include<iostream>
#include<cstdlib>
#include<ctime>
using namespace std;
int main()
{
	label:
	srand((unsigned) time(0)); //In every execution the random number changes
	int random = 0;
	cout<<"The Guessing Game:"<<endl;
	cout<<"----Enter a guess between 1 to 100----"<<endl;
	cout<<"----You have 5 tries to guess it right----\n"<<endl;
	
	random = (rand()%100)+1;   // Generates random numbers b/w 1 and 100 inclusive
    
    char op;
	int a = 1;
	int turns = 0;
	int turns_left = 5;
	do{
	int guess;
    cout<<"\nYour turns: "<<turns_left<<endl;	
	cout<<"Your guess:"<<endl;
	cin>>guess;
	turns_left--;
	if(turns==5||turns_left==0){
		cout<<"\nOh no!!!";
		cout<<"\nYour tries have been finished\n";
		cout<<"The secret number was "<<random<<endl;
		break;
	}
	if(guess>random){
		cout<<"Try a smaller number:"<<endl;
		turns ++;
	}
	else if(guess<random){
		cout<<"Try a larger number:"<<endl;
		turns ++;
	}
	else{
		cout<<"You Guessed the Number!"<<endl;
		cout<<"Congratulations, You won the game!"<<endl;
		a = 0;
	}
}
  while(a==1);
	cout<<"\n\nGAME OVER"<<endl;
	cout<<"Would you like to play again?(y/n)"<<endl;
	cin>>op;
	if(op=='y'||op=='Y'){
		goto label;  //Use of goto statement is highly discouraged!
	}
	else{
		cout<<"Exiting the game......."<<endl;
	}
}
