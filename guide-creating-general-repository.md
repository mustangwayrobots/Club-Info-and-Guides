# Guide: Creating a General Project Repository

This guide walks through setting up a new repository for 3D printing designs, laser-cut parts, mechanical assemblies, or general documentation using the **`General-Boilerplate`** template. This ensures it integrates seamlessly with the **Mustang Way Robots** portal and follows a clean folder structure.

---

## Step 1: Create the Repository from Template
1. Navigate to the master template repository: **`mustangwayrobots/General-Boilerplate`**.
2. Click the green **"Use this template"** button in the top-right area and select **"Create a new repository"**.
3. Under **Owner**, select `mustangwayrobots`.
4. Give your repository a clear, hyphenated name (e.g., `chassis-mounting-bracket` or `electronics-enclosure-box`).
5. Set the repository to **Public** so students, teachers, and makers can view and download the files.
6. Click **Create repository from template**.

> *Note: If you prefer a completely blank slate instead of a template, you can simply click **New repository** on GitHub, add a README, and add your own MIT license manually.*

---

## Step 2: Tag It for the Portal (`project`)
To make sure your new project automatically appears as a card on the main portal grid:
1. Return to your repository's main **Code** page.
2. Look at the right-hand sidebar under **About** and click the gear icon (or **Edit topics**).
3. Add the required topic tag:
   * **`project`** (Required: tells the portal to render this as a standard project card)
   * *(Optional)* Add helpful tags like `3d-print`, `laser-cut`, `cad`, or `mechanical`.
4. Click **Save changes**.

---

## Step 3: Organize Your Project Files
Keep your file structure clean so anyone can easily find what they need to fabricate or build your design:
* **CAD / Source Files:** Store native editable files (like Fusion 360 exports, SolidWorks, or FreeCAD files) in a folder named `/cad/` or `/source/`.
* **Fabrication Files:** Put ready-to-print or ready-to-cut files in clear folders (e.g., `/stl/` for 3D prints or `/dxf/` for laser cutting).
* **Previews / Renders:** Include a photo or render of the finished physical build in the root directory so it displays nicely in documentation previews.

---

## Step 4: Document Your Project in the README
Every project repository needs a quick explanation in its main `README.md` file so builders know how to make it:
* **Overview:** What is this part, and what robot or project does it belong to?
* **Fabrication Settings:** For 3D prints, note recommended material (e.g., PETG or TPU), infill percentage, and layer height. For laser cutting, note material thickness (e.g., 1/4" acrylic or plywood).
* **Assembly Instructions:** Detail any special hardware, screws, inserts, or steps required to assemble the physical parts.
