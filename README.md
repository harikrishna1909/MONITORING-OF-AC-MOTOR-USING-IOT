## The main blocks of this project are:
1. Regulated power supply.
2. PIC Microcontroller.
3. ESP8266 Wi-Fi module. 
4. Voltage sensor. 
5. Current Sensor.
6. Frequency Sensor. 
7. Temperature Sensor. 
8. Reset. 
9. Crystal oscillators. 
10. LED indicators. 
11. Buzzer with driver. 
12. LCD display.

### SOFTWARE DESCRIPTION
This project is implemented using following software’s:
Express PCB – for designing circuit
PIC C compiler - for compilation part

### COMPILATION AND SIMULATION STEPS:
For PIC microcontroller, PIC C compiler is used for compilation. The compilation steps are as follows:
1.Open PIC C compiler.
2.You will be prompted to choose a name for the new project, so create a separate folder where all the files of your project will be stored, choose a name and click save.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/70a1ca94-e38a-4347-8984-1d58f39e5e67)

Fig : Picture of opening a new file using PIC C compiler
3.Click Project, New, and something the box named 'Text1' is where your code should be written later.
4.Now you have to click 'File, Save as' and choose a file name for your source code ending with the letter '.c'. You can name as 'project.c' for example and click save. Then you have to add this file to your project work.  
      
![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/09fdbff8-ae16-4bcd-9168-e39e284a45f0)

Fig : Picture of compiling a new file using PIC C compiler

 
![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/45a5d9e8-9501-4abb-a080-e97a90b57b8b)

Fig : Picture of compiling a project.c file using PIC C compiler

5.You can then start to write the source code in the window titled 'project.c' then before testing your source code; you have to compile your source code, and correct eventual syntax errors. 

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/4153e7ec-d71e-4ee3-8b8b-78d894496c7a)

Fig : Picture of checking errors and warnings using PIC C compiler

6.By clicking on compile option .hex file is generated automatically.
7.This is how we compile a program for checking errors and hence the compiled program is saved in the file where we initiated the program. 

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/3b97dfbf-cab8-4065-85c9-c0fb082a929c)

Fig : Picture of .hex file existing using PIC C compiler

After compilation, next step is simulation. Here first circuit is designed in Express PCB using Proteus 7 software and then simulation takes place followed by dumping. The simulation steps are as follows:
8.Open Proteus 7 and click on IS1S6.
9.Now it displays PCB where circuit is designed using microcontroller. To design circuit components are required. So click on component option.
10. Now click on letter ’p’, then under that select PIC16F73 ,other components related to the project and click OK. The PIC 16F73 will be called your “'Target device”, which is the final destination of your source code.      
       




### DUMPING STEPS:
The steps involved in dumping the program edited in proteus 7 to microcontroller are shown below:
1.Initially before connecting the program dumper to the microcontroller kit the window is appeared as shown below.               

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/77665172-f1fe-40dc-ab94-cc12e292356c)

Fig : Picture of program dumper window
2.Select Tools option and click on Check Communication for establishing a connection as shown in below window

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/5357d91d-d1f2-441e-9757-c4475da4b4cc)

Fig : Picture of checking communications before dumping program into microcontroller
	
3. After connecting the dumper properly to the microcontroller kit the window is appeared as shown below.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/afd8ff73-d0db-40f4-8e34-92ff08a610ea)

Fig : Picture after connecting the dumper to microcontroller
4. Again by selecting the Tools option and clicking on Check Communication the microcontroller gets recognized by the dumper and hence the window is as shown below.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/97807f7e-6509-42c3-91f2-bcd108cd1688)

Fig : Picture of dumper recognition to microcontroller


5. Import the program which is ‘.hex’ file from the saved location by selecting File option and clicking on ‘Import Hex’ as shown in below window.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/efe54f93-461e-4cc3-9c75-2e9ccf17d231)

Fig : Picture of program importing into the microcontroller

6. After clicking on ‘Import Hex’ option we need to browse the location of our program and click the ‘prog.hex’ and click on ‘open’ for dumping the program into the microcontroller.
7. After the successful dumping of program the window is as shown below.
![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/4e94bb85-e182-42b8-be88-b96bce1c3ad9)

Fig : Picture after program dumped into the microcontroller


### RESULTS
The main controlling device of the whole system is a Microcontroller. AC motor through Voltage sensor, current sensor, temperature sensor and frequency counter are interfaced to Microcontroller. The Microcontroller gets input from all the sensors, which will be processed and transmitted into to the thingspeak cloud over WI-FI module. The parameters are displayed on the mobile phone. The system alerts through BUZZER, if any abnormality is detected in the parameter values. To perform the task, Microcontroller is loaded with an intelligent program written in embedded ‘C’ language. The Microcontroller is programmed using Embedded C language.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/0b695ac2-204b-4f50-b8f8-2be8fbaf0d2b)

Fig : Representation of Voltage graph.         

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/372cc809-8a0e-4e0d-a0ce-393526aab365)

Fig : Representation of Current graph.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/4e372090-a0f7-4bd6-9be8-15487a2271f9)

Fig : Representation of  Temperature graph.

![image](https://github.com/harikrishna1909/MONITORING-OF-AC-MOTOR-USING-IOT/assets/134721651/24c2a2eb-49d0-46eb-a835-e34b479a75c5)

Fig : Representation of Frequency graph.
