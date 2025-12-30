"""
Python for Marine Scientists: Complete Exercise Solutions
Author: TheKings294
Date: 2024

This file contains solutions for all exercises with:
- Type hints for all variables and functions
- PEP 8 style compliance
- Clear comments and docstrings
- Best practices for scientific computing
"""
```py
from typing import List, Dict, Tuple, Set, Optional, Union
import math
```

# =============================================================================
# TOPIC 1: VARIABLES AND TYPES
# =============================================================================

```py
def topic1_classic_exercises() -> None:
    """Classic exercises for variables and types."""
    
    # Exercise 1: Create and print variables of different types
    name: str = "Alice"
    age: int = 28
    height: float = 1.75
    likes_programming: bool = True
    
    print(f"Name: {name}")
    print(f"Age: {age}")
    print(f"Height: {height} meters")
    print(f"Likes programming: {likes_programming}")
    
    # Exercise 2: Convert integer to float
    days_in_week: int = 7
    days_as_float: float = float(days_in_week)
    print(f"\nDays as integer: {days_in_week}")
    print(f"Days as float: {days_as_float}")
    
    # Exercise 3: Temperature conversion
    temp_fahrenheit: float = 98.6
    temp_celsius: float = (temp_fahrenheit - 32) * 5 / 9
    print(f"\n{temp_fahrenheit}°F = {temp_celsius:.2f}°C")
    
    # Exercise 4: Using type() function
    sample_string: str = "ocean"
    sample_int: int = 42
    sample_float: float = 3.14
    
    print(f"\nType of '{sample_string}': {type(sample_string)}")
    print(f"Type of {sample_int}: {type(sample_int)}")
    print(f"Type of {sample_float}: {type(sample_float)}")


def topic1_marine_exercises() -> None:
    """Marine science exercises for variables and types."""
    
    # Exercise 1: Station measurements
    depth: float = 15.5
    temperature: float = 18.2
    salinity: float = 35.1
    ph: float = 8.1
    
    print("Station A Measurements:")
    print(f"Depth: {depth} m")
    print(f"Temperature: {temperature} °C")
    print(f"Salinity: {salinity} ppt")
    print(f"pH: {ph}")
    
    # Exercise 2: Integer to float conversion
    depth_int: int = 42
    depth_float: float = float(depth_int)
    print(f"\nDepth as integer: {depth_int}")
    print(f"Depth as float: {depth_float}")
    print("Float is more appropriate for precise depth measurements.")
    
    # Exercise 3: Length conversion
    fish_length_cm: float = 45.0
    fish_length_mm: float = fish_length_cm * 10
    print(f"\nFish length: {fish_length_cm} cm = {fish_length_mm} mm")
    
    # Exercise 4: Multiple variable types
    species_name: str = "Atlantic Cod"
    specimen_count: int = 12
    avg_weight_g: float = 1200.5
    is_endangered: bool = False
    
    print(f"\nSpecies: {species_name}, Type: {type(species_name)}")
    print(f"Count: {specimen_count}, Type: {type(specimen_count)}")
    print(f"Avg Weight: {avg_weight_g}g, Type: {type(avg_weight_g)}")
    print(f"Endangered: {is_endangered}, Type: {type(is_endangered)}")
```

# =============================================================================
# TOPIC 2: ARITHMETIC AND OPERATORS
# =============================================================================

