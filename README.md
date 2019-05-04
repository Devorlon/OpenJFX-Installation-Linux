# How to install Java 12 & JavaFX for Debian – Eclipse-IDE
1.	Install Ubuntu 19.04
2.	Update Ubuntu 19.04
3.	Run: 
```
sudo apt-get install openjdk-12-jdk
```
4.	Run:
```
sudo snap install eclipse
```
5.	Download OpenJFX 12
6.	Extract the .zip and place the contents in a folder called .javafx in your home folder.
7.	Open eclipse
8.	Select: 
```
Eclipse -> Window -> Preferences -> Java -> Build Path -> User Libraries -> New
```
9.	Name it JavaFX12
10.	Click ‘Add External JARs…”
11.	Go to /home/.javafx/lib
12.	Select OK
13.	Select ‘Apply and Close’
14.	Select: 
```
Eclipse -> Help -> Eclipse Marketplace
```
15.	In the find field search for ‘FX’ (press enter)
16.	Install a version greater than or equal to ‘e(fx)clispe 3.5.0’
17.	Accept License agreement and Certificates then restart.

Well done you can now create Java and JavaFX applications in Linux.

## Help:
Q: Will this work on any Distro or even Windows?

A: Yes, it should as long as you replace the ‘apt install’ with your system counterpart.


Q: When I try to run my application, it tells me:

Error: JavaFX runtime components are missing, and are required to run this application.
A: Follow these steps:
1.	Select: Eclipse -> Run -> Run Configurations
2.	Under ‘Java Application’ select your created program
3.	Under the arguments tab insert the following command into ‘VM arguments’ as one line:

-module-path /home/YOUR_USERNAME/.javafx/lib -add-modules javafx.controls,javafx.graphics,javafx.fxml

4.	Select ‘Apply’

Q: Will this work for Netbeans / IntelliJ?

A: No, a lot of this is specific to Eclipse if you want a good guide follow the OpenJFX documentation: 
https://openjfx.io/openjfx-docs/#introduction


Q: Can you add pictures?

A: I would like to as I find them easy to follow as well, but I can’t be bothered.


Q: My machine is now broken.

A: That’s not a question, and I don’t care reset it and try again.


Q: You stole this from openjfx.io 

A: Yes, yes I did. Though I did it because I / the people I wrote this for found it easier to follow.
(P.S. Please go check these guys out they’ve done tones for the FX community)

