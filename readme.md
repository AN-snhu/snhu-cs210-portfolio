# Corner Grocer - Item Usage Tracker

## Project Summary
The Corner Grocer application is a data analysis tool designed to track frequencies of inventory items. It reads text data from an input file (`CS210_Project_Three_Input_File.txt`), processes the lookups using C++, and outputs a data file (`frequency.dat`). It also utilizes a Python integration script (`report_generator.py`) to handle report generation, allowing user to view a list of all item frequencies as a text-based histogram.

## Reflection

### What I Did Particularly Well
I structured the integration between C++ and Python to leverage both languages. Additionally, designing the object-oriented structure in C++ with an `ItemTracker` making the program easy to follow and modify.

### Areas for Enhancement
To make the application more secure and efficient, I would enhance the file handling mechanisms. Currently, the code assumes the input files are perfectly formatted.

### Challenges Overcome & Support Network
The most challenging part of this assignment was implementing the data serialization to create the `frequency.dat` backup file while simultaneously keeping track of formatting for the user histogram. I overcame this by isolating the logic into class methods and checking my output files incrementally.

### Transferable Skills
The most transferable skill from this project is the ability to connect multiple programming languages together to build a single application. Understanding file input/output streams and data tracking will directly transfer to future coursework in database management and systems architecture.

### Maintainability, Readability, and Adaptability
This application is designed to be highly maintainable and adaptable through:
Modular Code Structure: By utilizing clear header (`.h`) and source (`.cpp`) separation, the core item-tracking logic is completely separated from the execution menu.
Readable Naming Conventions: Functions and variables follow naming styles so any developer can quickly understand the code's intent.
And adaptability Because the Python report script is isolated from the C++ data collector, we could easily rewrite the frontend visualization without needing to change lines in C++.
