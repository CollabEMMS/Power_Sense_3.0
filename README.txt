README.txt
Power Sense v3.1.2
@author: Joe Wambach
@LastEditor: Joe Wambach		<----------------------- UPDATE THIS WHOEVER LAST EDITS THIS

last edit to this document: 2/21/19

Revision History:

	3.0:	Initial version of new power sense
	3.1: 	Removed Murata Transformer
		Removed R1
		Added Test Headers for CH0+, CH1+, HFout, Fout0, Fout1
		Added Triad Transformer
		Added Resistor Divider to bypass transformer circuitry
	3.1.1:	Changed connection for test header from CH1+ to CH1-
		R5 --> 20k 1%
	3.1.2:	Removed R15 and R16
		Fixed Connection to +5V on SPI Connector

Edits to be made in the future:
	- Fix issue with test header for CH1. Either flip connections to filters so CH1- is connected to GND. OR just change the connection for the test header from CH1+ to CH1-.
		DONE

	⁃ Fix circuitry so that resistor divider (bypassing transformer) and resistor divider (on transformer secondary) don’t connect and interfere with each other. OR just develop a good method to assemble boards with only one set of resistors or the other.

	⁃ Change resistor values on transformer secondary. It currently uses 10k and 1k to scale down by 11. This works for 120Vrms since transformer will output about 6Vp so MCP will get ~600mV. However, if 240Vrms connect to primary coils, 12Vp comes out of secondary meaning MCP will see 1.2Vp which is > 660mV maximum rating.
		DONE

	- Fix silkscreen part numbers and values

	- Fix trace connection to +5V of SPI because it barely touches it 
		DONE
	
	- Get rid of R16 and R15 because they prevent communication from working
		DONE

