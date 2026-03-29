<!-- Christine Tobias -->
<!-- Module 5 - CIT-66 Spring2026 -->

Design Plan - “Zookeeper’s Challenge”:

1. Open arrivingAnimals.txt using an ifstream.
2. Open animalNames.txt using an ifstream.
3. Open zooPopulation.txt using an ofstream for final output.
4. Define the base class Animal with fields for name, species, sex, color, origin, birth date, unique ID, age, and weight.
5. Define subclasses Hyena, Lion, Tiger, and Bear that inherit from Animal.
6. Create vectors to store names for each species loaded from animalNames.txt.
7. Create vectors to store final animal objects for each habitat (hyenas, lions, tigers, bears).
8. Initialize integer counters for unique ID generation for each species.
9. Read each line from animalNames.txt.
10. Parse the species and name from each line.
11. Insert each parsed name into the correct species specific name vector.
12. Read each line from arrivingAnimals.txt.
13. Parse the age from the line.
14. Parse the sex from the line.
15. Parse the species from the line.
16. Parse the birth season if it exists.
17. Parse the color descriptor.
18. Parse the weight value.
19. Parse the origin location string.
20. Call genBirthDay() to compute the ISO formatted birth date.
21. Determine the birth year by subtracting the age from the current year.
22. Convert the birth season into a month/day (e.g., spring → 03/21).
23. Construct the final "YYYY-MM-DD" birth date string.
24. Select the next unused name from the species specific name vector.
25. Remove or mark the selected name as used.
26. Call genUniqueID() to generate the species prefix (Hy, Li, Ti, Be).
27. Append the next sequential two digit number to form the unique ID.
28. Increment the species counter.
29. Create an object of the correct subclass (Hyena, Lion, Tiger, or Bear).
30. Assign all parsed and generated attributes to the object.
31. Insert the object into the correct habitat vector.
32. Repeat steps 12–31 for every animal in arrivingAnimals.txt.
33. Write the header "Hyena Habitat:" to zooPopulation.txt.
34. Loop through the hyena vector and write each formatted record.
35. Write the header "Lion Habitat:" to zooPopulation.txt.
36. Loop through the lion vector and write each formatted record.
37. Write the header "Tiger Habitat:" to zooPopulation.txt.
38. Loop through the tiger vector and write each formatted record.
39. Write the header "Bear Habitat:" to zooPopulation.txt.
40. Loop through the bear vector and write each formatted record.
41. Format each output line as: ID; Name; birth date YYYY-MM-DD; color; sex; weight pounds; from origin; arrived YYYY-MM-DD
42. Close all input and output file streams.
43. Wrap file opening operations in try/catch blocks.
44. Throw an exception if any file fails to open.
45. Throw an exception if parsing fails for any animal line.
46. Throw an exception if a species runs out of available names.
47. End the program after confirming all animals were processed and written successfully.
