# MobileNavigationMenuComponent
A beautiful mobile navigation component for your Canvas Apps!
![ezgif-2-8e4b09c310](https://user-images.githubusercontent.com/86930618/174883461-8e08a363-7305-451f-a0e4-b04b59b12dc2.gif)


Beautiful navigation for your mobile Canvas Apps!

This menu consists of a mixture of code and out-of-the-box controls. 

To install the component, please follow these steps:

**- Please download it from this repo,**
**- Import it into your application **
- ![image](https://user-images.githubusercontent.com/86930618/174883894-b4bc2004-7848-4085-bd4d-3e3890d86652.png)


**- Change the MenuItems property to**

Table(
    {
        //this is the name of the screen
MenuItem: "Home",
        // this is the screen you will navigate to when you select this item
        MenuScreenNavigate: Home,
        // this is the colour of the background circle 
        BackgroundHex: "#dc582a",
        // optional value
        HTMLFill: "rgb(249, 81, 19, 0.2)",
        //if you are not comfortable with SVG's, you can use standard icons instead!  - just make sure you change the icon property of MenuIcon to ThisItem.StandardIcon
        StandardIcon: Icon.Home
    },
    {
        MenuItem: "Add new",
        MenuScreenNavigate: 'Add new',
        BackgroundHex: "#038761",
        HTMLFill: "rgb(85, 226, 131, 0.1)",
        StandardIcon: Icon.Add
    },
    {
        MenuItem: "Profile",
        MenuScreenNavigate: Profile,
        BackgroundHex: "#007FAA",
        HTMLFill: "rgb(17, 130, 253, 0.2)",
        StandardIcon: Icon.AddUser
    },
    {
        MenuItem: "Settings",
        MenuScreenNavigate: Settings,
        BackgroundHex: "#d3273e",
        HTMLFill: "rgb(245, 111, 174, 0.2)",
        StandardIcon: Icon.Settings
    }
)

**- Create screens in your app to match the MenuItem name.**
**- Change the StandardIcon to whatever out-of-the-box icon you'd like to use.**
**- If you would like to use the animated SVG's, please note there are some additional steps to be carried out. The SVG code is contained within the MenuLogo image control - as we are changing the colour of the SVG's dynamically based on the active screen, we are using the Switch() function. I have recently blogged step by step how to achieve this -** https://www.kristinekolodziejski.com/blog/building-a-beautiful-power-apps-mobile-navigation-menu-svgs-part-3


The component has four main properties:

![image](https://user-images.githubusercontent.com/86930618/174884603-64b31cd8-a59e-4b26-a11d-7ce8cccee3e3.png)

- **MenuItems** is the table of menu items pasted above,
- **Animation** - this is applicable to SVG's in this component only - if you want the active screen SVG to float, please set that to true, otherwise set it to fault.
- **IconSVGorStandard** - if you want your icons to be SVG's, set that to true. If you are not comfortable SVG's and want to use out-of-the-box icons instead, please set that to false.

I have added as many comments to the component itself to help you understand how it's built! 

However, if you have any questions, issues or comments - as always, please reach out to me on my socials and I'll be more than happy to help 😊

Kristine

