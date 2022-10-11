# ese5190-lab2
Sudong wang 
Windows 10 Dell XPS 13

Section1 SDK
To get your QT Py board sending data over USB again, this time via the C SDK
Open the link is given, https://datasheets.raspberrypi.com/pico/getting-started-with-pico.pdf, since I am operating in the windows environment, I need to navigate to page 9.2.1. 
![image](https://user-images.githubusercontent.com/113209201/194995730-be55d851-e1d8-4cd1-8964-4a8d99e06735.png)

download and install the tools above. 

for the arm GNU toolchain, I select the one ending with .exe
![image](https://user-images.githubusercontent.com/113209201/194995759-ed8d6405-6a46-4063-b5ce-f02181e49b5a.png)


and remember to click the add path to the environmental variable

for CMake, I use the windows installer
![image](https://user-images.githubusercontent.com/113209201/194995801-6f9f2cab-3bed-40c0-8901-6b30ed1fc1ad.png)

and click add system path to all users during installation. 
 
Then for the visual studio, remember to click the link given instead of downloading from the public website since you need to click the “desktop development with C++”. 
For python 3.10 and git, it is recommended to use the installer from the link. 

After that, I open the terminal from the VS2022. 
![image](https://user-images.githubusercontent.com/113209201/194995806-abe56f0f-d016-42cd-8854-9750f4399a9e.png)

select the file location. I create the ese5190 file in the document. 
cd to the file, and use the code from 9.22

after successfully set up, set the path to SDK as 
setx PICO_SDK_PATH "..\..\pico-sdk"
and close the terminal and open a new one. 
cd to the file location, and type the code given from 9.23
the terminal should look like 
![image](https://user-images.githubusercontent.com/113209201/194995822-3051f213-dfc3-4bba-86a0-675d161304f3.png)

then copy the file from the pico example:
![image](https://user-images.githubusercontent.com/113209201/194995835-9d2a8b05-1ed8-4599-9785-8c2aea66dd1d.png)

after using putty to connect the RP2040 and copy the example code to the device, it will loop hello world as follows:
![image](https://user-images.githubusercontent.com/113209201/194995862-e7a6e9ad-0223-41ea-841d-77d2dbc21432.png)



