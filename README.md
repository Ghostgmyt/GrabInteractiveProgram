****Grab Fare & ETA Estimator (C++)****
**Overview**

This is a simple interactive program inspired by Grab ride-hailing. It estimates:

ETA (minutes)

Fare (RM), including surge multiplier, loyalty discounts, and optional tolls

The logic is based on our Part 1 Innovation Model (Disruptive Innovation):

Dynamic Surge Pricing → adapts when demand is higher than supply

Grab Pool option → cheaper access point (low-end disruption)

Tier Discounts → sustaining innovation for loyal users

Features

Interactive input questions (distance, time, demand, supply, tier, service type, toll option)

Adjusted ETA for peak and off-peak traffic

Surge multiplier (up to 3.5x)

Loyalty tier discounts (Basic / Silver / Gold)

Fare recommendation: suggests Pool during high surge short trips

Error handling for invalid inputs (non-numeric, out-of-range values, incorrect yes/no answers)

How to Run
Option 1 – Online Compiler

Paste the program code into an online compiler such as Replit or OnlineGDB.

Compile and run directly.

The program will ask questions step by step.

Option 2 – Local Compilation

On macOS/Linux (Terminal):

cd /Users/mishkumusthafa/Desktop/GrabInteractiveProgram
clang++ -std=c++11 -o grab main.cpp
./grab


On Windows (MinGW):

g++ -std=c++11 -o grab main.cpp
grab.exe

Example Run
**********************************************
        === GRAB Fare & ETA Estimator ===
**********************************************

Enter trip distance in km (0.5 - 100): 7
Enter the hour of the day (0 - 23): 18
On a scale of 1 to 10, how high is the demand? 9
On a scale of 1 to 10, how many drivers (supply) are available? 3
Choose your tier (1 = Basic, 2 = Silver, 3 = Gold): 2
Choose service type (1 = Standard, 2 = Pool): 1
Are there any toll charges? (y/n): y
Enter toll charges (RM): 2.50

**********************************************
                Fare Result
**********************************************
Service       : Standard
Distance (km) : 7
ETA (minutes) : 19
Surge         : x2.25
Tier Discount : 7%
Ride Fare     : RM 38
Toll Charges  : RM 2.50
Estimated Fare: RM 40.50
**********************************************

Tip: POOL may be cheaper now due to high surge on a short trip.

Testing and Debugging

Invalid inputs (letters instead of numbers) are rejected, program re-prompts.

Out-of-range values (e.g., hour = 30) are rejected.

Toll question only accepts "y" or "n" (no accidental defaults).

Validated calculations for surge, discount, tolls, and ETA.

Project Files

main.cpp → C++ source code for the estimator

README.md → documentation and instructions
