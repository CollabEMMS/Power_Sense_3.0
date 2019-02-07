README.txt
Power Sense v3.1
@author: Joe Wambach

last edit: 12/6/18

Edits to be made in the future:
	- Fix issue with test header for CH1. Either flip connections to filters so CH1- is connected to GND. OR just change the connection for the test header from CH1+ to CH1-.
		DONE

	⁃ Fix circuitry so that resistor divider (bypassing transformer) and resistor divider (on transformer secondary) don’t connect and interfere with each other. OR just develop a good method to assemble boards with only one set of resistors or the other.

	⁃ Change resistor values on transformer secondary. It currently uses 10k and 1k to scale down by 11. This works for 120Vrms since transformer will output about 6Vp so MCP will get ~600mV. However, if 240Vrms connect to primary coils, 12Vp comes out of secondary meaning MCP will see 1.2Vp which is > 660mV maximum rating.

	- Fix silkscreen part numbers and values

	- Fix trace connection to +5V of SPI because it barely touches it 
		DONE