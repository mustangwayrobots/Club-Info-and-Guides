# Guide: Creating a New Firmware & Flashing Repository

This guide walks you through setting up a new microcontroller or robotics repository so it integrates seamlessly with the **Mustang Way Robots** portal, supports web firmware flashing, and stays clean and organized.

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

## Step 4: Add the Flashing Files (`/flash/`)
To enable browser-based flashing directly from the portal, your repository needs a `/flash/` directory:
1. Copy the **`/flash/`** folder (which includes the `index.html` file and your compiled build files) directly from an existing working repository like `ESP NOW CAR`[cite: 1].
2. Paste or upload it into your new repository. 
3. *Note:* Because these files are written to be generic, you generally do not need to modify them—they will automatically look for and flash the binary builds inside your repository!

---

## Step 5: Enable GitHub Pages for Web Flashing
So the web flasher can run live in the browser via GitHub Pages:
1. In your repository, click **Settings** in the top navigation bar.
2. On the left sidebar, click **Pages**.
3. Under **Build and deployment > Source**, select **Deploy from a branch**.
4. Set the branch to **`main`** (and `/ (root)`), then click **Save**.

---

## Step 6: Document Your Project in the README
Every good robotics project needs a brief overview so students know how to build it:
* **Overview:** What does this robot or test code do?
* **Hardware Wiring:** List pins, microcontrollers (e.g., ESP32-C3), and motor drivers used.
* **How to Flash:** Mention that visitors can use the ⚡ **Flash Firmware** button directly from the main portal[cite: 1]!
