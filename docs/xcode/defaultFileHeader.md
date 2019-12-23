##  Changing Xcode File Header
#### Steps
1. Create plist file
    * Filename
      * IDETemplateMacros.plist
    * Locations (in seacrch order)
      * <ProjectName>.xcodeproj/xcuserdata/[username].xcuserdatad/IDETemplateMacros.plist.
      * <ProjectName>.xcodeproj/xcshareddata/IDETemplateMacros.plist
      * <WorkspaceName>.xcworkspace/xcuserdata/[username].xcuserdatad/IDETemplateMacros.plist.
      * <WorkspaceName>.xcworkspace/xcshareddata/IDETemplateMacros.plist.
      * ~/Library/Developer/Xcode/UserData/IDETemplateMacros.plist.
1. Create the text macro
    * Text macro must be surrounded by three underscores on each side
    * Currently, "//" is automatically added to the beginning of the text macro when implemented
    * Leave the first line empty to accomodate the initial "//" 
1. Add new plist entry
    * Name the entry FILEHEADER
    * Set the type to String
    * Copy and Paste the text macro into the value field
#### Common macro keys
* COPYRIGHT
* DATE
* FILEBASENAME
* FILENAME
* FULLUSERNAME
* ORGANIZATIONNAME
* PACKAGENAME
* PROJECTNAME
* TIME
* USERNAME
* YEAR
#### Example Text Macro
```
<leave this line blank>
  /*
___PACKAGENAME___
___FILENAME___
Created by ___FULLUSERNAME___, on ___DATE___
___COPYRIGHT___
*/
```
or
```
<leave this line blank>
// ___PACKAGENAME___
// ___FILENAME___
// Created by ___FULLUSERNAME___, on ___DATE___
// ___COPYRIGHT___
```
#### References
- [Apple](https://help.apple.com/xcode/mac/9.0/index.html)
  - [Customize Text Macros](https://help.apple.com/xcode/mac/9.0/index.html?localePath=en.lproj#/dev91a7a31fc)
  - [Text Macros Reference](https://help.apple.com/xcode/mac/9.0/index.html?localePath=en.lproj#/dev7fe737ce0)
  - [Text Macro Format](https://help.apple.com/xcode/mac/9.0/index.html?localePath=en.lproj#/devc8a500cb9)
- [Use Your Loaf](https://useyourloaf.com/blog/changing-xcode-header-comment/)
- [Medium](https://medium.com/@silmy/how-to-easily-change-your-file-header-text-in-xcode-347fa77d76f4)
- [Ole Begemann](https://oleb.net/blog/2017/07/xcode-9-text-macros/)
