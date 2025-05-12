# ece3301l-lab-10-i2c-bus-implementation-solved
**TO GET THIS SOLUTION VISIT:** [ECE3301L LAB 10-I2C Bus Implementation Solved](https://www.ankitcodinghub.com/product/ece3301l-lab-10-i2c-bus-implementation-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;91511&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;ECE3301L LAB 10-I2C Bus Implementation Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
LAB 10: I2C Bus Implementation

This lab will introduce the student to the use of the I2C bus and in particular to interface to a Real-Time Clock (RTC) and Digital Temperature Sensor.

The following link will introduce the student to the I2C bus:

http://www.ti.com/lit/an/slva704/slva704.pdf

I will go over in class to the concept of this bus.

Normally the I2C bus uses a hardware technique whereas all the data bit transmissions are performed by internal hardware inside the microcontroller. This method allows faster data transmissions but the two SCL and SDA pins must be dedicated. In addition, the PIC 18 microcontroller that we are using merges the two I2C and SPI functions into the same pins thus allowing the use of only one function and not both simultaneously. If we want to use both SPI and I2C, we will need to switch from the use of hardware I2C to software I2C. This new technique will use the concept of software bit banging to perform all the data bit transmission. For sure this technique will not have the same speed performance as the hardware I2c but it does allow the microcontroller to communicate with any I2C device. Since bit banging can be applied to any pin, software I2C also allows the flexibility to choose any GPIO pin for the implementation.

The attached file ‘I2C.c’ will provide the needed library function for the software I2C implementation. Now, let us choose two different pins for the signal SCL and SDA. See the attached schematics for the pin assignments of those two pins. For example, let us physically move SCL to PORT C bit 0 and SDA to PORT C bit 1. Edit the file to reflect the assignments of those signals.

Part 1)

The DS1621 is a digital thermometer with the I2C bus interface. Here is the link to its datasheet:

https://pdfserv.maximintegrated.com/en/ds/DS1621.pdf

Study this device and pay attention to page 9 regarding the serial communications to this device. On the next page (page 10), the command ‘Read Temperature’ will provide the reading of the actual temperature. Write a routine called ‘char DS1621_Read_Temp()’ to return the reading of the temperature. Follow the following steps:

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
<ol>
<li>a) &nbsp;Use the attached ‘Lab10_sample.c’ as the reference for the rest of this lab.</li>
<li>b) &nbsp;Go to the second attached file ‘I2C.c’ and copy the content of the function ‘char I2C_Write_Cmd_Read_One_Byte (char Device, char Cmd)’ and put that content in the function ‘char DS1621_Read_Temp()’ located in the attached ‘I2C_Support.c’</li>
<li>c) &nbsp;At the beginning of the routine, define a char variable ‘Device’ being 0x48. That is the I2C address for this DS1621 device</li>
<li>d) &nbsp;Next, define another char variable called Cmd and set it to equal to the label READ_TEMP (0xAA). That is the ‘Read_Temperature’ command</li>
<li>e) &nbsp;That will conclude the definition of this routine.</li>
</ol>
In addition, we will need to initialize the DS1621. We need to build another function for this task. Let us call that function ‘void DS1621_Init()’ and it is also located in the ‘I2C_Support.c’ file.

<ol>
<li>a) &nbsp;At the beginning of the routine, define a char variable ‘Device’ being 0x48. That is the I2C address for this DS1621 device</li>
<li>b) &nbsp;Insert the following 2 lines
<ol>
<li>I2C_Write_Cmd_Write_Data (Device, ACCESS_CFG, CONT_CONV);</li>
<li>I2C_Write_Cmd_Only(Device, START_CONV)</li>
</ol>
</li>
</ol>
When both new functions are defined, do the following steps:

<ol>
<li>a) &nbsp;Call (add) the function ‘void DS1621_Init()’ in the Do_init() routine to initialize the DS1621 chip</li>
<li>b) &nbsp;Write a while loop that will wait every second (Use Wait_One_Second() routine) and call the routine ‘char DS1621_Read_Temp()’ to get the temperature (in degree Celsius). Calculate the equivalent Fahrenheit temperature and printout both temperatures on TeraTerm.</li>
</ol>
Part 2)

Next, we are going to use the I2C to interface to a Real-Time-Clock (RTC) device called DS3231. This device is used to keep the time. Below is the link to the datasheet of this device:

https://datasheets.maximintegrated.com/en/ds/DS3231.pdf

The RTC has a set of registers that store the actual time in terms of second, minute, hour, day, day of the week, month and year. Refer to page 11 of the datasheet. The registers with the

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
addresses from 00 to 06 are the ones that contain the time values. We will need to write a routine called ‘void DS3231_Read_Time()’ to fetch all the mentioned registers and to display them on the TeraTerm. In addition, to avoid displaying duplicated data, it is required to check the ‘Second’ register to determine whether it has been updated with a new second. If so, then the new data can be displayed on the screen. When a new time is displayed, also called the routine ‘int DS1621_Read_Temperature()’ from Part 1) to get the temperature and show it on the screen.

Here is how to implement this routine:

