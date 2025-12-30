# Python for Marine Scientists: A Complete Exercise Guide

This guide provides a progressive learning path from Python basics to marine science applications. Each topic includes classic programming exercises followed by marine science adaptations with realistic datasets.

---

## Topic 1: Variables and Types

### Classic Exercises

1. Create variables to store your name (string), age (integer), height in meters (float), and whether you like programming (boolean). Print each variable with a descriptive label.

2. Create a variable storing the number of days in a week as an integer. Convert it to a float and print both versions.

3. Store a temperature in Fahrenheit (98.6) and convert it to Celsius using the formula: `C = (F - 32) × 5/9`. Print the result.

4. Create variables for three different data types and use the `type()` function to print the type of each variable.

5. Swap values of `a` and `b` without using a third variable.

### Marine Science Exercises

**Dataset (`ocean_measurements.csv`):**

| Location | Depth_m | Temperature_C | Salinity_ppt | pH |
|----------|---------|---------------|--------------|-----|
| Station_A | 15.5 | 18.2 | 35.1 | 8.1 |
| Station_B | 42.0 | 14.7 | 35.8 | 8.0 |
| Station_C | 8.3 | 20.1 | 34.2 | 8.2 |
| Station_D | 65.2 | 12.4 | 36.0 | 7.9 |
| Station_E | 28.7 | 16.8 | 35.4 | 8.1 |

1. Create variables to store measurements from Station_A: depth (float), temperature (float), salinity (float), and pH (float). Print each with labels like "Depth: 15.5 m".

2. Store the depth of Station_B as an integer (42) and convert it to float. Discuss why float might be more appropriate for depth measurements.

3. A fish was measured at 45 cm length. Store this value and convert it to millimeters (multiply by 10). Print both measurements.

4. Create variables for a species name (string), specimen count (integer), average weight in grams (float), and whether the species is endangered (boolean). Use `type()` to verify each variable's type.

---

## Topic 2: Arithmetic and Operators

### Classic Exercises

1. Calculate the area of a rectangle with width 5 and height 12 using multiplication.

2. Calculate the remainder when 47 is divided by 5 using the modulo operator (`%`).

3. Use comparison operators to check if 15 is greater than 10 and if 20 equals 20. Print the results.

4. Calculate compound interest: if you invest $1000 at 5% annual interest for 3 years, what's the final amount? Use the formula: `final = principal * (1 + rate) ** years`

### Marine Science Exercises

**Dataset (`fish_catch.csv`):**

| Species | Count | Total_Weight_kg | Net_Size_cm |
|---------|-------|-----------------|-------------|
| Mackerel | 24 | 18.6 | 50 |
| Herring | 156 | 31.2 | 50 |
| Cod | 8 | 24.0 | 50 |
| Haddock | 12 | 15.6 | 50 |
| Plaice | 18 | 22.5 | 50 |

1. Calculate the average weight per fish for Mackerel: divide total weight (18.6 kg) by count (24). Convert the result to grams.

2. Calculate the catch per unit effort (CPUE): divide the number of Herring caught (156) by the net size in meters (0.5). This gives fish per meter of net.

3. Compare whether Cod had a higher total catch weight than Haddock using comparison operators.

4. Calculate fish density: A sampling quadrat of 2.5m × 2.5m contained 8 juvenile fish. Calculate fish per square meter using the formula: `density = count / (length * width)`.

5. A water sample was taken at 10°C. After 3 hours in the sun, the temperature increased by 2.5°C each hour. Calculate the final temperature using arithmetic operators and exponentiation where needed.

---

## Topic 3: Strings

### Classic Exercises

1. Create a string with your full name and use string methods to: convert it to uppercase, lowercase, and title case.

2. Create two strings: "Hello" and "World". Concatenate them with a space in between.

3. Extract the first 5 characters from the string "Programming is fun" using string slicing.

4. Count how many times the letter 'o' appears in the string "oceanography".

5. Replace the word "bad" with "good" in the string "Today is a bad day".

### Marine Science Exercises

**Dataset (`species_names.csv`):**

| Common_Name | Scientific_Name | Family | Conservation_Status |
|-------------|-----------------|--------|---------------------|
| Blue Whale | Balaenoptera musculus | Balaenopteridae | Endangered |
| Great White Shark | Carcharodon carcharias | Lamnidae | Vulnerable |
| Green Sea Turtle | Chelonia mydas | Cheloniidae | Endangered |
| Clownfish | Amphiprion ocellaris | Pomacentridae | Least Concern |
| Atlantic Cod | Gadus morhua | Gadidae | Vulnerable |