```py
def topic2_classic_exercises() -> None:
    """Classic exercises for arithmetic and operators."""
    
    # Exercise 1: Rectangle area
    width: int = 5
    height: int = 12
    area: int = width * height
    print(f"Rectangle area: {area}")
    
    # Exercise 2: Modulo operator
    dividend: int = 47
    divisor: int = 5
    remainder: int = dividend % divisor
    print(f"\n{dividend} mod {divisor} = {remainder}")
    
    # Exercise 3: Comparison operators
    is_greater: bool = 15 > 10
    is_equal: bool = 20 == 20
    print(f"\n15 > 10: {is_greater}")
    print(f"20 == 20: {is_equal}")
    
    # Exercise 4: Compound interest
    principal: float = 1000.0
    rate: float = 0.05
    years: int = 3
    final_amount: float = principal * (1 + rate) ** years
    print(f"\nInvestment after {years} years: ${final_amount:.2f}")


def topic2_marine_exercises() -> None:
    """Marine science exercises for arithmetic and operators."""
    
    # Exercise 1: Average weight per fish
    total_weight_kg: float = 18.6
    fish_count: int = 24
    avg_weight_kg: float = total_weight_kg / fish_count
    avg_weight_g: float = avg_weight_kg * 1000
    print(f"Average weight per Mackerel: {avg_weight_kg:.3f} kg = {avg_weight_g:.1f} g")
    
    # Exercise 2: Catch per unit effort (CPUE)
    herring_caught: int = 156
    net_size_cm: int = 50
    net_size_m: float = net_size_cm / 100
    cpue: float = herring_caught / net_size_m
    print(f"\nCPUE for Herring: {cpue:.2f} fish per meter")
    
    # Exercise 3: Compare catch weights
    cod_weight: float = 24.0
    haddock_weight: float = 15.6
    cod_heavier: bool = cod_weight > haddock_weight
    print(f"\nCod weight ({cod_weight} kg) > Haddock weight ({haddock_weight} kg): {cod_heavier}")
    
    # Exercise 4: Fish density
    quadrat_length: float = 2.5
    quadrat_width: float = 2.5
    juvenile_count: int = 8
    area: float = quadrat_length * quadrat_width
    density: float = juvenile_count / area
    print(f"\nFish density: {density:.2f} fish per square meter")
    
    # Exercise 5: Temperature increase
    initial_temp: float = 10.0
    temp_increase_per_hour: float = 2.5
    hours: int = 3
    final_temp: float = initial_temp + (temp_increase_per_hour * hours)
    print(f"\nFinal temperature after {hours} hours: {final_temp}°C")
```

# =============================================================================
# TOPIC 3: STRINGS
# =============================================================================

```py
def topic3_classic_exercises() -> None:
    """Classic exercises for strings."""
    
    # Exercise 1: String methods
    full_name: str = "John Smith"
    print(f"Original: {full_name}")
    print(f"Uppercase: {full_name.upper()}")
    print(f"Lowercase: {full_name.lower()}")
    print(f"Title case: {full_name.title()}")
    
    # Exercise 2: String concatenation
    greeting: str = "Hello"
    subject: str = "World"
    message: str = greeting + " " + subject
    print(f"\n{message}")
    
    # Exercise 3: String slicing
    text: str = "Programming is fun"
    first_five: str = text[:5]
    print(f"\nFirst 5 characters: {first_five}")
    
    # Exercise 4: Count character occurrences
    word: str = "oceanography"
    letter: str = "o"
    count: int = word.count(letter)
    print(f"\nLetter '{letter}' appears {count} times in '{word}'")
    
    # Exercise 5: String replacement
    sentence: str = "Today is a bad day"
    new_sentence: str = sentence.replace("bad", "good")
    print(f"\nOriginal: {sentence}")
    print(f"Modified: {new_sentence}")


def topic3_marine_exercises() -> None:
    """Marine science exercises for strings."""
    
    # Exercise 1: Scientific name manipulation
    scientific_name: str = "Balaenoptera musculus"
    print(f"Original: {scientific_name}")
    print(f"Uppercase: {scientific_name.upper()}")
    print(f"Lowercase: {scientific_name.lower()}")
    
    parts: List[str] = scientific_name.split()
    genus: str = parts[0]
    print(f"Genus: {genus}")
    
    # Exercise 2: String concatenation
    common_first: str = "Green"
    common_last: str = "Sea Turtle"
    common_name: str = common_first + " " + common_last
    print(f"\n{common_name}")
    
    # Exercise 3: Format vessel name
    vessel_code: str = "RV_OCEAN_EXPLORER"
    vessel_formatted: str = vessel_code.replace("_", " ").title()
    print(f"\nVessel: {vessel_formatted}")
    
    # Exercise 4: Count conservation status
    status: str = "Endangered"
    count_endangered: int = status.count("Endangered")
    print(f"\n'{status}' contains 'Endangered' {count_endangered} time(s)")
    
    # Exercise 5: Create species code
    species_common: str = "Atlantic Cod"
    words: List[str] = species_common.split()
    code_part1: str = words[0][:3].upper()
    code_part2: str = words[1][:3].upper()
    species_code: str = code_part1 + code_part2
    print(f"\nSpecies code for '{species_common}': {species_code}")
```

