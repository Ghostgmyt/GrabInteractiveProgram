GRAB Fare & ETA Estimator
📌 Overview

This is a simple C++ program that estimates Grab ride fares and ETAs.
It is part of our assignment to translate the innovation model into logic/code and demonstrate testing & debugging for a smooth user experience.

The program asks the user for ride details (distance, time, demand, supply, tier, service type, and tolls), applies surge pricing, tier discounts, and calculates an estimated fare.

🛠 Features

Interactive Q&A style input.

Validates all inputs (rejects letters, out-of-range values, etc.).

Handles tolls (asks if applicable, accepts decimal values).

Applies surge pricing based on demand/supply and peak hours.

Applies loyalty tier discounts (Basic, Silver, Gold).

Outputs fare, tolls, and total clearly formatted.

Provides a small tip/recommendation at the end.

📊 Example Run
=== GRAB Fare & ETA Estimator ===
Enter trip distance in km (0.5 - 100): 7
Enter the hour of the day (0 - 23): 18
On a scale of 1 to 10, how high is the demand? 9
On a scale of 1 to 10, how many drivers (supply) are available? 3
Choose your tier (1 = Basic, 2 = Silver, 3 = Gold): 2
Choose service type (1 = Standard, 2 = Pool): 1
Are there any toll charges? (y/n): y
Enter toll charges (RM): 2.50

--- Fare Result ---
Service       : Standard
Distance (km) : 7
ETA (minutes) : 19
Surge         : x2.25
Tier Discount : 7%
Ride Fare     : RM 38
Toll Charges  : RM 2.50
Estimated Fare: RM 40.50
Tip: POOL may be cheaper now due to high surge on a short trip.

🧪 Testing & Debugging

Tested with valid inputs and invalid ones (letters, out-of-range values).

Program now re-prompts for wrong input instead of crashing.

Handles tolls correctly as decimals.

Ensures smoother user experience for assignment requirements.

📂 Project Structure

main.cpp → C++ source code for the estimator

README.md → Documentation (this file)

📌 Notes

This is a student-level program, simplified for assignment use.

Logic and pricing are approximations and not official Grab fares.

Git commit history shows incremental development (inputs → surge logic → toll handling → error handling).
