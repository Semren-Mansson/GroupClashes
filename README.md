# Group Clashes

A Navisworks Manage plugin for rule-based clash results grouping.

## Getting Started

This plugin will help you to group clash results in a given Navisworks clash test. For now, you can group clashes by:
* ~~Nearest level~~
* ~~Nearest grid intersection~~
* Current selection
* Element belonging to a model
* Status, approval or assignment

Open the Group Clashes window by clicking on the Group Clashes button (Group Clashes tab).
Select a clash test. The two selections involved in the clash test are displayed below.
Select one or two clash rules. Since Navisworks Manage does not support subgroup for clashes, the group name will include the result of the two rules.
Click on Group.
For a full description of each grouping rule, visit [bim42.com](http://bim42.com/2016/10/group-clashes/).

### Prerequisities

This application is originally developed with Visual Studio 2015 and compiled with Visual Studio 2019.
To run this plugin, you will need Navisworks Manage:

|Supported Navisworks Manage|Version|
|-|-|
|2015|v12|
|2016|v13|
|2017|v14|
|2018|v15|
|2019|v16|
|2020|v17|
|**2021**|**v18**|

**Build steps**:
1. Launch Visual Studio 2019 in Admin mode.
2. Reference `Autodesk.Navisworks.Api.dll` and `Autodesk.Navisworks.Clash.dll` from `C:\Program Files\Autodesk\Navisworks Manage 20XX\` if they are missing. Don't forget to set the **Copy Local** to `False`.
3. Compile the solution in **Debug** mode and wait until `PostBuild.ps1` script copies the resulting dll in the Navisworks Manage Plugin folder.

Before modifying anything, I advise you to check the Navisworks Manage SDK on the [Autodesk Developer Network](http://usa.autodesk.com/adsk/servlet/index?id=15024694&siteID=123112).

## Built With

* [Visual Studio 2015](https://www.visualstudio.com/vs/community/) - My tool of choice

## Contributing

Please feel free to submit pull request in any manner you want.

## Authors

* **Simon Moreau** - *Initial work* - [BIM 42](https://bim42.com)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Thanks to the team behind the Navisworks Manage SDK for providing me the idea with the tools to implementing it.

