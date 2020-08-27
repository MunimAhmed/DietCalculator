#include <iostream>

using namespace std;

void male_function ();
void female_function ();

int main ()
{

int gender;

    cout << "\n\n";
    cout << "This program will calculate your Basal Metabolic Rate and Active Metabolic Rate" << endl;
    cout << "Your BMR will tell you roughly how many calories" << endl;
    cout << "Your body requires in order to sustains it's normal function and" << endl;
     cout << "AMR will tell you how much calories you would burn." << endl;

    cout << "\n\n" << "Let's get started." << endl;
    cout << "\n\n" << "What is your gender? (1 for female, and 2 for male): ";
    cin >> gender;

    while (gender <=0 || gender >= 3)
          {
                  cout << "\n\n" << "I'm sorry, you entered something other than 1 or 2." << endl;
                  cout << "\n\n" << "Please indicate if you are male or female." << endl;
                  cout << "by entering 1 for female or 2 for male: ";
                  cin >> gender;

                  }

if (gender == 1)
{
           female_function ();
}
else
{
           male_function ();
}

}

void female_function()
{
     const int g2SIZE = 7;
     char sex2 [g2SIZE] = "Female";

     cout << "\n\n";
     cout << "You have indicated that you are " << sex2 << endl;
     cout << "\n\n";
     cout << "What is your height in inches? ";

     int height;
     cin >> height; //get height

         while (height < 50 || height > 96)
               {
                       cout << "\n\n";
                       cout << "You must be taller than 50 inches" << endl;
                       cout << "Please enter a height between 50 and 96" << endl;
                       cin >> height;

                       }

cout << "Thank you." << endl;


cout << "\n\n";
cout << "Now, how much do you weight in kg? ";
int weight;
cin >> weight;

while (weight < 18 || weight > 205)
{
cout << "\n\n";
cout << "Please enter a weight more than 40 and 450" << endl;
cin >> weight;
}

cout << "Thank you" << endl;
cout << "\n\n";
cout << "Now how old are you (In Years): "; // get age
int age;
cin >> age;

while (age < 10 || age > 80)
      {
           cout << "\n\n";
           cout << "Im sorry, but this program is not accurate" << endl;
           cout << "Please enter an age beteeen 10 and 80" << endl;
           cin >> age;
           }

cout << "\n\nn" << "Calculating BMR..." << endl;
double amr, bmr;
bmr = 655 + (4.35 * weight * 2.20462) + (4.7 * height) - (4.7 * age);
cout << "\n\n";
cout << "Your Basal Metabolic Rate is " << bmr << "." << endl;
cout << "\n" << "This is roughly the amount of calories your body will burn in a day" << endl;
cout << "without any additional exercise." << endl;

cout << "\n\n" << "Now that you know your Basal Metobolic Rate (BMR)" << endl;
cout << "Let's take a look at your AMR" << endl;
cout << "Your AMR is your BMR adjusted for your activity level. " << endl;

cout << "\n\n";
cout << "Please select your activity level; " << endl;
cout << "-----------------------------------" << endl;
cout << "1. Little to no exercise " << endl;
cout << "2. Light exercise (1-3 days per week) " << endl;
cout << "3. Moderate exercise ( 3-5 days per week) " << endl;
cout << "4. Heavy exercise ( 6-7 days per week ) " << endl;
cout << "5. Very heavy exercise (twice per day, extra heavy workouts) " << endl;
cout << "\n\n" << "Please enter the number to the left of your activity" ;
int selection;
cin>> selection;

if (selection == 1)
{
           amr = bmr * 1.2;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 2)
{
           amr = bmr * 1.375;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 3)
{
           amr = bmr * 1.55;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 4)
{
           amr = bmr * 1.725;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 5)
{
           amr = bmr * 1.9;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}
}

void male_function ()
{
   const int g1SIZE = 7;
     char sex1 [g1SIZE] = "male";

     cout << "\n\n";
     cout << "You have indicated that you are " << sex1 << endl;
     cout << "\n\n";
     cout << "What is your height in inches? ";

     int height;
     cin >> height; //get height

         while (height < 50 || height > 96)
               {
                       cout << "\n\n";
                       cout << "You must be taller than 50 inches" << endl;
                       cout << "Please enter a height between 50 and 96" << endl;
                       cin >> height;

                       }

cout << "Thank you." << endl;


cout << "\n\n";
cout << "Now, how much do you weight in pounds? ";
int weight;
cin >> weight;

while (weight < 40 || weight > 450)
{
cout << "\n\n";
cout << "Please enter a weight more than 40 and 450" << endl;
cin >> weight;
}

cout << "Thank you" << endl;
cout << "\n\n";
cout << "Now how old are you (In Years): "; // get age
int age;
cin >> age;

while (age < 10 || age > 80)
      {
           cout << "\n\n";
           cout << "Im sorry, but this program is not accurate" << endl;
           cout << "Please enter an age beteeen 10 and 80" << endl;
           cin >> age;
           }

cout << "\n\nn" << "Calculating BMR..." << endl;
double amr, bmr;
bmr = 66.5 + (13.75* weight) + (5.003 * height) - (6.755 * age);
cout << "\n\n";
cout << "Your Basal Metabolic Rate is " << bmr << "." << endl;
cout << "\n" << "This is roughly the amount of calories your body will burn in a day" << endl;
cout << "without any additional exercise." << endl;

cout << "\n\n" << "Now that you know your Basal Metobolic Rate (BMR)" << endl;
cout << "Let's take a look at your AMR" << endl;
cout << "Your AMR is your BMR adjusted for your activity level. " << endl;

cout << "\n\n";
cout << "Please select your activity level; " << endl;
cout << "-----------------------------------" << endl;
cout << "1. Little to no exercise " << endl;
cout << "2. Light exercise (1-3 days per week) " << endl;
cout << "3. Moderate exercise ( 3-5 days per week) " << endl;
cout << "4. Heavy exercise ( 6-7 days per week ) " << endl;
cout << "5. Very heavy exercise (twice per day, extra heavy workouts) " << endl;
cout << "\n\n" << "Please enter the number to the left of your activity" ;
int selection;
cin>> selection;

if (selection == 1)
{
           amr = bmr * 1.2;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 2)
{
           amr = bmr * 1.375;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 3)
{
           amr = bmr * 1.55;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 4)
{
           amr = bmr * 1.725;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

if (selection == 5)
{
           amr = bmr * 1.9;
           cout << "\n\n";
           cout << "Your BMR is: " << bmr << endl;
           cout << "Your AMR is: " << amr << endl;
}

}



