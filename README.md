# eclipse.ini
- Replaces all memory limits with 1024 and add "-Xverify:none" and "-XX:+UseSerialGC" to Eclipse.app/Contents/MacOS/eclipse.ini.

# Per Eclipse Installation Workspace
1. `mkdir eclipse/workspace`
1. `mv eclipse ~/opt/eclipse-android`
1. Launch Eclipse.
1. At prompt, set workspace to "../../../workspace" and check always.

# Plugins
- ADT: https://dl-ssl.google.com/android/eclipse/
- FindBugs: http://findbugs.cs.umd.edu/eclipse

# Preferences

#### General
- Check General -> Editors -> Text Editors -> Insert spaces for tabs
- Check General -> Editors -> Text Editors -> Show print margin
- Check General -> Editors -> Text Editors -> Show whitespace characters
- Uncheck General -> Editors -> Text Editors -> configure visibility -> Space -> Leading
- Uncheck General -> Editors -> Text Editors -> configure visibility -> Space -> Enclosed

- Check Startup and Shutdown -> Refresh workspace on startup
- Uncheck Startup and Shutdown -> Confirm exit when closing last window

- Uncheck Workspace -> Refresh on access

- Check Run/Debug -> Launching -> Always launch the previously launched application

#### Android
- Set Verbose Android -> Build -> Build output
- Set Android -> DDMS -> Base local debugger port
- Uncheck Android -> LogCat -> Monitor logcat for message from applications in workspace
- Set Android -> NDK -> NDK Location

### C/C++
- Set C/C++ -> Build -> Environment -> Add...
  - NDK_CCACHE /Users/stephen/opt/homebrew/bin/ccache
  - USE_CCACHE 1
- Uncheck C/C++ -> Indexer -> Enable indexer

#### Java
- Set to m Java -> Code Style -> Conventions for variable names -> Fields -> Prefix list

- Click Java -> Code Style -> Formatter -> Import... and select ~/Workspace/aosp/development/ide/eclipse/android-formatting.xml
- Click Java -> Code Style -> Formatter -> Organize Imports -> Import... and select ~/Workspace/aosp/development/ide/eclipse/android.importorder

- Set Warning Java -> Compiler -> Errors/Warnings -> Code style -> Parameter assignment

- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Possible accidental boolean assignment
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Empty statement
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Unused object allocation
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Potential resource leak
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Missing synchronized modifier on inherited method
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Class overrides 'equals()' but not 'hashCode()'

- Set Warning Java -> Compiler -> Errors/Warnings -> Name shadowing and conflicts -> Field declaration hides another field or variable
- Set Warning Java -> Compiler -> Errors/Warnings -> Name shadowing and conflicts -> Local variable declaration hides another field or variable

- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Value of parameter is not used
- Unset Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Ignore in overriding and implementing methods
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unused type parameter
- Unset Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Ignore unused paramters documented with '@param' tag
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unnecessary 'else' statement
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unnecessary cast or 'instanceof' operation
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unnecessary declaration of thrown exception
- Unset Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Ignore in override and implementing methods
- Unset Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Ignore exceptions documented with '@throws' or '@exception' tags
- Unset Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Ignore 'Exception' and 'Throwable'

- Set Warning Java -> Compiler -> Errors/Warnings -> Annotations -> Missing '@Override' annotation

- Set Warning Java -> Compiler -> Errors/Warnings -> Null analysis -> Potential null pointer access
- Set Warning Java -> Compiler -> Errors/Warnings -> Null analysis -> Redundant null check

#### Team
- Uncheck Team -> Git -> Refresh resources when index changes
- Uncheck Team -> Git -> Refresh only when workbench is active

- Uncheck Team -> Git -> Projects -> Automatically share projects located in a Git repository
- Uncheck Team -> Git -> Projects -> Track each branch's imported projects and restore on checkout
- Uncheck Team -> Git -> Projects -> Automatically ignore derived resources by adding them to .gitignore

#### XML
- Check XML -> XML Files -> Editor -> Indent using spaces
- Set to 4 Check XML -> XML Files -> Editor -> Indentation size
- Set to 80 Check XML -> XML Files -> Editor -> Line width

# Project Explorer Window Settings
- Set Project Explorer -> Top Level Elements -> Working sets

# Problems Window Settings
- Uncheck Configure Contents... -> Use item limits

# Make a Copy of Eclipse
