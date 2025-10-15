<div align="center">

# TypeScript Bootcamp — Elzero Web School 🚀

<img
  src="https://upload.wikimedia.org/wikipedia/commons/4/4c/Typescript_logo_2020.svg"
  alt="TypeScript Logo"
  width="150"
/>

### My Personal Journey to Mastering TypeScript, by Yehia

</div>

> This repository is a comprehensive documentation of everything I have learned and applied during the TypeScript bootcamp from Elzero Web School. Every line of code, every file, and every solution is my personal work, reflecting my learning journey and development in this powerful language.

---

## 📊 Badges & Status

<p align="left">
  <!-- TypeScript Version -->
  <img src="https://img.shields.io/badge/TypeScript-v5.x-blue.svg" alt="TypeScript Version">
  <!-- Repo Stars -->
  <img src="https://img.shields.io/github/stars/YourUsername/TypeScript-Bootcamp-Elzero?style=social" alt="GitHub Stars">
  <!-- License -->
  <img src="https://img.shields.io/github/license/YourUsername/TypeScript-Bootcamp-Elzero" alt="License">
  <!-- Last Commit -->
  <img src="https://img.shields.io/github/last-commit/YourUsername/TypeScript-Bootcamp-Elzero" alt="Last Commit">
  <!-- Repo Size -->
  <img src="https://img.shields.io/github/repo-size/YourUsername/TypeScript-Bootcamp-Elzero" alt="Repo Size">
  <!-- Issues -->
  <img src="https://img.shields.io/github/issues/YourUsername/TypeScript-Bootcamp-Elzero" alt="Open Issues">
  <!-- Pull Requests -->
  <img src="https://img.shields.io/github/issues-pr/YourUsername/TypeScript-Bootcamp-Elzero" alt="Open Pull Requests">
</p>

---

## 📚 Table of Contents

