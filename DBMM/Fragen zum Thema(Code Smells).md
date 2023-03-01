Code Smells
"Code Smells" are typical errors or problems in code that indicate that the code may need improvement. Here are some of the most common code smells and how to avoid them:

Duplicate Code
Duplicate Code occurs when similar code is repeated at different places in the program. This can affect the maintainability of the code as changes made in one place may need to be made in multiple places.

Avoidance
To avoid Duplicate Code, focus on creating reusability by creating a function or method that can be called at different places in the code.

Long Methods
Long Methods occur when a method becomes too long and has too many responsibilities. This can make the code difficult to read and affect its maintainability.

Avoidance
To avoid Long Methods, break methods into smaller, more specific parts. Each method should only perform one task and be between 5-15 lines long.

Large Classes
Large Classes occur when a class has too many responsibilities and becomes too large. This can make the code difficult to read and affect its maintainability.

Avoidance
To avoid Large Classes, break classes into smaller, more specific classes that are responsible for a specific task.

Shotgun Surgery
Shotgun Surgery occurs when a change in one part of the code requires many changes in other parts. This can affect the maintainability of the code and lead to errors.

Avoidance
To avoid Shotgun Surgery, make changes to the code as locally as possible to minimize the impact on other parts of the code. This can be achieved through the use of design patterns and clean architecture.

Feature Envy
Feature Envy occurs when a method or class uses several properties or functions of another class instead of having its own functions. This can lead to unnecessary dependency problems and make the code difficult to read.

Avoidance
To avoid Feature Envy, classes should only access the properties and functions they need. Classes should not have excessive dependencies on other classes. If a class needs the functions of another class, it may need to be reorganized to integrate the functions into a common class.