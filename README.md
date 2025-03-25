# Rebrickable Community Build Together Repository

This repository is used for creating and sharing LEGO build projects collaboratively on the Rebrickable forum. It is a **community-driven** initiative and is **not affiliated** with the official Rebrickable team in any way. For more information head to the Rebrickable forum and go to the [topic](https://forum.rebrickable.com/t/building-together/58702) explaining the rules.

## How to Commit and Push .ldr Files

Follow these simple steps to save and upload your `.ldr` file changes to the repository.

### 1. Install Git
To commit and push changes, you need to install Git first. Follow these steps:

#### For Windows:
1. Download Git from the official website: [https://git-scm.com/download/win](https://git-scm.com/download/win)
2. Run the installer and follow the installation steps (you can leave the options at their defaults).
3. After installation, open the **Git Bash** (or **Command Prompt**) and run:
   ```sh
   git --version
   ```
   This will show the installed version of Git if it was successfully installed.

#### For macOS:
1. Open **Terminal** and run:
   ```sh
   git --version
   ```
2. If Git is not installed, you'll be prompted to install it via **Xcode Command Line Tools**. Follow the prompts to install Git.

#### For Linux:
1. Open your **Terminal** and run:
   ```sh
   sudo apt update
   sudo apt install git
   ```
2. After installation, check the version with:
   ```sh
   git --version
   ```

### 2. Clone the Repository
Before you can make changes, you need to clone the repository to your local machine. Run the following command in **Git Bash** or **Terminal**:
```sh
git clone https://github.com/thomkok18/Rebrickable-Build-Together.git
```
This will create a copy of the repository on your computer.

### 3. Open the Git Bash
- If you are using Windows, open the **Git Bash**.
- If you are using macOS or Linux, open the **Terminal**.

### 4. Navigate to the Repository Folder
Type the following command and press **Enter**:
```sh
cd path/to/repository
```
Replace `path/to/repository` with the actual folder where you downloaded this repository and point it to the repository itself.

### 5. Check for Changes
Run:
```sh
git status
```
This will show the modified files.

### 6. Add Your Changes
To add all new files you made, run:
```sh
git add .
```

### 7. Commit Your Changes
Run the following command when you are done with your step:
```sh
git commit -m "Updated .ldr files"
```
You can change `"Updated .ldr files"` to a short message describing what was changed.

### 8. Push Your Changes
Upload the changes by running:
```sh
git push
```
If asked for login details, enter your GitHub username and password (or use an access token if required).

### Done!
Your files are now saved and uploaded to the repository.
