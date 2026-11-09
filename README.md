### Game Automation Pipeline

**Game Automation Pipeline** eliminates the repetitive manual tasks involved in preparing and running multiple games. It is designed to scan a source directory (`data/`), identify game code, organize the files into a dedicated structure, generate metadata, and automatically compile and execute the games.

#### Features

- **Automated Discovery:** Scans the `data/` directory to automatically identify game files and directories.
- **Smart Organization:** Copies discovered games into a structured `games/` directory, automatically stripping the `game` suffix from filenames for cleaner naming conventions.
- **Metadata Generation:** Creates a structured JSON file containing information about all discovered games, serving as a manifest for the available content.
- **Automated Compilation:** Automatically compiles the organized game code.
- **Automated Execution:** Runs the compiled games immediately after the build process is complete.
- **Zero Configuration:** Works out-of-the-box with the standard `data/` directory structure.

The script follows a linear pipeline to process your game files:

1.  **Scan:** Reads the `data/` source directory.
2.  **Organize:** Creates a `games/` directory and copies files over, removing the `game` suffix from the filenames.
3.  **Manifest:** Generates a JSON file detailing the discovered games.
4.  **Compile:** Compiles the organized game code.
5.  **Execute:** Runs the compiled games.
