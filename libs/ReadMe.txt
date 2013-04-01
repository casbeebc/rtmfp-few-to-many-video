
To make use of the Flash Player 10.1 features in Flash Builder in Flex and ActionScript projects, you will need to add the playerglobal.swc.  The playerglobal.swc is the reference that exposes all new APIs that are available as of this release.

When adding the playerglobal.swc, please remember to first remove the reference to the existing playerglobal.swc in your project.

Create a new application project. Edit the project properties:
1. Open the "Flex Build Path" tab
2. Click "Add SWC" and navigate to the that path, and then deeper into frameworks/libs/player/10, select playerglobal.swc.
3. Expand "playerglobal.swc", double-click "Link Type" and change it to "External".

To update the HTML to require Flash Player 10.1:
4. Open the "Flex Compiler" tab
5. In "HTML wrapper", change the "Require Flash Player version" to 10.1.0. 

Alternately, you can override this value for the compiler by adding -target-player=10.1.0 to "Additional commandline arguments", and leaving HTML wrapper alone.

You will need to test content in the browser with Flash Player 10.1 installed.