1. Create a string with the scientific name "Balaenoptera musculus" and use string methods to: convert to uppercase, lowercase, and extract just the genus name (first word) using slicing or `.split()`.

2. Concatenate the common name "Green" with "Sea Turtle" using the `+` operator or `.join()` method.

3. A research vessel is named "RV_OCEAN_EXPLORER". Use string methods to replace underscores with spaces and convert to title case for a report.

4. Count how many species in the dataset have "Endangered" in their conservation status. (Practice with a single string first: `"Endangered".count("Endangered")`).

5. Create a standardized species code: take the first 3 letters of "Atlantic" and first 3 letters of "Cod", convert to uppercase, and concatenate (should produce "ATLCOD").

---

## Topic 4: Lists

### Classic Exercises

1. Create a list of 5 numbers. Print the list, then print the first and last elements.

2. Create a list of fruits. Add two more fruits using `.append()` and `.insert()`. Remove one fruit using `.remove()`.

3. Create a list of numbers from 1 to 10. Use slicing to extract the first 5 numbers and the last 3 numbers.

4. Sort a list of random numbers in ascending and descending order.

5. Create two lists and concatenate them into a single list.

### Marine Science Exercises

**Dataset (`daily_temperatures.csv`):**

| Day | Temperature_C | Salinity_ppt | Dissolved_O2_mg_L |
|-----|---------------|--------------|-------------------|
| 1 | 18.5 | 35.2 | 7.8 |
| 2 | 18.8 | 35.1 | 7.9 |
| 3 | 19.2 | 35.3 | 7.7 |
| 4 | 18.9 | 35.2 | 8.0 |
| 5 | 19.5 | 35.0 | 7.6 |
| 6 | 19.8 | 34.9 | 7.5 |
| 7 | 20.1 | 34.8 | 7.4 |

1. Create a list of daily sea temperatures: `[18.5, 18.8, 19.2, 18.9, 19.5, 19.8, 20.1]`. Print the list, the first temperature (Day 1), and the last temperature (Day 7).

2. Create a list of observed fish species: `["Tuna", "Salmon", "Cod"]`. Add "Mackerel" using `.append()` and insert "Herring" at position 1 using `.insert()`. Remove "Salmon" from the list.

3. Create a list of salinity measurements: `[35.2, 35.1, 35.3, 35.2, 35.0, 34.9, 34.8]`. Use slicing to extract the first 3 days and the last 2 days of measurements.

4. Create a list of fish lengths in cm: `[45, 32, 67, 23, 54, 38, 61]`. Sort the list to find the smallest and largest fish. Calculate the range (max - min).

5. You conducted surveys at two sites. Site A species: `["Cod", "Haddock", "Plaice"]`. Site B species: `["Herring", "Mackerel", "Cod"]`. Concatenate these lists to create a complete species list from both sites.

---

## Topic 5: Tuples

### Classic Exercises

1. Create a tuple containing 5 different integers. Try to modify one element and observe what happens.

2. Create a tuple with coordinates (latitude, longitude). Use indexing to access each coordinate.

3. Use tuple unpacking to assign values from a tuple to separate variables.

4. Create a list of tuples, where each tuple represents a (name, age) pair.

### Marine Science Exercises

**Dataset (`sampling_locations.csv`):**

| Station_ID | Latitude | Longitude | Depth_m | Substrate_Type |
|------------|----------|-----------|---------|----------------|
| ST001 | 42.3601 | -71.0589 | 12.5 | Sandy |
| ST002 | 41.8240 | -71.4128 | 8.3 | Rocky |
| ST003 | 42.0654 | -70.1773 | 18.7 | Muddy |
| ST004 | 41.7658 | -71.2515 | 15.2 | Sandy |
| ST005 | 42.2352 | -70.9295 | 22.1 | Rocky |

1. Create a tuple for Station ST001 coordinates: `(42.3601, -71.0589)`. Try to change the latitude value and note that tuples are immutable.

2. Store a sampling location as a tuple: `("ST002", 41.8240, -71.4128, 8.3)`. Use indexing to extract the station ID, latitude, and depth.

