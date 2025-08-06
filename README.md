# Analogue OS Menu for ES-DE

This is a tranlation of the Analogue OS menu interface (originally designed & created by [Analogue](https://www.analogue.co/os)) for ES-DE.

My work focused on tranlating the layout so that it could be buildable in the theme engine for ES-DE.  Please refer to the `Changes Made` section below for additional details. 

The original version of the UI can be found as part of the OS available on the Analogue Pocket and other devices made by [Analogue](https://www.analogue.co/)

## Changes Made

- Referenced [Analogue OS](https://www.analogue.co/os) to approximate the components that would be used build a theme compatible with ES-DE.
- Added the helpsystem from ES-DE and created a layout that tries to evoke the original helpsystem design (sadly it can't be a 1:1 translation due to differences in the theme engines)
- Added icons and badges specific to ES-DE functionality
- Created a full set of custom pixel art icons for the ES-DE helpsystem

## **Preview**

![System View](https://github.com/anthonycaccese/analogue-os-menu-es-de/assets/1454947/ad46707a-eba9-4986-858d-166b05622372)

## **Configuration Options**

The theme has a simple set of options that can be changed directly from the UI Settings menu of ES-DE 

### **Variants:**

- `Theme Variant` - sets the layout used for the gamelist view.
   - `List` - The default variant. A list view that matches the same style as system view.
   - `Carousel` - An attempt to translate the list view with images that exists in Analogue OS. See the reference image [here](https://images.analogue.co/os-library-image.b7bbf0123dfe40e9d30f9dde054b9d06.png?auto=format&w=1000&q=100&s=3122733796f9330200cf8c0857ac88e0).
   - `Grid` - An attempt to translate the grid view that exists in Analogue OS. See the reference image [here](https://images.analogue.co/os-library-grid.e720ee19f4aa5a23177e725a28532383.png?auto=format&w=1000&q=100&s=78951d124f8051d55eb18b267552e73c).
 
| List | Carousel | Grid |
|----|----|----|
![List](https://github.com/anthonycaccese/analogue-os-menu-es-de/assets/1454947/ca512e3b-22fd-4b56-b709-4dcd6ae6ce47) | ![Carousel](https://github.com/anthonycaccese/analogue-os-menu-es-de/assets/1454947/e0d561fa-e775-485f-872e-d316602ff004) | ![Grid](https://github.com/anthonycaccese/analogue-os-menu-es-de/assets/1454947/8ef43932-031b-4d0b-9d8f-d24a51eb52be) |

### **Color Schemes:**

- `Theme Color Scheme` - sets the color scheme that is used for the overall theme on all views.
   - `Dark` - The default color scheme. 
   - `Light` - A `light` version of the above color scheme.
 
| Dark | Light |
|----|----|
| ![Gamelist View - Dark](https://github.com/anthonycaccese/analogue-os-menu-es-de/assets/1454947/3883d56c-99ce-4eb3-be88-c2ec2926c5da) | ![Gamelist View - Light](https://github.com/anthonycaccese/analogue-os-menu-es-de/assets/1454947/dda70f3b-c91a-469f-ae6a-3b97d155b025) |

### **Font Sizes:**

- `Theme Font Size` - sets the size that text will render at. This can be helpful when using the theme on small screens.
   - Supported Font Sizes:
   - `Large` - Good for small handheld screens under 4 inches in size.

### **Aspect Ratios:**

- `Theme Aspect Ratio` - sets the aspect ratio to match your display. This should happen automatically but can also be set manually if needed.
   - Supported Aspect Ratios:
   - `4:3`
   - `16:9`
   - `16:10`
   - `3:2`
   - `19.5:9`
   - `1:1`
 
## Additional Notes

### **Creating your own color scheme:**

1) In the resources folder you will find a template file called [colors-custom.xml](https://github.com/anthonycaccese/analogue-os-menu-es-de/blob/main/resources/colors-custom.xml)

2) Make a folder named `theme-customizations` and place a copy of the `colors-custom.xml` file inside that folder.  The folder structure should look like this when you are done:
   ```
   /ES-DE/themes/minui-menu-es-de/theme-customizations/colors-custom.xml
   ```
   *Note: This structure should allow you to continue to get updates for the theme from the theme downloader while also retaining your customizations.*

3) Edit the properites in `colors-custom.xml` to create your custom color scheme:
   - Here is a definition of each property:
      - `backgroundColor` - Sets the color to be used for the background on all screens.
      - `listSelectedColor` - Sets the text color of the selected item on the List Variant.
      - `listSelectedBackgroundColor` - Sets the highlight color for the selected item on the List Variant.
      - `listUnselectedColor` - Sets the text color for unselected items on the List Variant.
      - `gridGameName` - Sets the text color of the game name on the Grid Variant.
      - `gridTextColor` - Sets the text color of the selected item when it does not have an image to display on the Grid & Carousel Variants.
      - `gridTextBackgroundColor` - Sets the background color of the selected item when it does not have an image to display on the Grid & Carousel Variants.
      - `carouselGameName` - Sets the text color of the game name on the Carousel Variant.
      - `carouselGameSystemName` - Sets the text color the system name on the Carousel Variant.
      - `helpIconColor` - Sets the icon color for items in the included help system
      - `helpTextColor` - Sets the text color for items in the included help system
    
4) Set the `Theme Color Scheme` in ES-DE's UI Settings menu to `Custom` and you should see your custom color scheme display.  If you see an error check that the paths discussed above are correct and then check that the values you added for each property are correct and well formatted.

If you make a custom color scheme and are comfortable with sharing I would love to check it out 😊
- Please feel free to create an issue in this repo called `Custom Color Scheme: [Name of your Color Scheme]`
- Include the values you used for the properties above (xml is preferred), the background image and fonts you added (if any) and a screenshot of what it looks like.

## **Credits:**

- The original UI was created & designed by [Analogue](https://www.analogue.co/)
- The included font is called "GamePocket-font" and was created by [mumchristmas](https://github.com/mumchristmas/GamePocket-font)
