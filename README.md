# lora_arduino
lora_arduino
this is from WWW.DORJI.COM.
this is the driver for sx1278.
the control board is  Arduino  Board  Mega2560. 
1.DRF1278F: 433MHz band, SPI interface, +3.3 working voltage. 

2.I/O Port definition of Mega2560 

int led  = 13; 

int nsel = 22; 

int sck  = 24; 

int mosi = 26; 

int miso = 28; 

int dio0 = 30; 

int reset = 32; 

a.Maser LED: Sending data indication; Slave LED: Receiving data indication 

b.NSEL: DRF1278F SPI chip select input 

c.SCK: DRF1278F SPI clock input 

d.MOSI: DRF1278F SPI data input 

e.MISO: DRF1278F SPI data onput 

f.DIO0:  Special  application  port  which  can  be  used  as  the  indication  for  the  success  of sending or receiving a full data package

g.RESET: DRF1278Freset pin. It can be controlled by an I/O port or floated. In the sample codes this pin is not used. 

3.In Master side, the module sends one data package. After 2s delay, it will send the next data 
package.  In  the  sending  process,  the  LED  will  be  lighted.  After  finishing  transmission,  the  LED  will be turned off. In Slave side, the LED will blink when it receives a full package of data. 
