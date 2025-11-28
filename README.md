# 🚀 Asteroid Dodger - Backend System

This repository contains the **backend system** for the **Asteroid Dodger** project.

## 📝 Submission Context

This repository was created specifically to comply with the submission requirement for the backend component only.

The full project, which includes both the frontend and backend, was originally developed under the following repository:
* [**Original Full Stack Repository (Frontend + Backend)**](https://github.com/VirajGandhi07/asteroid-dodger)

Since this repository (`asteroid-dodger-backend`) was created by extracting and cloning only the relevant backend files from the original project, it appears with a single initial commit and **lacks the complete development commit history**. The full history can be found in the original repository linked above.

---

## 💻 Project Structure (Backend)

The backend is built using **.NET 8.0** and is organized into several projects responsible for different data management tasks:

| Project Directory | Description | Technology |
| :--- | :--- | :--- |
| `DataManager/AsteroidManager` | Manages asteroid data, including generation and service logic. | C#, .NET 8.0 |
| `DataManager/PlayerManager` | Handles player profile and data management. | C#, .NET 8.0 |
| `DataManager/GameLauncher` | Acts as the main entry point to run the system, including data analysis and reporting. | C#, .NET 8.0 |
| `DataStorage` | Contains JSON files (`asteroids.json`, `players.json`) used for persistent data storage (simulated database). | JSON |
| `DataManager/Reports` | Contains logic for generating data reports (e.g., `AsteroidReports.cs`). | C#, .NET 8.0 |
| `GDD.md` | The Game Design Document. | Markdown |

---

## ▶️ How to Run the Backend Project

This project is a Console Application and requires the **.NET 8.0 SDK** to be installed on your system.

### Prerequisites

* **[.NET 8.0 SDK](https://dotnet.microsoft.com/download/dotnet/8.0)** (or later)

### Running the Application (GameLauncher)

The primary executable project is **`DataManager/GameLauncher/GameLauncher`**.

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/VirajGandhi07/asteroid-dodger-backend](https://github.com/VirajGandhi07/asteroid-dodger-backend)
    cd asteroid-dodger-backend
    ```

2.  **Navigate to the main project directory:**
    ```bash
    cd DataManager/GameLauncher/GameLauncher
    ```

3.  **Run the project:**
    ```bash
    dotnet run
    ```

The console application will start, and you will see output related to the game's data operations (e.g., generating players/asteroids, running game cycles, generating reports).

### Running Unit Tests

Unit tests are included in the **`.Tests`** projects for each data manager.

1.  **Navigate to the root directory** (if you are not already there):
    ```bash
    cd <path-to-repo-root>/asteroid-dodger-backend
    ```

2.  **Run all tests** within the solution:
    ```bash
    dotnet test
    ```

The output will show the results for all tests in `AsteroidManager.Tests`, `PlayerManager.Tests`, and `GameLauncher.Tests`.

---

## 🛠️ Key Technologies

* **Language:** C#
* **Framework:** .NET 8.0 (Console Application)
* **Testing:** xUnit / Microsoft.NET.Test.Sdk
* **Data Storage:** Local JSON files (simulated persistence)