# =============================================================================
# TOPIC 4: LISTS
# =============================================================================

```py
def topic4_classic_exercises() -> None:
    """Classic exercises for lists."""
    
    # Exercise 1: Basic list operations
    numbers: List[int] = [3, 7, 12, 18, 25]
    print(f"List: {numbers}")
    print(f"First element: {numbers[0]}")
    print(f"Last element: {numbers[-1]}")
    
    # Exercise 2: List modification
    fruits: List[str] = ["apple", "banana", "orange"]
    fruits.append("mango")
    fruits.insert(1, "grape")
    fruits.remove("banana")
    print(f"\nModified fruits list: {fruits}")
    
    # Exercise 3: List slicing
    full_list: List[int] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    first_five: List[int] = full_list[:5]
    last_three: List[int] = full_list[-3:]
    print(f"\nFirst 5: {first_five}")
    print(f"Last 3: {last_three}")
    
    # Exercise 4: List sorting
    random_numbers: List[int] = [45, 12, 67, 23, 89, 34]
    sorted_asc: List[int] = sorted(random_numbers)
    sorted_desc: List[int] = sorted(random_numbers, reverse=True)
    print(f"\nAscending: {sorted_asc}")
    print(f"Descending: {sorted_desc}")
    
    # Exercise 5: List concatenation
    list1: List[int] = [1, 2, 3]
    list2: List[int] = [4, 5, 6]
    combined: List[int] = list1 + list2
    print(f"\nCombined list: {combined}")


def topic4_marine_exercises() -> None:
    """Marine science exercises for lists."""
    
    # Exercise 1: Temperature list
    temperatures: List[float] = [18.5, 18.8, 19.2, 18.9, 19.5, 19.8, 20.1]
    print(f"Temperatures: {temperatures}")
    print(f"Day 1 temperature: {temperatures[0]}°C")
    print(f"Day 7 temperature: {temperatures[-1]}°C")
    
    # Exercise 2: Species list modification
    species: List[str] = ["Tuna", "Salmon", "Cod"]
    species.append("Mackerel")
    species.insert(1, "Herring")
    species.remove("Salmon")
    print(f"\nSpecies observed: {species}")
    
    # Exercise 3: Salinity slicing
    salinity: List[float] = [35.2, 35.1, 35.3, 35.2, 35.0, 34.9, 34.8]
    first_three_days: List[float] = salinity[:3]
    last_two_days: List[float] = salinity[-2:]
    print(f"\nFirst 3 days salinity: {first_three_days}")
    print(f"Last 2 days salinity: {last_two_days}")
    
    # Exercise 4: Fish length analysis
    fish_lengths: List[int] = [45, 32, 67, 23, 54, 38, 61]
    sorted_lengths: List[int] = sorted(fish_lengths)
    smallest: int = sorted_lengths[0]
    largest: int = sorted_lengths[-1]
    length_range: int = largest - smallest
    print(f"\nSmallest fish: {smallest} cm")
    print(f"Largest fish: {largest} cm")
    print(f"Range: {length_range} cm")
    
    # Exercise 5: Combine survey sites
    site_a: List[str] = ["Cod", "Haddock", "Plaice"]
    site_b: List[str] = ["Herring", "Mackerel", "Cod"]
    all_species: List[str] = site_a + site_b
    print(f"\nAll species from both sites: {all_species}")
```

# =============================================================================
# TOPIC 5: TUPLES
# =============================================================================