1.  [About The Project](#-about-the-project)
2.  [Key Features](#-key-features)
3.  [Tech Stack](#-tech-stack)
4.  [Project Structure](#-project-structure)
5.  [Getting Started](#-getting-started)
    *   [Prerequisites](#prerequisites)
    *   [Installation & Usage](#installation--usage)
6.  [Code Examples](#-code-examples)
7.  [Assignments Overview](#-assignments-overview)
8.  [What I've Learned](#-what-ive-learned)
9.  [Contributing](#-contributing)
10. [License](#-license)
11. [About The Author](#-about-the-author)
12. [Acknowledgements](#-acknowledgements)

---

## 🎯 About The Project

This repository is more than just a collection of code; it's a living journal of my journey into the world of TypeScript. It serves as a practical portfolio demonstrating my ability to apply theoretical concepts to real-world problems.

**Why did I create this repository?**

*   **For Practical Application:** To transform theoretical knowledge into practical skills.
*   **To Deepen Understanding:** To solidify concepts through practice and repetition.
*   **To Document the Journey:** To build a personal reference that I can return to in the future and showcase to potential employers.

---

## ✨ Key Features

*   **Comprehensive Coverage:** Solutions for a wide range of TypeScript topics, from basic types to advanced features.
*   **Clean & Commented Code:** My solutions are written to be readable and understandable.
*   **Personal Notes:** Includes personal insights and summaries of important concepts.
*   **Practical Challenges:** Real-world exercises to demonstrate a solid grasp of the material.
*   **Structured Learning:** Assignments are organized logically, reflecting the bootcamp's curriculum.

---

## 🛠️ Tech Stack

This project was built using a modern and efficient toolset:

| Tool / Technology         | Version/Details         | Purpose in the Project                                                       |
| ------------------------- | ----------------------- | ---------------------------------------------------------------------------- |
| **TypeScript**            | `~5.x`                  | The core language of the bootcamp, providing safety and robustness to code.      |
| **Node.js**               | `LTS`                   | The runtime environment for executing the compiled JavaScript code.            |
| **ts-node**               | `latest`                | To run TypeScript code directly in a Node.js environment without pre-compilation. |
| **tsc (TypeScript Compiler)**| `~5.x`                  | The official compiler for converting TypeScript to JavaScript.               |
| **pnpm**                  | `latest`                | A fast and disk-space-efficient package manager.                             |

---

## 📂 Project Structure

The repository is organized into folders, with each folder representing a specific assignment or group of assignments.

```
/
├── assignment-1/
│   ├── src/
│   │   └── index.ts         # Solution for assignment 1
│   ├── package.json
│   └── tsconfig.json
│
├── assignment-2/
│   ├── src/
│   │   └── index.ts         # Solution for assignment 2
│   └── ...
│
├── ... (assignments 3 through 26)
│
├── README.md                # This file
└── package.json             # Root package file
```

This structure helps in isolating the context of each assignment, making it easy to navigate and test individual solutions.

---

## 🚀 Getting Started

To run any of the assignments in this repository, follow these simple steps.

### Prerequisites

Make sure you have the following installed on your local machine:

*   [Node.js](https://nodejs.org/) (LTS version recommended)
*   [pnpm](https://pnpm.io/installation) (or you can use `npm` or `yarn`)

### Installation & Usage

1.  **Clone the repository to your local machine:**
    ```bash
    git clone https://github.com/YourUsername/TypeScript-Bootcamp-Elzero.git
    cd TypeScript-Bootcamp-Elzero
    ```

2.  **Navigate to the desired assignment folder:**
    ```bash
    # Example for the first assignment
    cd assignment-1
    ```

3.  **Install the dependencies:**
    ```bash
    # Using pnpm (recommended)
    pnpm install
    
    # Or using npm
    # npm install
    ```

4.  **Compile and run the code:**
    The `tsc` command compiles the `.ts` file into a `.js` file in a `dist` folder, and the `node` command runs the compiled code.
    ```bash
    pnpm tsc && node ./dist/index.js
    ```

---

## 💡 Code Examples

Here are a few examples that showcase the type of code and solutions you'll find in this repository.

**Example 1: Generic Function**

```typescript
// (From Assignment #38)
// A function that accepts an array of any type and returns it.
function getArray<T>(items: T[]): T[] {
  return new Array<T>().concat(items);
}

let numArray = getArray<number>([1, 2, 3]);
let strArray = getArray<string>(["Yehia", "Elzero", "TypeScript"]);

console.log(numArray); // Output: [1, 2, 3]
console.log(strArray); // Output: ["Yehia", "Elzero", "TypeScript"]
```

**Example 2: Using Interfaces**

```typescript
// (From Assignment #19)
interface Game {
  title: string;
  price: number;
  rate?: number; // Optional property
  getDiscount(): string;
  getLocation(): string;
}

// Creating an object that adheres to the Game interface
const gameOne: Game = {
  title: "Ys",
  price: 100,
  rate: 10,
  getDiscount: () => "Discount",
  getLocation: () => "Location"
};

console.log(gameOne.title); // "Ys"
console.log(gameOne.price); // 100
```

---

## 📖 Assignments Overview

This repository covers a wide range of TypeScript topics, from the basics to advanced concepts. Each assignment focuses on a specific aspect of the language.

| Topic                              | Explanation                                                                                         | Relevant Assignments |
| ---------------------------------- | --------------------------------------------------------------------------------------------------- | -------------------- |
| **Type System**                    | Mastering static types like `string`, `number`, `boolean`, `array`, `any`, `unknown`, `void`, `never`. | `1-10`               |
| **Annotations & Inference**        | Understanding how TypeScript infers types and when to use explicit annotations.                     | `11-15`              |
| **Interfaces & Type Aliases**      | Creating custom, reusable types for complex data structures.                                      | `16-20`              |
| **Functions**                      | Typing parameters, return values, and understanding function overloads.                             | `21-26`              |
| **Object-Oriented Programming (OOP)** | Implementing Classes, Interfaces, Inheritance, and Access Modifiers.                              | `27-35`              |
| **Generics**                       | Writing flexible, reusable code that can work with any data type.                                   | `36-40`              |
| **Decorators**                     | Exploring this experimental feature for metaprogramming.                                            | `41-45` (Upcoming)   |
| **Modules & Namespaces**           | Organizing code for better maintainability and scalability.                                         | `46-50` (Upcoming)   |

---

## 🌟 What I've Learned

This bootcamp was a transformative experience that changed how I think about writing code.

*   **A Shift in Mindset:** Moving from dynamic JavaScript to static TypeScript has radically changed how I handle errors, making my applications more robust and stable.
*   **The Power of Interfaces:** I learned how to design cleaner, more predictable data structures and APIs.
*   **Problem-Solving with Generics:** Understanding generics was the biggest challenge, but through constant application, I've become confident in my ability to build reusable, type-safe components.

**My advice to learners:** Don't just watch the lessons. Write the code yourself, solve every exercise, and try to break and fix your code. That's where the real learning happens.

---

## 🤝 Contributing

While this is a personal project, suggestions and improvements are welcome. If you see a better way to solve a problem or want to suggest an improvement, please feel free to open an `Issue` or submit a `Pull Request`.

1.  **Fork the Project**
2.  **Create your Feature Branch** (`git checkout -b feature/AmazingFeature`)
3.  **Commit your Changes** (`git commit -m 'Add some AmazingFeature'`)
4.  **Push to the Branch** (`git push origin feature/AmazingFeature`)
5.  **Open a Pull Request**

---

## 📜 License

This project is licensed under the **MIT License**. See the `LICENSE` file for more details.

---

## 👤 About The Author

I am a passionate developer driven by a love for building elegant, efficient, and scalable web solutions. My programming journey began with a curiosity about how things work, and it has since grown into my career. I believe in continuous learning and am always looking for new challenges.

🔗 **Connect with me:**

*   **GitHub:** [github.com/YourUsername](https://github.com/YourUsername) 🐙
*   **LinkedIn:** [linkedin.com/in/YourProfile](https://linkedin.com/in/YourProfile) 💼
*   **Personal Website:** [your-website.com](https://your-website.com) 🌐

---

## 🙏 Acknowledgements

*   A huge thank you to Eng. **Osama Elzero** and **[Elzero Web School](https://elzero.org/)** for this valuable training bootcamp.
*   Thanks to all the contributors and community members who provide help and inspiration.
*   Shields.io for the awesome badges.


