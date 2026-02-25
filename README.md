# Temperature-Monitoring-System_AashishKumar_202501100700002

# Problem Statement


1. Build a Python code to display messages according to the temperature received from an assumed IoT system.


2. Accept max and min limit temperature.


3. Generate random values for temperature at every 2 second interval.


4. Compare with the limits to display appropriate value.


# Approach: Temperature Monitoring System


Library Initialization: The script imports random to simulate sensor readings and time to manage the polling frequency (the delay between readings).


Configuration Phase: It prompts the user for specific thresholds (min and max). It uses a try-except block to ensure the program doesn't crash if the user enters text instead of numbers.


The Monitoring Loop:
     
     Data Generation: It uses random.uniform(10.0, 50.0) to generate a float value, mimicking a fluctuating environment.
     
     
     Logic Evaluation: It compares the generated value against the user's defined limits using an if-elif-else structure.
     
     
     Status Reporting: It prints the current time, the temperature, and the status message to the console.
     
     
     Throttling: The time.sleep(2) command prevents the script from consuming excessive CPU power and mimics a standard 2-second sensor sampling rate. 