```py
def topic5_classic_exercises() -> None:
    """Classic exercises for tuples."""
    
    # Exercise 1: Tuple immutability
    numbers: Tuple[int, ...] = (10, 20, 30, 40, 50)
    print(f"Tuple: {numbers}")
    try:
        # This will raise an error
        numbers[0] = 100  # type: ignore
    except TypeError as e:
        print(f"Error when modifying tuple: {e}")
    
    # Exercise 2: Tuple indexing
    coordinates: Tuple[float, float] = (42.3601, -71.0589)
    latitude: float = coordinates[0]
    longitude: float = coordinates[1]
    print(f"\nLatitude: {latitude}")
    print(f"Longitude: {longitude}")
    
    # Exercise 3: Tuple unpacking
    person_data: Tuple[str, int, str] = ("Alice", 28, "Boston")
    name: str
    age: int
    city: str
    name, age, city = person_data
    print(f"\nName: {name}, Age: {age}, City: {city}")
    
    # Exercise 4: List of tuples
    people: List[Tuple[str, int]] = [
        ("Alice", 28),
        ("Bob", 35),
        ("Charlie", 42)
    ]
    print(f"\nPeople list: {people}")


def topic5_marine_exercises() -> None:
    """Marine science exercises for tuples."""
    
    # Exercise 1: Immutable coordinates
    station_coords: Tuple[float, float] = (42.3601, -71.0589)
    print(f"Station ST001 coordinates: {station_coords}")
    print("Tuples are immutable - cannot modify coordinates")
    
    # Exercise 2: Tuple indexing
    station_data: Tuple[str, float, float, float] = ("ST002", 41.8240, -71.4128, 8.3)
    station_id: str = station_data[0]
    lat: float = station_data[1]
    depth: float = station_data[3]
    print(f"\nStation: {station_id}")
    print(f"Latitude: {lat}")
    print(f"Depth: {depth} m")
    
    # Exercise 3: Tuple unpacking
    location: Tuple[str, float, float, float, str] = ("ST003", 42.0654, -70.1773, 18.7, "Muddy")
    st_id: str
    st_lat: float
    st_lon: float
    st_depth: float
    substrate: str
    st_id, st_lat, st_lon, st_depth, substrate = location
    print(f"\nUnpacked: Station {st_id} at ({st_lat}, {st_lon})")
    print(f"Depth: {st_depth}m, Substrate: {substrate}")
    
    # Exercise 4: List of fish measurements
    fish_measurements: List[Tuple[str, int, int]] = [
        ("Cod", 45, 1200),
        ("Haddock", 38, 950),
        ("Plaice", 32, 780)
    ]
    print("\nFish Measurements:")
    for fish in fish_measurements:
        print(f"  {fish[0]}: {fish[1]}cm, {fish[2]}g")
    
    # Exercise 5: Oceanographic parameters
    ocean_params: Tuple[float, float, float, float] = (18.5, 35.2, 7.8, 8.1)
    temp: float
    salinity: float
    do: float
    ph: float
    temp, salinity, do, ph = ocean_params
    print(f"\nOcean Parameters:")
    print(f"Temperature: {temp}°C, Salinity: {salinity}ppt")
    print(f"DO: {do}mg/L, pH: {ph}")
    print("Tuples are ideal for fixed parameter sets")
```

# =============================================================================
# TOPIC 6: DICTIONARIES
# =============================================================================

```py
def topic6_classic_exercises() -> None:
    """Classic exercises for dictionaries."""
    
    # Exercise 1: Basic dictionary
    person: Dict[str, Union[str, int]] = {
        "name": "Alice",
        "age": 28,
        "city": "Boston"
    }
    print(f"Person: {person}")
    print(f"Name: {person['name']}")
    
    # Exercise 2: Add and update
    person["country"] = "USA"
    person["age"] = 29
    print(f"\nUpdated person: {person}")
    
    # Exercise 3: Dictionary methods
    print(f"\nKeys: {list(person.keys())}")
    print(f"Values: {list(person.values())}")
    print(f"Items: {list(person.items())}")
    
    # Exercise 4: Check key existence
    has_name: bool = "name" in person
    has_email: bool = "email" in person
    print(f"\nHas 'name': {has_name}")
    print(f"Has 'email': {has_email}")
    
    # Exercise 5: Nested dictionary
    employees: Dict[str, Dict[str, Union[str, int]]] = {
        "emp1": {"name": "Alice", "age": 28, "dept": "Science"},
        "emp2": {"name": "Bob", "age": 35, "dept": "Engineering"}
    }
    print(f"\nEmployees: {employees}")


def topic6_marine_exercises() -> None:
    """Marine science exercises for dictionaries."""
    
    # Exercise 1: Species dictionary
    atlantic_cod: Dict[str, Union[str, int]] = {
        "species": "Atlantic Cod",
        "length_cm": 65,
        "weight_g": 2800,
        "habitat": "Benthic"
    }
    print(f"Species data: {atlantic_cod}")
    print(f"Length: {atlantic_cod['length_cm']} cm")
    
    # Exercise 2: Water sample dictionary
    water_sample: Dict[str, float] = {
        "temperature": 18.5,
        "salinity": 35.2,
        "pH": 8.1
    }
    water_sample["dissolved_oxygen"] = 7.8
    water_sample["temperature"] = 18.7
    print(f"\nWater sample: {water_sample}")
    
    # Exercise 3: Fish counts dictionary methods
    fish_counts: Dict[str, int] = {
        "Cod": 12,
        "Haddock": 8,
        "Plaice": 15
    }
    print(f"\nSpecies: {list(fish_counts.keys())}")
    print(f"Counts: {list(fish_counts.values())}")
    print(f"Species-Count pairs: {list(fish_counts.items())}")
    
    # Exercise 4: Check species presence
    observed: Dict[str, int] = {"Tuna": 5, "Salmon": 3, "Cod": 12}
    has_herring: bool = "Herring" in observed
    print(f"\nHerring observed: {has_herring}")
    
    # Exercise 5: Nested station dictionary
    stations: Dict[str, Dict[str, float]] = {
        "ST001": {"depth": 12.5, "temperature": 18.5, "salinity": 35.2},
        "ST002": {"depth": 8.3, "temperature": 19.2, "salinity": 34.8},
        "ST003": {"depth": 18.7, "temperature": 17.6, "salinity": 35.6}
    }
    st002_temp: float = stations["ST002"]["temperature"]
    print(f"\nTemperature at ST002: {st002_temp}°C")
```

