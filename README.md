# Temperature-Monitoring-System_AashishKumar_202501100700002

# Problem Statement


1. Build a Python code to display messages according to the temperature received from an assumed IoT system.


2. Accept max and min limit temperature.


3. Generate random values for temperature at every 2 second interval.


4. Compare with the limits to display appropriate value.


# Approach: Temperature Monitoring System


1. Library Initialization: The script imports random to simulate sensor readings and time to manage the polling frequency (the delay between readings).


2. Configuration Phase: It prompts the user for specific thresholds (min and max). It uses a try-except block to ensure the program doesn't crash if the user enters text instead of numbers.


3. The Monitoring Loop:
     
     1. Data Generation: It uses random.uniform(10.0, 50.0) to generate a float value, mimicking a fluctuating environment.
     
     
     2. Logic Evaluation: It compares the generated value against the user's defined limits using an if-elif-else structure.
     
     
     3. Status Reporting: It prints the current time, the temperature, and the status message to the console.
     
     
     4. Throttling: The time.sleep(2) command prevents the script from consuming excessive CPU power and mimics a standard 2-second sensor sampling rate.


# Sample Output


If a user sets a Minimum of 20°C and a Maximum of 40°C, the output would look like this:


Enter minimum temperature limit: 20


Enter maximum temperature limit: 40


Monitoring started. Range: 20.0°C - 40.0°C

[14:05:01] Temp: 24.52°C - Temperature is Normal


[14:05:03] Temp: 18.15°C - !! LOW TEMPERATURE ALERT !!


[14:05:05] Temp: 32.88°C - Temperature is Normal


[14:05:07] Temp: 45.10°C - !! HIGH TEMPERATURE ALERT !!


[14:05:09] Temp: 38.92°C - Temperature is Normal

