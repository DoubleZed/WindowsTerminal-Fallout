# Fallout Theme for the Windows Terminal

![WindowsTerminal-Fallout](https://github.com/DoubleZed/WindowsTerminal-Fallout/blob/master/animation.gif)

## Installation
You can download the Windows Terminal here: https://github.com/microsoft/terminal or from the Windows Store.

You will need to download a terminal background image if you want the background to not be just a solid color. Here are a couple options:

![WindowsTerminal-Fallout](https://github.com/DoubleZed/WindowsTerminal-Fallout/blob/master/background.png)
![WindowsTerminal-Fallout](https://github.com/DoubleZed/WindowsTerminal-Fallout/blob/master/background_purple.png)

Navigate to %localappdata%\Packages\Microsoft.WindowsTerminal_8wekyb3d8bbwe\RoamingState and add the background image. For the below code to work you have to name it background.png

Now you can open the terminal and click settings under the menu arrow next to the open tab. Then click on "Open JSON file" bottom left of the terminal settings window.

The settings.json will open. Under the right GUID (E.g. PowerShell, Ubuntu, CMD), add the following lines:                

    {
        "guid": "{xxxxxxx-xxxx-xxxx-xxxx-xxxxxxx}", //Replace this with yours
        "hidden": false,
        "name": "PowerShell", //Replace this with your tab
        "source": "Windows.Terminal.PowershellCore", //This one too
        "experimental.retroTerminalEffect": true,
        "colorScheme": "Fallout",
        "backgroundImage" : "ms-appdata:///roaming/background.png", //or whatever your background file is named
        "backgroundImageOpacity" : 0.5
    }

and under "schemes" below add the following:

    {
        "name" : "Fallout",
        "cursorColor": "#FFFFFF",
        "background" : "#0C0C0C",
        "foreground" : "#26E476",
        "selectionBackground": "#0C0C0C",
        "black" : "#0C0C0C",
        "blue" : "#26E476",
        "cyan" : "#26E476",
        "green" : "#022000",
        "purple" : "#26E476",
        "red" : "#26E476",
        "white" : "#26E476",
        "yellow" : "#26E476",
        "brightBlack" : "#767676",
        "brightBlue" : "#26E476",
        "brightCyan" : "#26E476",
        "brightGreen" : "#26E476",
        "brightPurple" : "#26E476",
        "brightRed" : "#26E476",
        "brightWhite" : "#26E476",
        "brightYellow" : "#26E476"
    }
        
You should be good to go!
