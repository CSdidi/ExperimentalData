# ExperimentalData
This repository provides the raw experimental data for the paper "How C++ templates are used for generic programming – an empirical study on 50 open source systems". The detailed desciption for each sub-folder is shown in the following:

- BasicInfo
 This folder contains data for "Descriptive Statistics" in Section 5.3.
 -- BasicInfo_0.csv
	This file contains the basic information for each project, including SLOC (source lines of code), number of developers, and project age.
 -- BasicInfo_1
	This folder contains the basic information for each studied historical revision of each project, including SLOC (source lines of code), number of developers, and project age.
 -- BasicInfo_2
	This folder contains the basic information about template definitions and template uses in each project.
 -- BasicInfo_3
	This folder contains information about the use of new template features (variadic function templates, variadic class templates, and alias class templates), their old substitutes, and potential program sites to use new template features.
 -- BasicInfo_4
	This folder contains information about the program sites using implicit type declaration and explicit type declaration
	
- RQ1
  This folder contains data for "RQ1: Are templates practically used to prevent code duplication?" in Section 6.1. For each project, we provide the information of all user-defined function/class templates, including the template's name, the number of template instantiations, the number of multiple overload instantiations, the LOC metric for the template's definition, and the program site (the file and the line number) of the template's definition.
 
- RQ2
  This folder contains data for "RQ2: Are function templates practically used to reduce C-style generics?" in Section 6.2. For each historical revision of each project, we provide the information about three language constructs, including function templates, generic function-like macros, and functions implemented with void*. For each language construct, we show its name, the number of instantiations, the number of multiple overload instantiations, the developer (his/her name and email) who defines this construct, the edit time, and the program site (the file and the line number) of the construct's definition.

- RQ3
  This folder contains data for "RQ3: Are class templates practically used to reduce deep inheritance hierarchies?" in Section 6.3. For each historical revision of each project, we provide the information about two language constructs, including class templates and class inheritance hierarchies.
  For each class template, we show its name, the number of instantiations, the number of multiple overload instantiations, the developer (his/her name and email) who defines this template, the edit time, and the program site (the file and the line number) of the template's definition.
  For each class inheritance hierarchy, we show the name of the base class, the developer (his/her name and email) who defines this base class, the edit time, and the program site (the file and the line number) of the class's definition. Most importantly, we provide the sub-class hierarchies derived from this base class, where "0" stands for the base class, "1" stands for its children, "2" stands for its children's children, etc. If the depth of inheritance exceeds 5, we will regard it as a deep inheritance hierarchy.
  
- RQ4
  This folder contains data for "RQ4: Is CRTP (Curiously Recursive Template Pattern) practically used to reduce virtual functions?" in Section 6.4. For each historical revision of each project, we provide the information about two language constructs, including CRTP and virtual functions.
  For each CRTP, we show the class that implements this CRTP, the number of uses of the CRTP, the developer (his/her name and email) who defines this class, the edit time, and the program site (the file and the line number) of the class's definition.
  For each virtual function, we show the virtual function name, the number of calls, the developer (his/her name and email) who defines this function, the edit time, and the program site (the file and the line number) of the function's definition.

- RQ5
  This folder contains data for "RQ5: Do a small percentage of developers commit a disproportionately large percentage of template uses?" in Section 6.5. For each project, we provide the information of all developers, including the developer's name, the number of code commits, the start/end year of participation in the project, the number of use of library class templates, the number of use of library function templates, the number of use of user-defined class templates, and the number of use of user-defined function templates.

- RQ6
  This folder contains data for "RQ6: Which STL types are used most often?" in Section 6.6. For each project, we provide the information of the applied STL types and their inclusive operations.
  For each STL type, we show its name and the number of instantiations.
  For each STL function (i.e. the inclusive operations of STL types), we show its name and the number of function calls.

- RQ7
  This folder contains data for "RQ7: Are STL types derived less often than user-defined class templates?" in Section 6.7. For each project, we provide the number of derivations of STL types (i.e. library class templates) and the number of derivations of user-defined class templates.


