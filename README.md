# SE-E-Portfolio-Cheat-Engine
This repository will contain the materials that were used and created during the E-Portfolio: Cheat Engine

## Example

1. Attach Cheat Engine to the process of your choice. I will use Terraria in this example.
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20135718.png)
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20140130.png)

2. Scan for a value of your choice until you find the correspondig address. I will be using a stack of wood.
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20141311.png)

3. Right click the address and choose "See what accesses this address". You will see a lot of compare instructions (cmp). These come from the GUI checking if you have 0 of that item, in which case it will stop diplaying that item in your inventory(as can be seen in the example below).

![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20140747.png)

4. Right click one of the compare instructions and choose "show this address in the dissassembler"

5. In  the dissassembler, press Ctrl + A to auto assemble the specific code. Then go to Template -> AOB Injection.
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20141037.png)

6. You should see something that resembles following template code:
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20141322.png)

7. Below the compare instruction, add an instruction that pushes the value 999 to the address that is compared (mov [register + offset], (Int)999).
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20143851.png)

8. Go to File -> Assign to current cheat table.
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20141651.png)

9. Now activate your script in the cheat table.
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20142524.png)

10. I don't know what you would want 999 copper shortswords for, but hey, now you have 999 copper shortswords
![alt text](https://github.com/schmida736/SE-E-Portfolio-Cheat-Engine/blob/main/img/Screenshot%202021-06-09%20142456.png)