# =============================================================================
# TOPIC 7: SETS
# =============================================================================

```py
def topic7_classic_exercises() -> None:
    """Classic exercises for sets."""
    
    # Exercise 1: Set operations
    set1: Set[int] = {1, 2, 3, 4, 5}
    set2: Set[int] = {4, 5, 6, 7, 8}
    
    union: Set[int] = set1 | set2
    intersection: Set[int] = set1 & set2
    difference: Set[int] = set1 - set2
    
    print(f"Set 1: {set1}")
    print(f"Set 2: {set2}")
    print(f"Union: {union}")
    print(f"Intersection: {intersection}")
    print(f"Difference (Set1 - Set2): {difference}")
    
    # Exercise 2: Duplicate handling
    numbers_with_dupes: List[int] = [1, 2, 2, 3, 3, 3, 4, 5, 5]
    unique_numbers: Set[int] = set(numbers_with_dupes)
    print(f"\nOriginal list: {numbers_with_dupes}")
    print(f"Unique values: {unique_numbers}")
    
    # Exercise 3: Add and remove
    fruits: Set[str] = {"apple", "banana", "orange"}
    fruits.add("mango")
    fruits.remove("banana")
    print(f"\nModified set: {fruits}")
    
    # Exercise 4: Subset check
    set_a: Set[int] = {1, 2, 3}
    set_b: Set[int] = {1, 2, 3, 4, 5}
    is_subset: bool = set_a.issubset(set_b)
    print(f"\n{set_a} is subset of {set_b}: {is_subset}")


def topic7_marine_exercises() -> None:
    """Marine science exercises for sets."""
    
    # Exercise 1: Beach species comparison
    beach_a: Set[str] = {"Cod", "Haddock", "Plaice", "Herring"}
    beach_b: Set[str] = {"Herring", "Mackerel", "Cod", "Whiting"}
    
    both_beaches: Set[str] = beach_a & beach_b
    either_beach: Set[str] = beach_a | beach_b
    only_beach_a: Set[str] = beach_a - beach_b
    
    print(f"Beach A species: {beach_a}")
    print(f"Beach B species: {beach_b}")
    print(f"Found at both: {both_beaches}")
    print(f"Found at either: {either_beach}")
    print(f"Only at Beach A: {only_beach_a}")
    
    # Exercise 2: Unique species from observations
    observations: List[str] = ["Cod", "Herring", "Cod", "Plaice", "Herring", "Cod"]
    unique_species: Set[str] = set(observations)
    print(f"\nObservations: {observations}")
    print(f"Unique species: {unique_species}")
    
    # Exercise 3: Protected species management
    protected: Set[str] = {"Blue_Whale", "Green_Turtle", "White_Shark"}
    protected.add("Hammerhead_Shark")
    protected.remove("White_Shark")
    print(f"\nProtected species: {protected}")
    
    # Exercise 4: Subset relationship
    mpa_species: Set[str] = {"Cod", "Haddock", "Plaice"}
    commercial_species: Set[str] = {"Cod", "Haddock", "Plaice", "Herring", "Mackerel"}
    all_commercial: bool = mpa_species.issubset(commercial_species)
    print(f"\nAll MPA species are commercial: {all_commercial}")
    
    # Exercise 5: Multi-vessel intersection
    vessel1: Set[str] = {"Tuna", "Marlin", "Swordfish"}
    vessel2: Set[str] = {"Tuna", "Mahi-Mahi", "Marlin"}
    vessel3: Set[str] = {"Swordfish", "Tuna", "Sailfish"}
    
    all_vessels: Set[str] = vessel1 & vessel2 & vessel3
    print(f"\nSpecies observed by all vessels: {all_vessels}")
```

