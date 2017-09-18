# Killometers
Soource File: Killometers


//Killometers.cpp
#include <fstream>
#include <string>
#include <iostream>
using namespace std;
int main() 
{
	string klm;
	ifstream takeData;
	ofstream saveData;
	takeData.open("data.dat");
	takeData >> klm;
	takeData.close();
	cout << "The last killometers of your bike was : " << klm  ;
	cout << "\nGive me your bike killometers: \n";
	cin >> klm ;
	saveData.open("data.dat");
	saveData << klm;
	saveData.close();
return 0;
}