3. Use tuple unpacking to assign a location's data to separate variables:
   ```python
   station_data = ("ST003", 42.0654, -70.1773, 18.7, "Muddy")
   station_id, lat, lon, depth, substrate = station_data
   ```

4. Create a list of tuples representing fish measurements: `[("Cod", 45, 1200), ("Haddock", 38, 950), ("Plaice", 32, 780)]`, where each tuple is (species, length_cm, weight_g).

5. Store oceanographic parameters as a tuple: `(18.5, 35.2, 7.8, 8.1)` representing (temperature, salinity, dissolved_oxygen, pH). Explain why tuples are appropriate for fixed measurement sets.

---

## Topic 6: Dictionaries

### Classic Exercises

1. Create a dictionary with keys: "name", "age", "city" and appropriate values. Print the dictionary and access individual values using keys.

2. Add a new key-value pair to an existing dictionary. Update an existing value.

3. Use `.keys()`, `.values()`, and `.items()` methods to explore dictionary contents.

4. Check if a specific key exists in a dictionary using the `in` keyword.

5. Create a nested dictionary (a dictionary containing other dictionaries).

### Marine Science Exercises

**Dataset (`species_database.csv`):**

| Species_ID | Common_Name | Length_cm | Weight_g | Habitat | Trophic_Level |
|------------|-------------|-----------|----------|---------|---------------|
| SP001 | Atlantic Cod | 65 | 2800 | Benthic | 4.2 |
| SP002 | Atlantic Herring | 28 | 180 | Pelagic | 3.1 |
| SP003 | European Plaice | 42 | 950 | Benthic | 3.5 |
| SP004 | Mackerel | 35 | 450 | Pelagic | 3.8 |
| SP005 | Blue Whiting | 32 | 280 | Pelagic | 3.4 |

1. Create a dictionary for Atlantic Cod with keys: "species", "length_cm", "weight_g", "habitat". Print the dictionary and access the length value.

2. Create a dictionary for a water sample: `{"temperature": 18.5, "salinity": 35.2, "pH": 8.1}`. Add a new measurement "dissolved_oxygen": 7.8, then update the temperature to 18.7.

3. Given the dictionary `{"Cod": 12, "Haddock": 8, "Plaice": 15}` representing fish counts, use `.keys()` to list all species, `.values()` to get all counts, and `.items()` to get both.

4. You have a dictionary of observed species: `{"Tuna": 5, "Salmon": 3, "Cod": 12}`. Check if "Herring" was observed using the `in` keyword.

5. Create a nested dictionary for multiple sampling stations:
   ```python
   stations = {
       "ST001": {"depth": 12.5, "temperature": 18.5, "salinity": 35.2},
       "ST002": {"depth": 8.3, "temperature": 19.2, "salinity": 34.8},
       "ST003": {"depth": 18.7, "temperature": 17.6, "salinity": 35.6}
   }
   ```
   Access the temperature at ST002.

---

## Topic 7: Sets

### Classic Exercises

1. Create two sets of numbers. Find the union, intersection, and difference between them.

2. Create a set with duplicate values and observe how sets handle duplicates.

3. Add and remove elements from a set using `.add()` and `.remove()`.

4. Check if one set is a subset of another using `.issubset()`.

### Marine Science Exercises

**Dataset (`site_surveys.csv`):**

| Site | Date | Species_Observed |
|------|------|------------------|
| Beach_A | 2024-01-15 | Cod, Haddock, Plaice, Herring |
| Beach_B | 2024-01-15 | Herring, Mackerel, Cod, Whiting |
| Beach_A | 2024-01-22 | Plaice, Cod, Flounder, Haddock |
| Beach_B | 2024-01-22 | Cod, Mackerel, Herring, Tuna |

1. Create two sets of species observed at different beaches:
   - Beach A: `{"Cod", "Haddock", "Plaice", "Herring"}`
   - Beach B: `{"Herring", "Mackerel", "Cod", "Whiting"}`
   
   Find species found at both beaches (intersection), species found at either beach (union), and species unique to Beach A (difference).

2. A researcher recorded species during multiple observations: `["Cod", "Herring", "Cod", "Plaice", "Herring", "Cod"]`. Convert this list to a set to find unique species observed.

3. Start with a set of protected species: `{"Blue_Whale", "Green_Turtle", "White_Shark"}`. Add "Hammerhead_Shark" using `.add()`. Remove "White_Shark" after re-classification.