# =============================================================================
# TOPIC 8: CONDITIONALS
# =============================================================================

```py
def topic8_classic_exercises() -> None:
    """Classic exercises for conditionals."""
    
    # Exercise 1: Positive, negative, or zero
    number: int = 5
    if number > 0:
        print(f"{number} is positive")
    elif number < 0:
        print(f"{number} is negative")
    else:
        print(f"{number} is zero")
    
    # Exercise 2: Grade classifier
    score: int = 85
    if score >= 90:
        grade: str = "A"
    elif score >= 80:
        grade = "B"
    elif score >= 70:
        grade = "C"
    else:
        grade = "F"
    print(f"\nScore {score} = Grade {grade}")
    
    # Exercise 3: Even or odd
    num: int = 42
    if num % 2 == 0:
        print(f"\n{num} is even")
    else:
        print(f"{num} is odd")
    
    # Exercise 4: Voting eligibility
    age: int = 20
    if age >= 18:
        print(f"\nAge {age}: Eligible to vote")
    else:
        print(f"Age {age}: Not eligible to vote")
    
    # Exercise 5: Range check
    value: int = 15
    if 10 <= value <= 20:
        print(f"\n{value} is between 10 and 20")
    else:
        print(f"{value} is not between 10 and 20")


def topic8_marine_exercises() -> None:
    """Marine science exercises for conditionals."""
    
    # Exercise 1: Water temperature classification
    temperature: float = 18.5
    if temperature < 15:
        temp_class: str = "Cold"
    elif 15 <= temperature <= 20:
        temp_class = "Moderate"
    else:
        temp_class = "Warm"
    print(f"Temperature {temperature}°C: {temp_class}")
    
    # Exercise 2: pH classification
    ph: float = 8.1
    if ph < 7.5:
        ph_status: str = "Acidic - concerning"
    elif 7.5 <= ph <= 8.3:
        ph_status = "Normal range"
    else:
        ph_status = "Alkaline - monitor"
    print(f"\npH {ph}: {ph_status}")
    
    # Exercise 3: Dissolved oxygen check
    dissolved_oxygen: float = 7.8
    if dissolved_oxygen >= 6.0:
        print(f"\nDO {dissolved_oxygen} mg/L: Sufficient oxygen")
    else:
        print(f"DO {dissolved_oxygen} mg/L: Hypoxic conditions - danger to marine life")
    
    # Exercise 4: Fish age classification
    fish_length: float = 27.0
    if fish_length < 30:
        age_class: str = "Juvenile"
    else:
        age_class = "Adult"
    print(f"\nFish {fish_length}cm: {age_class}")
    
    # Exercise 5: Water quality assessment
    sample_ph: float = 8.1
    sample_do: float = 7.8
    sample_turbidity: float = 2.3
    
    if (7.5 <= sample_ph <= 8.3) and (sample_do > 6.0) and (sample_turbidity < 5.0):
        quality: str = "Excellent"
    else:
        quality = "Needs monitoring"
    print(f"\nWater quality (pH={sample_ph}, DO={sample_do}, Turbidity={sample_turbidity}): {quality}")
    
    # Exercise 6: Fish size classification
    length: float = 45.0
    if length < 20:
        size: str = "Small"
    elif 20 <= length < 50:
        size = "Medium"
    elif 50 <= length < 100:
        size = "Large"
    else:
        size = "Very Large"
    print(f"\nFish {length}cm: {size}")
```

# =============================================================================
# TOPIC 9: LOOPS
# =============================================================================

