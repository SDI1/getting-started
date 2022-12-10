# Starter Project #

## Table of Contents ##

<details>

   <summary>Contents</summary>

   1. [About](#about)
   1. [How to Complete the Project](#how-to-complete-the-project)

</details>

## About ##

This  is a simple introduction to the Git & GitHub workflow.

## How to Complete the Project ##

1. To get started, fork this repository and cd into it.

   ```
   gh repo fork "https://github.com/SDI1/starter-project"
   cd starter-project/
   ```

1. Build and run "hello.cpp"

   ```
   g++ hello.cpp -o hello
   ./hello
   ```

   You should see output like this:

   ![Starter Project Screenshot 1](./img/Starter%20Project%20Screenshot%201.png)

1. You are now going to edit the program to print your name. Create a new branch.

   ```
   git checkout -b "add-name"
   ```

1. Open "hello.cpp" with your favourite text editor or IDE and add the following line.

   ```c++
   cout << "Hello, <insert your name here>!\n";
   ```

   ![Starter Project Screenshot 2](./img/Starter%20Project%20Screenshot%202.png)

1. Build and run again.

   ```
   g++ hello.cpp -o hello
   ./hello
   ```

   This time the program should also display your name.

   ![Starter Project Screenshot 3](./img/Starter%20Project%20Screenshot%203.png)

1. Now commit your changes.

   ```
   git add .
   git commit -m "Add name"
   ```

1. Push your changes to the branch.

   ```
   git push -u origin "add-name"
   ```

1. Open a pull request.

   ```
   gh pr create
   ```