4. You have a set of species observed in a marine protected area: `{"Cod", "Haddock", "Plaice"}` and a set of commercially important species: `{"Cod", "Haddock", "Plaice", "Herring", "Mackerel"}`. Check if all protected species are also commercially important using `.issubset()`.

5. Three research vessels surveyed different areas and found:
   - Vessel 1: `{"Tuna", "Marlin", "Swordfish"}`
   - Vessel 2: `{"Tuna", "Mahi-Mahi", "Marlin"}`
   - Vessel 3: `{"Swordfish", "Tuna", "Sailfish"}`
   
   Find species observed by all three vessels (intersection of three sets).

---

## Topic 8: Conditionals (if/elif/else)

### Classic Exercises

1. Write a program that checks if a number is positive, negative, or zero.

2. Create a simple grade classifier: if score >= 90: "A", >= 80: "B", >= 70: "C", else: "F".

3. Check if a number is even or odd using the modulo operator.

4. Write a program that checks if a person is eligible to vote (age >= 18).

5. Use multiple conditions with `and`, `or` to check if a number is between 10 and 20.

### Marine Science Exercises

**Dataset (`water_quality.csv`):**

| Sample_ID | Temperature_C | pH | Dissolved_O2_mg_L | Turbidity_NTU |
|-----------|---------------|-----|-------------------|---------------|
| W001 | 18.5 | 8.1 | 7.8 | 2.3 |
| W002 | 22.3 | 7.6 | 6.2 | 8.5 |
| W003 | 16.8 | 8.3 | 8.5 | 1.8 |
| W004 | 24.7 | 7.4 | 5.8 | 12.1 |
| W005 | 19.2 | 8.0 | 7.5 | 3.2 |

1. Write a program that classifies water temperature: if temp < 15: "Cold", 15-20: "Moderate", > 20: "Warm".

2. Create a pH classifier for seawater quality:
   - pH < 7.5: "Acidic - concerning"
   - pH 7.5-8.3: "Normal range"
   - pH > 8.3: "Alkaline - monitor"

3. Check if dissolved oxygen is adequate for fish survival: if DO >= 6.0 mg/L, print "Sufficient oxygen", else print "Hypoxic conditions - danger to marine life".

4. A fish is considered juvenile if length < 30 cm, adult if length >= 30 cm. Write a conditional to classify a fish measuring 27 cm.

5. Determine water quality status using multiple conditions:
   - If pH is between 7.5-8.3 AND dissolved oxygen > 6.0 AND turbidity < 5.0: "Excellent"
   - Otherwise: "Needs monitoring"
   
   Test with sample W001.

6. Create a fish size classification system:
   - Length < 20 cm: "Small"
   - Length 20-50 cm: "Medium"
   - Length 50-100 cm: "Large"
   - Length > 100 cm: "Very Large"

---

## Topic 9: Loops (for and while)

### Classic Exercises

1. Use a `for` loop to print numbers from 1 to 10.

2. Create a list of numbers and use a `for` loop to print each number multiplied by 2.

3. Use a `while` loop to print numbers from 10 down to 1.

4. Loop through a string and count the number of vowels.

5. Use a `for` loop with `range()` to calculate the sum of numbers from 1 to 100.

6. Loop through a list and use a conditional to print only even numbers.

### Marine Science Exercises

**Dataset (`fish_measurements.csv`):**

| Fish_ID | Species | Length_cm | Weight_g | Sex |
|---------|---------|-----------|----------|-----|
| F001 | Cod | 45 | 1200 | M |
| F002 | Cod | 38 | 890 | F |
| F003 | Haddock | 32 | 650 | M |
| F004 | Plaice | 28 | 480 | F |
| F005 | Cod | 52 | 1580 | M |
| F006 | Haddock | 35 | 720 | F |
| F007 | Plaice | 31 | 550 | M |

1. Create a list of fish lengths: `[45, 38, 32, 28, 52, 35, 31]`. Use a `for` loop to print each length with the label "Fish length: X cm".

2. You have daily temperature readings: `[18.5, 18.8, 19.2, 18.9, 19.5, 19.8, 20.1]`. Use a `for` loop to convert each temperature to Fahrenheit (F = C × 9/5 + 32) and print the results.

3. A water depth sensor takes readings every second. Use a `while` loop to simulate 10 depth readings, starting at 0 meters and increasing by 1.5 meters each time (stop when you reach 10 readings).