```py
print("\n" + "=" * 70)
print("TOPIC 9: LOOPS")
print("=" * 70)

# Classic Exercise 1: Print 1-10
print("\nNumbers 1-10:")
for i in range(1, 11):
    print(i, end=" ")
print()

# Classic Exercise 2: Multiply by 2
numbers: List[int] = [3, 7, 12]
print("Multiplied by 2:")
for n in numbers:
    print(n * 2, end=" ")
print()

# Classic Exercise 3: While countdown
print("Countdown:")
count: int = 10
while count >= 1:
    print(count, end=" ")
    count -= 1
print()

# Classic Exercise 4: Count vowels
test_str: str = "oceanography"
vowels: str = "aeiou"
vowel_count: int = sum(1 for char in test_str.lower() if char in vowels)
print(f"Vowels in '{test_str}': {vowel_count}")

# Classic Exercise 5: Sum 1-100
total: int = sum(range(1, 101))
print(f"Sum 1-100: {total}")

# Classic Exercise 6: Print even numbers
all_nums: List[int] = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
print("Even numbers:")
for num in all_nums:
    if num % 2 == 0:
        print(num, end=" ")
print()

# Marine Exercises
print("\n--- MARINE EXERCISES ---")
fish_lengths: List[int] = [45, 38, 32, 28, 52]
print("Fish lengths:")
for length in fish_lengths:
    print(f"  {length}cm")

daily_temps: List[float] = [18.5, 18.8, 19.2]
print("Temperatures in Fahrenheit:")
for celsius in daily_temps:
    fahrenheit: float = celsius * 9/5 + 32
    print(f"  {celsius}°C = {fahrenheit:.1f}°F")

print("Depth readings:")
depth: float = 0.0
reading_count: int = 0
while reading_count < 5:
    print(f"  Reading {reading_count + 1}: {depth:.1f}m")
    depth += 1.5
    reading_count += 1

species_str: str = "Balaenoptera musculus"
a_count: int = species_str.lower().count('a')
print(f"Letter 'a' in '{species_str}': {a_count}")

weights: List[int] = [1200, 890, 650, 480, 1580]
total_weight: int = sum(weights)
total_kg: float = total_weight / 1000
print(f"Total biomass: {total_weight}g = {total_kg}kg")

adult_count: int = sum(1 for l in fish_lengths if l > 35)
print(f"Fish > 35cm (adults): {adult_count}")
```

# =============================================================================
# TOPIC 10: FUNCTIONS
# =============================================================================

