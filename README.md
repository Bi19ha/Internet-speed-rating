#include <iostream>
using namespace std;

string checkSpeed(int speedMbps) {

	if (speedMbps <=1) {
		return "Very Slow";
	}
	else if (speedMbps <=5) {
		return "Slow";
	}
	else if (speedMbps <=20) {
		return "Average";
	}
	else if (speedMbps <=50) {
		return "Fast";
	}
	else if (speedMbps >=50) {
		return"Very Fast";
	}
}



	int main() {

		int speednit;
		cout << "Enter student's speed nit : " << endl;
		cin >> speednit;


		
		string nit = checkSpeed(speednit);
		cout << "Internet speed : " << speednit << " Rate it :" << nit << endl;


		cin.ignore();
		cin.get();
		return 0;
	}
