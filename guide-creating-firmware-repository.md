# Guide: Creating a New Firmware & Flashing Repository

This guide walks you through setting up a new microcontroller or robotics repository so it integrates seamlessly with the **Mustang Way Robots** portal, supports over-the-air/web firmware flashing, and stays clean and organized.

---

## Step 1: Create the Repository on GitHub
1. Go to your GitHub organization (`mustangwayrobots`) and click **New repository**.
2. Give your repository a clear, hyphenated name (e.g., `line-follower-robot` or `sensor-test-node`).
3. Set it to **Public** so students and visitors can access the code and docs.
4. Check the box to **Add a README file**.
5. Click **Create repository**.

---

## Step 2: Add the Required Open-Source License
To ensure our club's code remains open and shareable with the world[cite: 1]:
1. In your new repository, click **Add file > Create new file**.
2. Name the file **`LICENSE`** (exact spelling, no file extension).
3. On the right side, click **Choose a license template** and select the **MIT License**.
4. Click **Commit changes**.

---

## Step 3: Tag It for the Portal (`firmware`)
To make sure your project card automatically displays the **⚡ Flash Firmware** button on the main portal:
1. Look at the right-hand sidebar of your repository homepage under **About**.
2. Click the gear icon or the tags area.
3. Add the topic tag **`firmware`** (along with other helpful tags like `esp32`, `arduino`, or `sensor`).
4. Click **Save changes**.

---

## Step 4: Add the Flash Files (Quickest Method)
Instead of building flashing configuration files from scratch, the easiest method is to copy them directly from an existing working repository (such as `ESP NOW CAR`)[cite: 1]:

1. Open a working repository like `ESP NOW CAR` in another tab[cite: 1].
2. Copy the **`/flash/`** folder (which contains your `manifest.json` configuration)[cite: 1].
3. Paste or recreate that folder structure in your new repository.
4. Update the firmware binary paths inside your `manifest.json` to point to your new compiled build files so the web flasher targets the correct code.

---

## Step 5: Document Your Project in the README
Every good robotics project needs a brief overview so students know how to build it:
* **Overview:** What does this robot or test code do?
* **Hardware Wiring:** List pins, microcontrollers (e.g., ESP32-C3), and motor drivers used.
* **How to Flash:** Mention that visitors can use the ⚡ **Flash Firmware** button directly from the main portal[cite: 1]!
