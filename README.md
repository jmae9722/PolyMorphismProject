
🌀 Polymorphism Project
📌 Overview
This project demonstrates polymorphism in Object-Oriented Programming (OOP) using C++. It includes different shape classes (Circle, Rectangle, Triangle) that inherit from a base Shape class and override its methods.

🛠️ Technologies Used
C++ (Object-Oriented Programming)
Polymorphism (Method Overriding & Virtual Functions)
VS Code (for development)
Git & GitHub (for version control)

📂 Project Structure
📦 PolymorphismProject
 ┣ 📜 README.md             # Project documentation
 ┣ 📜 Shape.h               # Base Shape class (Abstract)
 ┣ 📜 Shape.cpp             # Implementation of base Shape class
 ┣ 📜 Circle.h              # Circle class (inherits Shape)
 ┣ 📜 Circle.cpp            # Implementation of Circle class
 ┣ 📜 Rectangle.h           # Rectangle class (inherits Shape)
 ┣ 📜 Rectangle.cpp         # Implementation of Rectangle class
 ┣ 📜 Triangle.h            # Triangle class (inherits Shape)
 ┣ 📜 Triangle.cpp          # Implementation of Triangle class
 ┗ 📜 main.cpp              # Main program file

📝 How It Works
The Shape class is an abstract base class with a virtual function for calculating the area.
Circle, Rectangle, and Triangle inherit from Shape and override the calculateArea() function.
The main program (main.cpp) creates instances of these shapes and demonstrates polymorphism.

📜 Code Example: Circle.h
The Circle class is a child class of Shape. It inherits from Shape and overrides the calculateArea() method.

#ifndef CIRCLE_H
#define CIRCLE_H

#include "Shape.h"

class Circle : public Shape {
private:
    double radius;

public:
    Circle(double r); // Constructor
    double calculateArea() const override; // Override the calculateArea function
};

#endif // CIRCLE_H

📜 Circle.cpp (Implementation)
#include "Circle.h"
#include <cmath>

Circle::Circle(double r) : radius(r) {}

double Circle::calculateArea() const {
    return M_PI * radius * radius;
}
//End Example//
🚀 How to Run
1️⃣ Clone the Repository
git clone https://github.com/jmae9722/PolyMorphismProject.git
cd PolyMorphismProject

2️⃣ Compile the Code (if using g++)
g++ -o main main.cpp Shape.cpp Circle.cpp Rectangle.cpp Triangle.cpp

3️⃣ Run the Program
./main

💡 Features
✔️ Uses abstract classes and virtual functions
✔️ Demonstrates method overriding for polymorphism
✔️ Uses dynamic memory allocation for objects

🔮 Future Improvements
🔹 Add more shape classes (e.g., Pentagon, Hexagon)
🔹 Implement operator overloading for shape comparison
🔹 Add a GUI visualization using OpenGL or SFML

📜 License
This project is open-source and free to use under the MIT License.

📌 Author
👩🏽‍💻 Mae Hornsby
📌 GitHub: jmae9722# PolyMorphismProject
 
Project Wrap Up Summary: 
✅ Summary of Work Done on the Polymorphism Project (GitHub Setup & Fixes)
🚀 1️⃣ Fixed Repository & GitHub Issues
Removed a duplicate nested .git repository that was causing errors.
Reinitialized Git properly at the correct project folder level.
Set up remote repository (origin) correctly to avoid conflicts.
Successfully pushed all project files (.cpp, .h, README.md).
📄 2️⃣ Created & Updated README.md
Wrote a structured README.md explaining the project.
Included a proper project structure, class explanations, and code examples.
Committed and pushed the README to GitHub successfully.
🔄 3️⃣ Managed Git Workflow
Fixed the error: src refspec main does not match any issue by ensuring the correct branch was used.
Resolved remote origin already exists error by confirming GitHub linkage.
Staged, committed, and pushed changes successfully.
Verified that all files now appear on GitHub (Repo Link).
🛠️ 4️⃣ Future Git Best Practices
Always git pull origin main before making changes to avoid conflicts.
Use git status before committing to check for untracked changes.
Commit with clear messages:
sh
Copy
Edit
git add .
git commit -m "Updated Shape class with new polymorphism method"
git push origin main
Keep the repository clean & organized to avoid duplicate folders.
🎯 Current Status: Everything is Set Up & Working!
✅ Git repository is clean and correctly linked to GitHub.
✅ README is published and visible on GitHub.
✅ All .cpp and .h files are committed & pushed.
✅ No more Git errors.

🚀 How to Edit the README from the Terminal & Push to GitHub
If you need to edit the README.md directly from the terminal and push the changes to GitHub, follow these steps:

1️⃣ Open and Edit the README
To edit the file using nano (or any text editor):

nano README.md
Make your changes inside the file.
Save the file: Press Ctrl + X, then Y, then Enter.
2️⃣ Stage, Commit, and Push Changes
Run the following commands in order:

git add README.md
git commit -m "Updated README with latest changes"
git push origin main
3️⃣ Force Git to Recognize a README Update (If Changes Don’t Show)
If Git doesn’t detect changes or GitHub doesn’t update the README:



echo " " >> README.md  # Adds an empty line to force a change
git add README.md
git commit -m "Force update README"
git push origin main
🎯 Now Your README is Updated on GitHub!
Go to your GitHub repo
Refresh the page 🔄 to see the changes
✅ This method ensures README changes are properly committed and visible on GitHub! 🚀








>>>>>>> 5abbb29 (Restored all project files)
