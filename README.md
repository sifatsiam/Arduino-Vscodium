# Custom Minimal Arduino IDE Alternative in VS Code or Vs Codium

## Overview

This document outlines the setup and usage of a Minimal Arduino IDE alternative using Visual Studio Code/VSCodium. This setup is lightweight and allows for an efficient development experience with Arduino-compatible projects.

## Requirements

- [Visual Studio Code](https://code.visualstudio.com/)
- [VSCodium](https://vscodium.com/)
- [Arduino IDE](https://www.arduino.cc/en/software) (for installation of boards and libraries)
- [Arduino Extension for VS Code](https://marketplace.visualstudio.com/items?itemName=ms-arduino.arduino)
- [Powershell](https://en.wikipedia.org/wiki/PowerShell)
- A fully functional computer or your favourite pc

## Installation Steps

1. **Install Visual Studio Code or VSCodium**:
   - Download and install from the [official website](https://code.visualstudio.com/).
   -  If you are on a Mac and have Homebrew installed try
     
   ``` brew install --cask vscodium ```

      
2. **Install the Arduino Extension**:
   - Open VS Code.
   - Go to the Extensions view by clicking on the Extensions icon in the Activity Bar or pressing `Ctrl+Shift+X`.
   - Search for "Arduino" and install the **Arduino Extension for VS Code**.

3. **Set Up Arduino Environment**:
   - Open the Command Palette (`Ctrl+Shift+P`) and type `Arduino: Initialize`.
   - Select your board type and configure the settings as needed.

4. **Include Libraries**:
   - Create a `lib.txt` or Open `lib.txt` file in your project folder or Download this from main repo. This file should contain a list of all official Arduino-compatible libraries you plan to use. For example:
     
     ```
     ﻿107-Arduino-24LCxx
     107-Arduino-BoostUnits
     Wire
     Adafruit_Sensor
     LiquidCrystal
     Adafruit AD569x Library
     ```

## Usage

1. **Creating a New Project**:
   - To create a new Arduino project, go to `File > New File` and save it with a `.ino` extension.

2. **Writing Code**:
   - Write your Arduino sketch as you would in the traditional IDE. The Arduino extension provides IntelliSense and code completion.

3. **Including Libraries**:
   - To include libraries from your `lib.txt`, use the following syntax in your sketch:
     ```cpp
     #include <Wire.h>
     #include <Adafruit_MCP4725.h>

     ```

4. **Compiling and Uploading**:
   - Use the Command Palette (`Ctrl+Shift+P`) and select `Arduino: Verify` to compile your code.
   - Select `Arduino: Upload` to upload the compiled code to your board.

## Additional Features

- **Integrated Terminal**: Use the integrated terminal in VS Code for command-line operations.
- **Version Control**: Leverage Git integration for version control and collaboration.
- **Customization**: Customize your workspace with themes and settings to fit your workflow.

## Conclusion

This Minimal Arduino IDE alternative provides a lightweight yet powerful environment for Arduino development and it looks amazing. With VS Code's extensive features and the Arduino extension, you can streamline your coding experience while maintaining the functionality you need. 

**ProTip:** You can download GNU BinUtilz_win32 for more **Control** in your windows based operating system.

## Resources

- [Arduino Documentation](https://www.arduino.cc/en/Reference/HomePage)
- [Visual Studio Code Documentation](https://code.visualstudio.com/docs)
- [Arduino Extension for VS Code GitHub](https://github.com/microsoft/vscode-arduino)
- [GNU BinUtilz_win32](https://github.com/SadBIOS/Arduino-Vscodium/releases/tag/Gen2_utilz)