4. Loop through the string "Balaenoptera musculus" and count how many times the letter 'a' appears.

5. Calculate the total biomass: fish weights in grams are `[1200, 890, 650, 480, 1580, 720, 550]`. Use a `for` loop to sum all weights and convert to kilograms.

6. Given fish lengths `[45, 38, 32, 28, 52, 35, 31]`, use a loop to count how many fish are longer than 35 cm (potential adults).

7. Loop through a list of species: `["Cod", "Haddock", "Plaice", "Cod", "Cod", "Haddock", "Plaice"]`. Count how many times "Cod" appears in the list.

8. You're monitoring pH levels. Create a list: `[8.1, 7.9, 8.2, 7.6, 8.0, 7.4, 8.1]`. Loop through and print a warning message for any reading below 7.5 or above 8.3.

---

## Topic 10: Functions

### Classic Exercises

1. Write a function that takes two numbers and returns their sum.

2. Create a function that takes a name as input and returns a greeting message.

3. Write a function that calculates the area of a circle given its radius (area = π × r²).

4. Create a function with default parameters: a function that raises a number to a power (default power = 2).

5. Write a function that takes a list of numbers and returns the average.

6. Create a function that checks if a number is prime.

### Marine Science Exercises

**Dataset (`research_data.csv`):**

| Sample_ID | Temperature_C | Salinity_ppt | Species | Count | Length_cm |
|-----------|---------------|--------------|---------|-------|-----------|
| S001 | 18.5 | 35.2 | Cod | 12 | 45 |
| S002 | 19.2 | 34.8 | Haddock | 8 | 38 |
| S003 | 17.8 | 35.6 | Plaice | 15 | 32 |
| S004 | 18.9 | 35.1 | Cod | 10 | 48 |
| S005 | 19.5 | 34.9 | Herring | 24 | 28 |

1. Write a function `celsius_to_fahrenheit(temp_c)` that converts Celsius to Fahrenheit and returns the result. Test with 18.5°C.

2. Create a function `greet_researcher(name)` that takes a researcher's name and returns: "Welcome to the marine lab, [name]!".

3. Write a function `calculate_fish_volume(length_cm)` that estimates fish volume using the simplified formula: volume = 0.01 × length³. Test with a 45 cm fish.

4. Create a function `salinity_status(salinity, threshold=35.0)` that returns "High salinity" if above threshold, "Normal" if equal, or "Low salinity" if below. Use a default threshold of 35.0 ppt.

5. Write a function `average_length(lengths)` that takes a list of fish lengths and returns the mean length. Test with: `[45, 38, 32, 48, 28]`.

6. Create a function `biomass_calculator(count, avg_weight_g)` that returns total biomass in kilograms. Test with 12 fish averaging 1200g each.

7. Write a function `classify_water_temp(temp)` that returns "Cold" (< 15°C), "Moderate" (15-20°C), or "Warm" (> 20°C).

8. Create a function `cpue(catch_count, effort_hours)` that calculates catch per unit effort and returns fish per hour. Include error handling for zero effort.

9. Write a function `species_diversity(species_list)` that takes a list of species names (with duplicates) and returns the number of unique species. Test with: `["Cod", "Haddock", "Cod", "Plaice", "Haddock"]`.

10. Create a function `depth_pressure(depth_m)` that calculates water pressure in atmospheres using: pressure = 1 + (depth / 10). Return the result rounded to 2 decimal places.

---

## Topic 11: File I/O (Optional but Recommended)

### Classic Exercises

1. Write a program that creates a text file and writes 5 lines to it.

2. Read a text file and print its contents line by line.

3. Read a text file and count the number of lines, words, and characters.

4. Append new content to an existing file without overwriting it.

5. Read a CSV file and print each row.

### Marine Science Exercises

**Dataset 1 (`stations.txt`):**
```
Station_A,18.5,35.2,12.5
Station_B,19.2,34.8,8.3
Station_C,17.8,35.6,18.7
Station_D,18.9,35.1,15.2
```

**Dataset 2 (`species_log.csv`):**
```csv
Date,Species,Count,Location
2024-01-15,Cod,12,Harbor_A
2024-01-15,Haddock,8,Harbor_A
2024-01-16,Plaice,15,Harbor_B
2024-01-16,Cod,10,Harbor_A
2024-01-17,Herring,24,Harbor_B
```