```py
print("\n" + "=" * 70)
print("TOPIC 10: FUNCTIONS")
print("=" * 70)

# Classic Exercise 1: Sum function
def add_numbers(a: float, b: float) -> float:
    """Return the sum of two numbers."""
    return a + b

print(f"\nadd_numbers(5, 3) = {add_numbers(5, 3)}")

# Classic Exercise 2: Greeting function
def greet(name: str) -> str:
    """Return a greeting message."""
    return f"Hello, {name}!"

print(greet("Alice"))

# Classic Exercise 3: Circle area
def circle_area(radius: float) -> float:
    """Calculate the area of a circle."""
    return math.pi * radius ** 2

print(f"Circle area (r=5): {circle_area(5):.2f}")

# Classic Exercise 4: Power function with default
def power(base: float, exponent: float = 2) -> float:
    """Raise base to exponent (default 2)."""
    return base ** exponent

print(f"power(3) = {power(3)}, power(3, 3) = {power(3, 3)}")

# Classic Exercise 5: Average
def average(numbers: List[float]) -> float:
    """Calculate the average of a list of numbers."""
    return sum(numbers) / len(numbers)

print(f"average([10, 20, 30]) = {average([10, 20, 30])}")

# Classic Exercise 6: Prime check
def is_prime(n: int) -> bool:
    """Check if a number is prime."""
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

print(f"is_prime(17) = {is_prime(17)}, is_prime(18) = {is_prime(18)}")

# Marine Exercises
print("\n--- MARINE EXERCISES ---")

def celsius_to_fahrenheit(temp_c: float) -> float:
    """Convert Celsius to Fahrenheit."""
    return temp_c * 9/5 + 32

print(f"18.5°C = {celsius_to_fahrenheit(18.5):.1f}°F")

def greet_researcher(name: str) -> str:
    """Greet a marine researcher."""
    return f"Welcome to the marine lab, {name}!"

print(greet_researcher("Dr. Smith"))

def calculate_fish_volume(length_cm: float) -> float:
    """Estimate fish volume using simplified formula."""
    return 0.01 * length_cm ** 3

print(f"Fish volume (45cm): {calculate_fish_volume(45):.2f} cm³")

def salinity_status(salinity: float, threshold: float = 35.0) -> str:
    """Classify salinity level."""
    if salinity > threshold:
        return "High salinity"
    elif salinity == threshold:
        return "Normal"
    else:
        return "Low salinity"

print(f"Salinity 35.5: {salinity_status(35.5)}")

def average_length(lengths: List[float]) -> float:
    """Calculate mean fish length."""
    return sum(lengths) / len(lengths)

print(f"Average length: {average_length([45, 38, 32, 48, 28]):.2f}cm")

def biomass_calculator(count: int, avg_weight_g: float) -> float:
    """Calculate total biomass in kilograms."""
    return (count * avg_weight_g) / 1000

print(f"Biomass (12 fish × 1200g): {biomass_calculator(12, 1200):.2f}kg")

def classify_water_temp(temp: float) -> str:
    """Classify water temperature."""
    if temp < 15:
        return "Cold"
    elif 15 <= temp <= 20:
        return "Moderate"
    else:
        return "Warm"

print(f"18.5°C is: {classify_water_temp(18.5)}")

def cpue(catch_count: int, effort_hours: float) -> Optional[float]:
    """Calculate catch per unit effort."""
    if effort_hours == 0:
        print("Error: Cannot divide by zero effort")
        return None
    return catch_count / effort_hours

print(f"CPUE (24 fish / 4 hours): {cpue(24, 4):.2f} fish/hour")

def species_diversity(species_list: List[str]) -> int:
    """Count unique species."""
    return len(set(species_list))

print(f"Diversity: {species_diversity(['Cod', 'Haddock', 'Cod', 'Plaice'])}")

def depth_pressure(depth_m: float) -> float:
    """Calculate water pressure in atmospheres."""
    return round(1 + (depth_m / 10), 2)

print(f"Pressure at 15m: {depth_pressure(15)} atm")
```

# =============================================================================
# TOPIC 11: FILE I/O
# =============================================================================

```py
print("\n" + "=" * 70)
print("TOPIC 11: FILE I/O")
print("=" * 70)

# Classic Exercise 1: Write to file
def write_sample_file() -> None:
    """Create a sample text file."""
    with open("sample.txt", "w") as file:
        for i in range(1, 6):
            file.write(f"Line {i}\n")
    print("\nWrote 5 lines to sample.txt")

write_sample_file()

# Classic Exercise 2: Read file
def read_file_lines(filename: str) -> None:
    """Read and print file contents."""
    try:
        with open(filename, "r") as file:
            for line in file:
                print(line.strip())
    except FileNotFoundError:
        print(f"File {filename} not found")

print("\nReading sample.txt:")
read_file_lines("sample.txt")

# Classic Exercise 3: Count lines, words, characters
def count_file_stats(filename: str) -> Tuple[int, int, int]:
    """Count lines, words, and characters in a file."""
    try:
        with open(filename, "r") as file:
            content: str = file.read()
            lines: int = content.count('\n')
            words: int = len(content.split())
            chars: int = len(content)
            return lines, words, chars
    except FileNotFoundError:
        return 0, 0, 0

lines, words, chars = count_file_stats("sample.txt")
print(f"\nFile stats: {lines} lines, {words} words, {chars} characters")

# Classic Exercise 4: Append to file
def append_to_file(filename: str, content: str) -> None:
    """Append content to a file."""
    with open(filename, "a") as file:
        file.write(content + "\n")
    print(f"Appended to {filename}")

append_to_file("sample.txt", "Line 6 - Appended")

# Marine Exercise 1: Write oceanographic data
def write_ocean_data() -> None:
    """Write oceanographic measurements to file."""
    with open("my_measurements.txt", "w") as file:
        file.write("Station_A,18.5,35.2\n")
        file.write("Station_B,19.2,34.8\n")
        file.write("Station_C,17.8,35.6\n")
    print("\nWrote oceanographic data to my_measurements.txt")

write_ocean_data()
```