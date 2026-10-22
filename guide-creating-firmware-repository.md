# Guide: Creating a New Firmware & Flashing Repository

This guide walks teachers and instructors through creating a new microcontroller or robotics repository using our master **`Firmware-Boilerplate`** template. This method ensures your repository automatically integrates with the **Mustang Way Robots** portal, compiles code, supports web-based firmware flashing, and stays clean and organized without manual file copying.

---

## Step 1: Create the Repository from Template
1. Navigate to the master template repository: **`mustangwayrobots/Firmware-Boilerplate`**.
2. Click the green **"Use this template"** button in the top-right area and select **"Create a new repository"**.
3. Under **Owner**, select `mustangwayrobots`.
4. Give your repository a clear, hyphenated name (e.g., `line-follower-robot` or `sensor-test-node`).
5. Set visibility to **Public** so students and visitors can access the code and web flasher.
6. Click **Create repository from template**.

> **Note:** The template automatically includes the pre-configured GitHub Action workflow (`.github/workflows/build.yml`), the web flasher tools (`/flash/`), `.gitignore`, and the MIT License.

---

## Step 2: Enable GitHub Pages for Web Flashing
To allow visitors to flash firmware directly from their web browser:
1. In your new repository, click **Settings** (gear icon) in the top navigation bar.
2. On the left sidebar under *Code and automation*, click **Pages**.
3. Under **Build and deployment > Source**, select **Deploy from a branch**.
4. Under **Branch**, select **`main`** and **`/ (root)`**, then click **Save**.

---

## Step 3: Tag It for the Portal (`firmware`)
To make sure your project card automatically displays on the portal with the **⚡ Flash Firmware** button:
1. Return to your repository's main **Code** page.
2. In the right-hand sidebar under **About**, click the gear icon (or **Edit topics**).
3. Add the required topic tag:
   * **`firmware`** (Required: tells the portal to render the Flash button)
   * *(Optional)* Add relevant hardware tags like `esp32-c3`, `robotics`, or `sensor`.
4. Click **Save changes**.

---

## Step 4: Add Your Arduino / ESP32 Code
1. Add your `.ino` sketch file directly into the root directory of the repository (or edit the starter sketch).
2. Commit your code to the `main` branch.
3. The GitHub Action workflow will automatically trigger, compile your `.ino` file into firmware binaries, and publish them to the `/flash/` web flasher directory on GitHub Pages.

---

## Step 5: Document Your Project in the README
Update the `README.md` file to give students and users an overview of the project:
* **Overview:** What does this robot or firmware code do?
* **Hardware Setup:** List pinout diagrams, microcontrollers used (e.g., ESP32-C3), and connected hardware/drivers.
* **Flashing Instructions:** Remind users they can click the ⚡ **Flash Firmware** button directly on the main portal landing page!