1. Create a program that writes oceanographic data to a file `my_measurements.txt`. Write 3 lines containing: station name, temperature, and salinity.

2. Read the `stations.txt` file and print each line. Then parse each line to extract temperature values and print them with labels.

3. Read `species_log.csv` and count:
   - Total number of observations (lines)
   - Total number of fish (sum all counts)
   - Number of different species

4. Append a new observation to `species_log.csv`: add "2024-01-18,Mackerel,18,Harbor_A" without overwriting existing data.

5. Write a program that:
   - Reads `species_log.csv`
   - Calculates total count for each species
   - Writes results to a new file `species_summary.txt`

6. Create a function `read_temperature_data(filename)` that reads a CSV file of temperatures and returns a list of temperature values.

7. Write a program that reads `stations.txt`, converts all temperatures from Celsius to Fahrenheit, and writes the results to a new file `stations_fahrenheit.txt`.

8. Create a simple data logger: write a program that asks the user to input 5 fish measurements (species, length, weight) and saves them to a CSV file with proper formatting.

---

## Mini-Project: Combining All Skills

### Project: Marine Survey Data Analyzer

Create a comprehensive program that combines all learned skills:

**Dataset (`complete_survey.csv`):**

```csv
Date,Station,Species,Count,Avg_Length_cm,Avg_Weight_g,Temperature_C,Salinity_ppt,Depth_m
2024-01-15,ST001,Cod,12,45,1200,18.5,35.2,12.5
2024-01-15,ST001,Haddock,8,38,890,18.5,35.2,12.5
2024-01-15,ST002,Plaice,15,32,650,19.2,34.8,8.3
2024-01-16,ST001,Cod,10,48,1350,18.7,35.1,12.5
2024-01-16,ST002,Herring,24,28,180,19.0,34.9,8.3
2024-01-16,ST003,Cod,14,42,1100,17.8,35.6,18.7
2024-01-17,ST001,Haddock,6,35,720,18.9,35.0,12.5
2024-01-17,ST002,Mackerel,18,35,450,19.5,34.7,8.3
```

**Requirements:**

1. **Data Loading**: Read the CSV file and store data in appropriate data structures (lists, dictionaries).

2. **Statistical Analysis Functions**:
   - Calculate average temperature across all stations
   - Find the station with highest fish diversity
   - Calculate total biomass per species
   - Identify temperature range (min and max)

3. **Data Filtering**:
   - Use conditionals to identify stations with temperature > 19°C
   - Find all Cod observations
   - List dates when more than 10 fish of any species were caught

4. **Reporting**:
   - Generate a summary report showing:
     - Total unique species observed
     - Total fish counted across all surveys
     - Average salinity by station
   - Write results to a new file

5. **Visualization Prep**:
   - Create lists suitable for plotting (dates, temperatures, counts)
   - Calculate daily catch totals

**Bonus Challenges**:
- Add error handling for missing data
- Create a menu system for different analysis options
- Calculate species richness by station
- Identify correlations (e.g., does temperature affect catch size?)

---

## Learning Tips for Marine Scientists

1. **Start Simple**: Master each topic with classic exercises before moving to marine applications.

2. **Practice Daily**: Code for 30 minutes each day rather than long sessions once a week.

3. **Modify Examples**: Take the marine exercises and adapt them to your own research data.

4. **Build Gradually**: Each topic builds on previous ones. Don't skip ahead.

5. **Real Data Next**: Once comfortable with these exercises, start using your actual research data.

6. **Ask Questions**: Python has a helpful community. Search "Python [your problem] marine science" for specific help.

7. **Document Your Code**: Use comments (`#`) to explain what each section does, especially for future reference.

8. **Common Marine Science Python Libraries** (for future learning):
   - `pandas`: Data manipulation and analysis
   - `numpy`: Numerical computing
   - `matplotlib`: Data visualization
   - `scipy`: Scientific computing
   - `xarray`: Multidimensional arrays (oceanographic data)

---

## Next Steps After Completing These Exercises

1. Learn `pandas` for data manipulation with larger datasets
2. Explore `matplotlib` for creating scientific plots
3. Study `numpy` for numerical analysis
4. Investigate domain-specific libraries like `gsw` (Gibbs SeaWater) for oceanographic calculations
5. Practice with real research datasets from your field

Happy coding, and welcome to Python for marine science!

[Solutions](corect/solutions.md)