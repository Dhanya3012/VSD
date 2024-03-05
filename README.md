# A 4-week Research Internship on VSDSquadron Mini RISC-V Dev Board








BOARD SPECIFICATIONS:

| Tech specs   |   |    |
|------------|------------|------------|
| *Board* | Name     | VSDSquadron Mini    |
|      | SKU    | VSDSQM    |
| *Microcontroller*    | CH32V003F4U6 chip with 32-bit RISC-V core based on RV32EC instruction set    |     |
| *USB connector* | USB 2.0 Type-C    |     |
| *Pins*     | Built-in LED Pin     | 1X onboard user led (PD6)     |
|      | Digital I/O pins     | 15     |
|      | Analog I/O pins     | 10-bit ADC, PD0-PD7, PA1, PA2, PC4     |
|      | PWM pins     | 14X     |
|      | External interrupts     | 	8 external interrupt edge detectors, but it only maps one external interrupt to 18 I/O ports     |
| *Communication*     | USART     | 	1x, PD6(RX), PD5(TX)     |
|      | I2C     | 1x, PC1(SDA), PC2(SCL)    |
|      | SPI     | 1x, PC5(SCK), PC1(NSS), PC6(MOSI), PC7(MISO)     |
|      | Programmer/debugger     | Onboard RISC-V programmer/debugger, USB to TTL serial port support     |
| *Power*     | I/O voltage     | 3.3 V    |
|      | Input voltage (nominal)     | 5 V    |
|      | Source Current per I/O Pin    | 8 mA     |
|      | Sink Current per I/O Pin     | 8 mA     |
| *Clock speed*     | Processor    | 24 MHz     |
| *Memory*     | SRAM     | 2kb onchip volatile sram,16kb external program memory     |
   

This repo is intended to document the weekly progress.

### The first online meet was held on 16th of Feb 2024 @6PM

<details>
    <summary> TASK 1 </summary>
 
1) install Yosys 

2) install iverilog 

3) install gtkwave

### CLONING RISC-V GNU TOOLCHAIN

# To install git 
sudo apt install git-all   

 make sure to install the dependencies
![git-all](https://github.com/Dhanya3012/VSD/assets/160576442/8276475f-10d4-406e-bab5-fc32cf4d7b1f)




### INSTALLING YOSYS, IVERILOG & GTKWAVE.

### 1.YOSYS


git clone https://github.com/YosysHQ/yosys.git
![git clone](https://github.com/Dhanya3012/VSD/assets/160576442/cf676ad3-13de-4725-b5e2-31c9ff90cadc)

cd yosys 

sudo apt install make
![sudo apt](https://github.com/Dhanya3012/VSD/assets/160576442/d999f8a0-79e2-4dbf-b2e1-4a82c6f130f0)

sudo apt-get install build-essential clang bison flex \libreadline-dev gawk tcl-dev libffi-dev git \ graphviz xdot pkg-config python3 libboost-system-dev\libboost-python-dev libboost-filesystem-dev zlib1g-dev

make config-gcc

make 

sudo make install
![sudo make install](https://github.com/Dhanya3012/VSD/assets/160576442/3006c9da-25c2-44d0-a76c-3b400015ac05)


### 2.iVerilog
installing iVerilog

sudo apt update

sudo apt-get install iverilog
![install verilog](https://github.com/Dhanya3012/VSD/assets/160576442/af1b2192-a8ac-4c40-99a2-997fb82d2834)


### 3.GTkWave
installing GTkWave

 sudo apt-get install gtkwave 
![GTKwave](https://github.com/Dhanya3012/VSD/assets/160576442/7ab62f60-e87c-4db5-a00e-abffcba9392a)


</details>

<details>
  <summary> TASK 2 </summary>
  
![Block Diagram of UART](https://github.com/Dhanya3012/VSD/assets/160576442/c71465aa-faac-47b1-a3a6-7fe450e2b680)

### Input Waveform

![Input Waveform](https://github.com/Dhanya3012/VSD/assets/160576442/3cb68f0a-7504-4449-a745-e634e1b2c240)

### Output Waveform

![Output Waveform](https://github.com/Dhanya3012/VSD/assets/160576442/7a6a8001-9336-47e8-bc03-26754eb22d7b)


</details>
<details>
  <summary> TASK 3 </summary>

![i1](<WhatsApp Image 2024-02-26 at 15.14.58_491a6b56.jpg>)

![i2](<WhatsApp Image 2024-02-26 at 15.16.03_a8686182.jpg>)
![i3](<WhatsApp Image 2024-02-26 at 15.16.48_65363ecc.jpg>)
![i4](<WhatsApp Image 2024-02-26 at 15.17.39_0ced7cfd.jpg>)
![WaveForm](<WhatsApp Image 2024-02-26 at 15.18.20_938e33c5.jpg>)
</details>

<details>
   <summary> TASK 4 </summary>
   
![1d](https://github.com/Dhanya3012/VSD/assets/160576442/311e0420-cb8c-49c1-829d-3d7799862aaf)
![2d](https://github.com/Dhanya3012/VSD/assets/160576442/4b69ee8d-fd2c-4f2f-9d19-9eea54c2f7aa)
![3d](https://github.com/Dhanya3012/VSD/assets/160576442/96a818b7-deb5-4fdd-b4ef-5bc74641c94e)
![4d](https://github.com/Dhanya3012/VSD/assets/160576442/eb46e755-f452-44a5-9b93-9fad4498f1ae)
![5d](https://github.com/Dhanya3012/VSD/assets/160576442/2e19e6f6-f3ca-4c2b-8480-1502da9a41f9)
![1w](https://github.com/Dhanya3012/VSD/assets/160576442/8769db01-bad3-40c0-aa74-257e60dc4cc2)
![2w](https://github.com/Dhanya3012/VSD/assets/160576442/1a9c34e6-cd07-4fe2-bed3-41b76f54949c)
![3w](https://github.com/Dhanya3012/VSD/assets/160576442/42c8a67f-6e82-4f38-8f49-d142c376d7dc)
![4w](https://github.com/Dhanya3012/VSD/assets/160576442/052177aa-22ed-491e-afab-32d9ed486c10)
![5w](https://github.com/Dhanya3012/VSD/assets/160576442/31db9307-61f2-4059-8b66-bfb28d13c96f)
![1](https://github.com/Dhanya3012/VSD/assets/160576442/861fe59e-b1d8-425f-ad9f-39ef48d391bc)
![2](https://github.com/Dhanya3012/VSD/assets/160576442/9234ca1d-0af5-40f1-b37f-1dd76f94839c)
![3](https://github.com/Dhanya3012/VSD/assets/160576442/9a395fa8-ee1e-4b89-90a0-38fd9d453c17)
</details>

<details>
   <summary> TASK 5 </summary>
   
   