<ol>
<li>a) &nbsp;Take the content of the sample routine ‘char I2C_Write_Address_Read_One_Byte(char Device, char Address) provided in the ‘I2C_Hard.c’ and place it in ‘void DS3231_Read_Time()’ inside the ‘I2C_Support.c’.</li>
<li>b) &nbsp;Since this is now a void routine, there is no need for the ‘return’ statement. Remove that line at the end.</li>
<li>c) &nbsp;At the beginning of the routine, define a char variable ‘Device’ being 0x68. That is the I2C address for this DS1621 device. That is the I2C address for this DS3231 device</li>
<li>d) &nbsp;Next, add another char variable ‘Address’ with the value 0x00. This is the value for the register 0x00 pointing to the register ‘second’</li>
<li>e) &nbsp;Delete the line ‘Data_Ret = I2C_Read(NAK);’</li>
<li>f) &nbsp;Add a new line ‘second = I2C_Read(ACK);’</li>
<li>g) &nbsp;The new line above allows the system to read the register ‘second’ from DS3231. Add similar lines below that line for the variables ‘minute’, ‘hour’, ‘dow’ (day of week), ‘day’, ‘month’, and ‘year’. Do that in the order provided. For the last variable ‘year’ substitute ‘ACK’ by ‘NAK’ to terminate the read sequence</li>
<li>h) &nbsp;Make sure to end the function with ‘I2C_Stop();’</li>
</ol>
Once this routine is completely designed, modify Part 1) of while loop by removing the ‘Wait_One_Second()’ routine and instead call this new routine ‘DS3231_Read_Time()’ to get the new time and in particular the reading of the ‘second’ register. Compare the new reading of the ‘second’ with an old reading. If the new second is the same as the old, then do nothing. If different, then print out the actual time. Use the following printf format

printf (“%02x:%02x:%02x %02x/%02x/%02x”,hour,minute,second,month,day,year);

This will display the time and date using the format “hh:mm:ss mm/dd/yy’.

In addition, print out the actual temperature as performed in part 1) followed by the readout of the temperature.

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
Note: Due to the potential effect that the RTC might not properly initialize, the time and date might not be correct. That will be fixed on the next part.

Part 3)

The next task is to write a routine to setup an initial time for the RTC. Call that routine ‘void DS3231_Setup_Time()’. The purpose of this routine is to pre-program all the registers from 00 to 06 of the RTC with fixed numbers.

Here is how to implement this function:

<ol>
<li>a) &nbsp;Copy the function ‘void I2C_Write_Address_Write_One_Byte(char Device, char Address, char Data)’ and name it as ‘void DS3231_Setup_Time()’. There is no parameter needed for this function</li>
<li>b) &nbsp;At the beginning of the routine, define a char variable ‘Device’ being 0x68. That is the I2C address for this DS1621 device.</li>
<li>c) &nbsp;Next, add another char variable ‘Address’ with the value 0x00. This is the value for the register 0x00 pointing to the register ‘second’</li>
<li>d) &nbsp;Set the values that you want to use to the variables ‘second’, ‘minute’, ‘hour’, ‘dow’, ‘day’, ‘month’ and ‘year’. Set the value as in bcd value. For example, if the minute is to be set as 45, don’t convert that number into hex number but use the value 0x45 instead.</li>
<li>e) &nbsp;Replace the line ‘I2C_Write(Data);’ with I2C_Write(second);’</li>
<li>f) &nbsp;Then add below that line the same I2C_Write command but with the next variable ‘minute’</li>
<li>g) &nbsp;Repeat the action above for the remaining variables.</li>
<li>h) &nbsp;Make sure to end the function with I2C_Stop();</li>
</ol>
Once this function is implemented, make a call to this function before the while (1) loop in the part 2). The time that will be displayed will be the new start time set by the new function.

Part 4)

Take the functions implemented on lab 9 for the remote control and move them in this lab10. The following tasks must be performed:

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
<ol>
<li>1) &nbsp;Modify the ‘interrupt.c’ file by:A. Creating the function init_INTERRUPT() by moving all the instructions on the main program that initialize the interrupt operationsB. movingthefollowingfunctionsintothisfile:
<ul>
<li>void interrupt high_priority chkisr()</li>
<li>void TIMER1_isr(void)</li>
<li>void force_nec_state0()</li>
<li>void INT0_ISR()</li>
</ul>
</li>
<li>2) &nbsp;When done, add the codes from last week’s code in the while (1) loop checking for the ‘nec_ok’ variable to be 1 indicating that a button on the remote control is pressed. Display as normal the button on the LCD screen as in lab 9. Remove the code to activate the three RGB LEDs since we don’t have them anymore in this lab. The BEEP sound and the Key Pressed LED should be the same as in the previous lab.</li>
<li>3) &nbsp;When a button is pressed, add a check to see whether it is the ‘EQ’ button. When that happens, call the routine ‘void DS3231_Setup_Time()’ to preset the time. The new time will be displayed on TeraTerm.Notes: When the project is completed, you should have the following files in the:
<ul>
<li>Header Files: o I2C.ho I2C_Support.h o Interrupt.h

o ST7735.h</li>
<li>Sources Files: o I2C.co I2C_Support.c o Interrupt.c

o Lab10.c

o ST7735.c</li>
</ul>
</li>
</ol>
</div>
</div>
</div>
