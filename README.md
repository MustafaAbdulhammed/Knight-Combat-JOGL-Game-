# Knight-Combat-JOGL-Game

A 2D fight-based game developed in Java using JOGL, featuring dynamic character animations, sophisticated AI opponents, and precise collision detection for an engaging combat experience. Players control a Knight and battle against various adversaries, including a Samurai Boss, across different difficulty levels.

---

## Table of Contents

- [Key Features & Benefits](#key-features--benefits)
- [Prerequisites & Dependencies](#prerequisites--dependencies)
- [Installation & Setup Instructions](#installation--setup-instructions)
- [Usage Examples](#usage-examples)
- [Configuration Options](#configuration-options)
- [Contributing Guidelines](#contributing-guidelines)
- [License Information](#license-information)
- [Acknowledgments](#acknowledgments)

---

## Key Features & Benefits

This game offers an immersive 2D combat experience with several key highlights:

*   **Engaging 2D Combat System**: Experience responsive and precise fight mechanics, complete with accurately calculated collision boxes for hit detection.
*   **Dynamic Animation States**: Enjoy fluid and realistic character movements for both the player (Knight) and enemy characters (e.g., Samurai Boss). Animations include:
    *   `Attack`
    *   `Run`
    *   `Damaged`
    *   `Dead`
    *   `Shield Parry`
*   **Advanced AI Controller**: Challenge yourself against AI opponents with three distinct difficulty levels:
    *   **Passive (Easy)**: Less aggressive, ideal for learning.
    *   **Balanced (Medium)**: Offers a fair challenge with varied tactics.
    *   **Aggressive (Hard)**: Utilizes pattern recognition for a highly challenging and relentless combat experience.
*   **Custom Texture Management**: Efficient handling of multi-texture assets, allowing for complex character animations and detailed environmental elements, derivative of techniques learned in labs.
*   **JOGL Graphics Integration**: Leverages the power of Java OpenGL (JOGL) for rendering all 2D game elements, ensuring smooth visuals and performance.

---

## Prerequisites & Dependencies

To build and run this project, you will need the following:

*   **Java Development Kit (JDK)**: Version 8 or newer. You can download it from [Oracle's website](https://www.oracle.com/java/technologies/downloads/) or your preferred OpenJDK distribution.
*   **JOGL (Java OpenGL) Libraries**: These are essential for the game's graphics rendering. The project is expected to link against these libraries.
*   **An Integrated Development Environment (IDE)**:
    *   **IntelliJ IDEA**: Highly recommended, as the project structure (`.idea/`, `.iml` files) indicates it was developed within IntelliJ.

---

## Installation & Setup Instructions

Follow these steps to get the Knight Combat game up and running on your local machine:

1.  **Clone the Repository**:
    ```bash
    git clone https://github.com/MustafaAbdulhammed/Knight-Combat-JOGL-Game-.git
    cd Knight-Combat-JOGL-Game-
    ```

2.  **Open with IntelliJ IDEA**:
    *   Launch IntelliJ IDEA.
    *   Go to `File > Open...` and select the cloned `Knight-Combat-JOGL-Game-` directory.

3.  **Configure JOGL Libraries**:
    The project relies on JOGL for rendering. You'll need to ensure the JOGL JARs are properly linked.
    *   Typically, JOGL libraries are placed in a `libraries/` directory within the project or managed through your build system.
    *   In IntelliJ IDEA, navigate to `File > Project Structure > Modules > Dependencies`.
    *   Click the `+` button and select `JARs or Directories...`.
    *   Locate and add all the necessary JOGL JAR files (e.g., `jogl-all.jar`, `gluegen-rt.jar`) to your project's module classpath. If these are available in a `libraries/` directory within this repository, link them from there.

4.  **Build the Project**:
    *   Once the JOGL dependencies are correctly configured, build the project within your IDE. In IntelliJ IDEA, you can usually do this by going to `Build > Build Project`.

---

## Usage Examples

To run and play the game after successful installation:

1.  **Locate the Main Class**:
    *   The entry point for the game will typically be a class with a `public static void main(String[] args)` method, likely within the `src/` directory.

2.  **Run the Game**:
    *   In IntelliJ IDEA, right-click on the main class file (e.g., `Main.java` or `GameRunner.java` if present) and select `Run 'Main'` (or the appropriate run configuration).

3.  **Basic Controls (Inferred)**:
    *   **Movement**: `W`, `A`, `S`, `D` or `Arrow Keys` (Up, Left, Down, Right)
    *   **Attack**: `Spacebar` or `Mouse Click`
    *   **Shield/Parry**: `Shift` key (or another designated key)

---

## Configuration Options

The game offers built-in AI difficulty settings to tailor your single-player experience:

*   **AI Difficulty Levels**: You can select the AI's aggressiveness from three predefined levels:
    *   **Passive (Easy)**
    *   **Balanced (Medium)**
    *   **Aggressive (Hard)**
    *   *Note*: The difficulty increases when triumphed in Singleplayer.

---

## Contributing Guidelines

We welcome contributions to the Knight-Combat-JOGL-Game! If you're interested in improving the project, please follow these guidelines:

1.  **Fork the Repository**: Start by forking the `Knight-Combat-JOGL-Game-` repository to your own GitHub account.
2.  **Create a New Branch**: Create a new branch for your feature or bug fix:
    ```bash
    git checkout -b feature/your-feature-name
    ```
    or
    ```bash
    git checkout -b bugfix/issue-description
    ```
3.  **Make Your Changes**: Implement your changes, ensuring they adhere to the existing coding style.
4.  **Test Your Changes**: Before submitting, thoroughly test your changes to avoid introducing new bugs.
5.  **Commit Your Changes**: Write clear and concise commit messages.
    ```bash
    git commit -m "feat: Add new feature"
    ```
    or
    ```bash
    git commit -m "fix: Resolve bug in collision detection"
    ```
6.  **Push to Your Fork**:
    ```bash
    git push origin feature/your-feature-name
    ```
7.  **Create a Pull Request**: Open a pull request from your forked repository's branch to the `main` branch of the original repository. Provide a detailed description of your changes.

---

## License Information

This project currently has **no specified license**.

It is recommended to add a license file (e.g., MIT, Apache 2.0, GPLv3) to the repository to clarify how others can use, distribute, and contribute to your project. Without a license, all rights are reserved by the copyright holder, and others cannot legally use or modify your work.

---

## Acknowledgments

*   **JOGL Community**: For providing the Java OpenGL libraries that make 2D graphics rendering possible in Java.
*   **Course Labs**: The texture management and animation state concepts are derivative of techniques and assets explored in previous academic labs.
