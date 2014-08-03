# eclipse.ini
- Replaces all memory limits with 1024 and add "-Xverify:none" and "-XX:+UseSerialGC" to Eclipse.app/Contents/MacOS/eclipse.ini.

# Per Eclipse Installation Workspace
1. `mkdir eclipse/workspace`
1. `mv eclipse ~/opt/eclipse-android`
1. Launch Eclipse.
1. At prompt, set workspace to "../../../workspace" and check always.

# Plugins
- ADT: https://dl-ssl.google.com/android/eclipse/
- UCDetector: http://ucdetector.sourceforge.net/update plugin.
- FindBugs: http://findbugs.cs.umd.edu/eclipse plugin.

# Preferences

#### Disable Git
- Uncheck Team -> Git -> Projects -> Automatically share projects located in a Git repository
- Uncheck Team -> Git -> Projects -> Track each branch's imported projects and restore on checkout
- Uncheck Team -> Git -> Refresh resources when index changes
- Uncheck Team -> Git -> Refresh only when workbench is active

#### Java Warnings
- Set Warning Java -> Compiler -> Errors/Warnings -> Null analysis -> Potential null pointer access
- Set Warning Java -> Compiler -> Errors/Warnings -> Null analysis -> Redundant null check
- Set Warning Java -> Compiler -> Errors/Warnings -> Annotations -> Missing '@Override' annotation
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Value of parameter is not used
- Set Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Ignore in overriding and implementing methods
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unused type parameter
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unnecessary 'else' statement
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unnecessary cast or 'instanceof' operation
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unnecessary declaration of thrown exception
- Set Warning Java -> Compiler -> Errors/Warnings -> Unnecessary code -> Unused 'break' or 'continue' label
- Set Warning Java -> Compiler -> Errors/Warnings -> Name shadowing and conflicts -> Field declaration hides another field or variable
- Set Warning Java -> Compiler -> Errors/Warnings -> Name shadowing and conflicts -> Local variable declaration hides another field or variable
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Potential accidental boolean assignment
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Empty statement
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Unused object allocation
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Potential resource leak
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Missing synchronized modifier on inherited method
- Set Warning Java -> Compiler -> Errors/Warnings -> Potential programming problems -> Class overrides 'equals()' but not 'hashCode()'
- Set Warning Java -> Compiler -> Errors/Warnings -> Code style -> Parameter assignment

#### Java Style
- Click Java -> Code Style -> Formatter -> Import... and select ~/Workspace/aosp/development/ide/eclipse/android-formatting.xml
- Click Java -> Code Style -> Formatter -> Organize Imports -> Import... and select ~/Workspace/aosp/development/ide/eclipse/android.importorder
- Set to m Java -> Code Style -> Conventions for variable names -> Fields -> Prefix list

#### General Style
- Check General -> Editors -> Text Editors -> Insert spaces for tabs
- Check General -> Editors -> Text Editors -> Show print margin
- Check General -> Editors -> Text Editors -> Show whitespace characters
- Uncheck General -> Editors -> Text Editors -> configure visibility -> Space -> Leading
- Uncheck General -> Editors -> Text Editors -> configure visibility -> Space -> Enclosed

#### XML Style
- Check XML -> XML Files -> Editor -> Indent using spaces
- Set to 4 Check XML -> XML Files -> Editor -> Indentation size
- Set to 80 Check XML -> XML Files -> Editor -> Line width

#### Android
- Set Android -> DDMS -> Base local debugger port
- Set C/C++ -> Build -> Environment -> Add...
  - NDK_CCACHE /Users/stephen/opt/homebrew/bin/ccache
  - USE_CCACHE 1
- Set Android -> NDK -> NDK Location
- Uncheck Android -> LogCat -> Monitor logcat for message from applications in workspace

#### Misc
- Uncheck C/C++ -> Indexer -> Enable indexer
- Uncheck Startup and Shutdown -> Confirm exit when closing last window
- Check Startup and Shutdown -> Refresh workspace on startup
- Uncheck Workspace -> Refresh on access
- Check Run/Debug -> Launching -> Always launch the previously launched application

# Project Explorer Window Settings
- Set Project Explorer -> Top Level Elements -> Working sets

# Problems Window Settings
- Uncheck Configure Contents... -> Use item limits
