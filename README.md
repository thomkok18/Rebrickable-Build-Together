# Rebrickable Community Build Together Repository

This repository is used for creating and sharing LEGO build projects collaboratively on the Rebrickable forum. It is a **community-driven** initiative and is **not affiliated** with the official Rebrickable team in any way. For more information head to the Rebrickable forum and go to the [topic](https://forum.rebrickable.com/t/building-together-v2/166766) explaining the rules.

## Editing the files

To open the .ldr file you need special software that allows you to change the file. The current recommended software that allows you to add steps into the file is called Bricklink Studio.
- Download te following software: [Bricklink Studio](https://www.bricklink.com/v3/studio/download.page).
- Open the .ldr file and make your edits. Don't forget to save afterwards by using Export as LDraw and overwrite the current .ldr file.

### Rules

1. Change **10 parts** at max per turn
   - Edit the color of a piece
   - Add a new piece to the build
   - Remove a brick from the build (Note: You can only remove **5 parts** per turn)
2. Always add a new Step for your changes
   - Before editing anything, add a new Step in Studio and place your new parts in it.
3. If you made the last change, you can only make a change again, if:
   - Someone else made a change
   - 5 days of inactivity passed
4. If you can, please upload a render of the model, put this inside the `./Images` subfolder.

### Naming schemes:

LDraw files: `[PROJECT NAME]`
- `[PROJECT NAME]`: The name of the project, as found in the folder (e.g. Build_Together)

Image Files: `[PROJECT NAME]_v[NUMBER]`
- `[PROJECT NAME]`: The name of the project, as found in the folder (e.g. Build_Together)
- `[NUMBER]`: The number of the step the render is from

Commit Messages: `[PROJECT NAME] Step [NUMBER]`
- `[PROJECT NAME]`: The name of the project, as found in the folder (e.g. Build_Together)
- `[NUMBER]`: The number of the step added

## Commit the changes
There are two ways to save your changes to GitHub. Try one or the other based on your preference.

### Changing the file on GitHub
Now, the file is changed locally, but not on GitHub. This is the most complicated step in this process. Just follow these substeps:

- Locate the file in your File Manager (Explorer, Finder, Nautilus, etc.).
- Right Click > Open With…
- Select a text editor from that list (e.g. Text Editor, Notepad++, TextEdit, etc.).
- Once the file is open, hit Ctrl + A to select everything and then Ctrl + C to copy everything.
- Head back to the file you downloaded earlier from the repository.
- Click the pencil icon to edit that file.
- Once in editing mode, hit Ctrl + A and then Ctrl + V to replace everything with your updated version.
- Click “Commit changes…” and set Build Together Step [XY] as the commit message ([xy] is the current step number).
- You can leave the Extended description empty. Let the commit email on the default option.
- Leave the radio select on “Commit directly to the main branch”.
- Click “Commit changes”.

### Changing the file locally
To save your changes locally on your computer you need to have Git installed.

#### 1. Open Git Bash
- If you are using Windows, open **Git Bash**.
- If you are using macOS or Linux, open the **Terminal**.

#### 2. Navigate to the Repository Folder
Type the following command and press **Enter**:
```sh
cd path/to/repository/Rebrickable-Build-Together
```
Replace `path/to/repository/Rebrickable-Build-Together` with the actual folder where you downloaded this repository and point it to the repository (Rebrickable-Build-Together folder) itself.

#### 3. Retrieve the current GitHub changes
Run:
```sh
git pull
```

#### 4. Check for Changes
Run:
```sh
git status
```
This will show the modified files.

#### 5. Add Your Changes
To add all new files you made, run:
```sh
git add .
```

#### 6. Commit Your Changes
Run the following command when you are done with your step:
```sh
git commit -m "[PROJECT NAME] Step [NUMBER]"
```
Look at the [Naming schemes](#naming-schemes)

#### 7. Push Your Changes
Upload the changes by running:
```sh
git push
```
If asked for login details, enter your GitHub username and password.

#### 8. Done!
Your files are now saved and uploaded to the repository. You will find your commit located at the top of the repository as shown in the image below. Go to the most recent commit by clicking on (for example) 0a2c06, or click on the amount of commits to look through all commits made. Now you are able to share the link of the commit in your post.

![Github commits](https://github.com/user-attachments/assets/d6b529d5-7e04-4369-9cfb-23e21d67599e)

## First Setup

Follow these simple steps to save and upload your `.ldr` file changes to the repository.

### 1. Install Git
To commit and push changes to this repository, you need to install Git first. Follow these steps:

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

## FAQ

1. When I try to use the ``git push`` command I get the following:

![GitHub merge conflict](https://github.com/user-attachments/assets/758f4c79-621d-45f5-a15b-dfd18dc1d132)
What do I need to do?

This happens when somebody else has made changes in the repository on GitHub and your version on your computer is not up-to-date. You have to do the following to update your version:
* Run ``git pull`` to receive the updates.
* If you see Merge branch press Esc button and type after that :wq to use the standard merge commit message. Press enter to exit when done.
* Now you are able to try ``git push`` again.
