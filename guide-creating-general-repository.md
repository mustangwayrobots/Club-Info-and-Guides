# Guide: Creating a General Project Repository

This guide walks you through setting up a new repository for 3D printing designs, laser-cut parts, mechanical assemblies, or general non-firmware hardware projects for the **Mustang Way Robots** portal.

---

## Step 1: Create the Repository on GitHub
1. Go to your GitHub organization (`mustangwayrobots`) and click **New repository**.
2. Give your repository a clear, descriptive name using hyphens (e.g., `chassis-mounting-bracket` or `electronics-enclosure-box`).
3. Set the repository to **Public** so students, teachers, and makers can view and download the files.
4. Check the box to **Add a README file**.
5. Click **Create repository**.

---

## Step 2: Add the Open-Source License
To keep our club's shared designs open and accessible:
1. In your new repository, click **Add file > Create new file**.
2. Name the file **`LICENSE`** (exact spelling, no extension).
3. On the right, click **Choose a license template** and pick the **MIT License**.
4. Click **Commit changes**.

---

## Step 3: Tag It for the Portal (`project`)
To make sure your new project automatically appears as a card on the main portal grid:
1. Look at the right-hand sidebar of your repository homepage under **About**.
2. Click the gear icon or tags area.
3. Add the topic tag **`project`** (along with specific descriptive tags like `3d-print`, `laser-cut`, `cad`, or `mechanical`).
4. Click **Save changes**.

---

## Step 4: Organize Your Project Files
Keep your file structure clean so anyone can easily find what they need to fabricate or build your design:
* **CAD / Source Files:** Store native files (like Fusion 360 exports, SolidWorks, or FreeCAD files) in a folder named `/cad/` or `/source/`.
* **Fabrication Files:** Put ready-to-print or ready-to-cut files in clear folders (e.g., `/stl/` for 3D prints or `/dxf/` for laser cutting).
* **Images / Renders:** Include a photo or render of the finished build in the root directory so it looks great on documentation pages.

---

## Step 5: Document Your Project in the README
Every project repository needs a quick explanation in its main `README.md` file:
* **Overview:** What is this part, and what project does it belong to?
* **Fabrication Settings:** For 3D prints, note recommended material (e.g., PETG or TPU), infill percentage, and layer height. For laser cutting, note material thickness (e.g., 1/4" acrylic or plywood).
* **Assembly Instructions:** Any special hardware, screws, or steps required to put it together.
