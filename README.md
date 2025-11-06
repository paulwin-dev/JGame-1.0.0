<img width="593" height="153" alt="image" src="https://github.com/user-attachments/assets/220c30f0-2e0d-4470-bbde-c6e098b10319" />

A lightweight java game engine created using the Java AWT library.

# Getting Started
To get started, clone the repository to your local machine. Once that's done, you can run JGameStudio/JGameHub/JGameHub.java to start the hub application where you can manage your projects and JGame installations.

### Studio
Using JGame Studio, you can develop your projects. To run code in your game, you have two options: <p>
1. Create a class that inherits from the `WritableScript` class and link it to a Script object in the editor (recommended)
2. Run and manage code from the Main.java file that is auto-generated for every project.

### Running Games
In order to play your games, run the Main.java file with your Java installation. No dependencies are required as the engine code itself is included with every project, making them portable and easy to run.

### Creating Games Without JGame Studio
It is entirely possible to create games without the use of JGame Studio as the engine itself is completely separate from the editor, however it comes with a few drawbacks. Not using Studio to manage and clone your JGame installation to projects means that you need to manually copy the JGame package to your project folder every time you start a new project. Even though Studio is still very new and may be a bit buggy at times, we definitely recommend using it to manage your projects and installations as it makes creating games much easier.

# Other Notes & Warnings
What becomes obvious by just looking at the file structure is that this is not how a traditional java project would be structured. While I would love to have a good explanation for this, the truth is that I started this project with almost no knowledge about Java and have kept the file structure since.
Not to worry: the file structure **will** be refacted to match java conventions.

Another glaring issue with JGame is the fact that it's quite slow. This is due to the reliance on the AWT library for rendering. As AWT itself is not intended for per-frame rendering calls, this slows down the engine significantly. A port to libgdx is likely in the future,
however this is a big change and will likely take quite a lot of time to do.
