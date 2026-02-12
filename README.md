# Personnal Projects

Lots of mini projects using ESP32, STM32MP135, Microchip SAMD/SAME
Many have references in my [github's repos](https://github.com/ericbaril72?tab=repositories)


# Firmware
## ESP32
- Visual Studio / Platformio /  C & C++
- Circuit Python / Python
- ESPHome / yaml
<div>
<img src="https://shop.m5stack.com/cdn/shop/products/1_3f420584-fb2f-48c3-bd01-17f083de0880_1200x1200.jpg" alt="drawing" width="200"/>
<img src="https://shop.m5stack.com/cdn/shop/products/12_8be1a6fd-be56-47c4-88c3-59f7fe3a3021_1200x1200.webp"  alt="drawing" width="200" />
<img src="https://shop.m5stack.com/cdn/shop/products/1_2_c215b5d9-d41a-4ab8-ad54-b2531930f075_1200x1200.jpg" alt="drawing" width="200"/>
<img src="https://shop.m5stack.com/cdn/shop/files/4_ae790f23-43de-4348-9df0-fa37c1c47dd2_1200x1200.webp" alt="drawing" width="200"/>
</div>
Canbus, Irda, LVGL, DMA->SPI

## STM32MP135
- Visual Studio / Buildroot
<img src="https://shop.m5stack.com/cdn/shop/files/1_73e1d5e8-3281-4a6b-b4f5-de7687f37cef_1200x1200.webp" width="200"/>

- defconfig update to support RAUC A/B partition
- Modifying UBOOT to control bootsequence LCD content via patches
- Modifying Linux config to select output console

## Home Assistant 
- Over 40 Nodes
- ESP32 Nodes for fireplace and thermostat

## Web front-end
### [Motrec.io](http://www.motrec.io)
Cloud server built with NGINX, Gunicorn, Flask web back-end, SQLite

### Automating CAD to ERP 
Python scripts to automate the process of converting CAD drawings into the ERP system with visual validation interface.

Engineering:
- Automate the process of Extracting the BOM, Generate all PDF documents, and compare with the ERP system to identify the missing components and any revision changes.
- The visual Interface reports any missing information/drawings/assemblies and inconsistencies.
Once the engineering teams has corrected all issues
- Automate the process of updating the data in the ERP system
- Reporting on the list of changes.
Result: 40 hours / week saved

Procurement:
Orders would be placed daily with the supplier at the last paid price. Supplier's response if a PDF document would show the quoted price resulting in 
thousands of line items to correct into the ERP system.
- Script to automate the correction of all line item
- Visual report in order of price discrepenties
Result : 20 hours / week saved + Same Day quote errors identification




# Hardware
## ESP32 Dual Canbus Gateway with LCD
Dual isolated canbus transceiver with LCD and Wifi interface.  
Maximize the use of Off-the-shelf sub-modules for a quick and low cost alternative to Peak+Laptop alternative


# Previous Work Projects
## 13 Cells Lithium Battery BMS with integrated Electronic Fuse, Programmable DC output and integrated Charger
Based on previous generations with external high cost battery chargers, we implemented a bi-direectional DC-DC converter circuit rather then unidirectional.  
This allowed to use the same circuit for both:
  - 48V battery voltage TO generate a programmable output voltage (6or12V) for Coordinate the team
  - 24V External power supply TO 48V boost for battery charging
System Cost Reduction of 20$ * 50k units per year.
  - 30$ savings from buying a 20$ Laptop type 90W power-supply instead of a 50$ Battery charger.
  - 10$ cost increase on the BMS 
Results: 1M$ Savings/year

<img src="https://www.bx-legacy.com/cdn/shop/products/1568656413483_1121x700.JPEG?v=1568656650" width="500" />

## Field Oriented Control Permanent Magnet AC Motor drive
Initial drive was using brushless dc algorythm resulting in [trapezoidal voltage output](https://wiki.analog.com/resources/eval/user-guides/ad-fmcmotcon1-ebz/introduction/bldc_control).  
Increasing the computing power of the CPU ( +1$) = Overall energy efficiency +25% = 33% larger battery ( more range ).

Merging the production volumes of both 24V and 36V into a much higher volume of a single product allowed for overall cost savings covering the CPU price increase.
Results: 33% more range at no extra cost

<img src="https://www.bx-legacy.com/cdn/shop/products/1575326251202_512x399.jpg" width="400" />
