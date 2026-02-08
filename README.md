![ranma1](https://i.ibb.co/R4G0HzzL/ranma1.png)
![ranma2](https://i.ibb.co/k2vk7340/ranma2.png)
![ranma3](https://i.ibb.co/0pf6GSBr/ranma3.png)
![ranma4](https://i.ibb.co/Cs4Qnmhb/ranma4.png)
![ranma5](https://i.ibb.co/qLnCXFYq/ranma5.png)
![ranma6](https://i.ibb.co/6cVkXZWd/ranma6.png)
![ranma7](https://i.ibb.co/zWhd8RLM/ranma7.png)

# OTHER LANGUAGES
[Português](README.pt.md)

# HOW TO INSTALL THE THEME

## NECESSARY EXTENSIONS
To install themes in Gnome, you need some extensions that can be downloaded here: https://extensions.gnome.org/
- [Install Browser Extension](https://extensions.gnome.org/) - Allows you to install extensions via your browser.
- [User Themes](https://extensions.gnome.org/extension/19/user-themes/) - Load shell themes from user directory.
- Gnome Tweaks - You need this tool to manage themes. Install it through your distro's store or type the following in the terminal: ```sudo apt install gnome-tweaks```
- [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) - Allows you to place a background image on the lock screen.
- [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/) - Allows you to customize the dock.

## INSTALLING THE THEME
Install all the necessary extensions above.

Go to the "home" folder and press Ctrl + H to view hidden folders (or check the option to view hidden folders), and create a folder named **.themes** and **.icons**.

Extract the theme .zip file, copy the extracted folder, and paste it into .themes.

Open Gnome Tweaks, go to Appearance, and under “Applications” and “Shell” select **RanmaTheme**, then press Alt + F2 to restart the shell and the theme will be installed.

### HOW TO CHANGE THE DOCK COLOR
To change the color of the dock, open Extensions, click on “Settings” in “Dash to Dock,” go to “Appearance,” and in “Customize the dash color” enter the color #0fc0fc.

### HOW TO INSTALL WALLPAPERS
Install the [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) extension from the Gnome Extensions website. Press the super key and open the Extensions application. In Lock Screen Background, click Settings, select the wallpaper, and you're done.
The images to be used as wallpapers are in the “images” folder.

### HOW TO PLACE THE LOGO ON THE TERMINAL (FAST FETCH)
First, generate a configuration file using the command below in the terminal:
<br>
```fastfetch --gen-config```
<br>
(The config.jsonc file will be generated in the location /.config/fastfetch/config.jsonc)

Take an image and convert it to ASCII. You can use the website below for this. Then copy and paste it into Notepad and save it as “logo.txt.”
https://www.asciiart.eu/image-to-ascii

Edit the “logo” class in the “config.jsonc” file located at “/home/user/.config/fastfetch/config.jsonc,” entering the path to your logo.txt file. An example of how it should look is shown below:
```
{
  "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/dev/doc/json_schema.json",
    "logo": {
        "type": "file",
        "source": "/home/user/.config/fastfetch/logo.txt",
        "height": 15,
        "width": 30,
        "padding": {
            "top": 5,
            "left": 3
        }
    },
```

To open the terminal with the logo without having to type the fastfetch command, paste the command below into the “.bashrc” file in the “/home/user” path.
<br>
```fastfetch --logo /home/user/.config/fastfetch/logo.txt```

### HOW TO MAKE NOTIFICATIONS APPEAR FOR TESTING
Type the command below into the terminal and a fake notification will appear.
<br>
```notify-send "Title" "Test message"```

### HOW TO TAKE A SCREENSHOT OF ANY AREA (SUCH AS THE LOCKSCREEN AND SCREENSHOT SCREEN)
Type the command below into the terminal, and a screenshot will be taken within 10 seconds:
<br>
```gnome-screenshot -d 10```

### THEME COLORS
blue = #0fc0fc
<br>
pink = #fe4eda
<br>
yellow = #F5C211
<br>
green = #32cd32
<br>
red = #e62020 or #d40000
<br>
purple = #663399
