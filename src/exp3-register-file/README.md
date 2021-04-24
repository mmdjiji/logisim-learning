# Register File

A register file is an array of processor registers in a central processing unit (CPU). Modern integrated circuit-based register files are usually implemented by way of fast static RAMs with multiple ports. Such RAMs are distinguished by having dedicated read and write ports, whereas ordinary multiported SRAMs will usually read and write through the same ports.

![Register File](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp3_register_file.png)

|Interface|Function|
|-|-|
|we|Register write enable|
|ra|Read the register number of port a|
|rb|Read the register number of port b|
|rd|Write port data|
|rw|Write port register number|
|qa|Read the data of port a|
|qb|Read the data of port b|

## The circuit

![The Circuit](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp3_the_circuit.png)


## Test

|No|Function|we|rw|rd|ra|rb|qa|qb|
|-|-|-|-|-|-|-|-|-|
|1|Write R4 to 04H|1|100|00000100|000|000|00000000|00000000|
|2|Write R5 to 05H|1|101|00000101|000|000|00000000|00000000|
|3|Read R4 to port a|0|000|00000000|100|000|00000100|00000000|
|4|Read R5 to port b|0|000|00000000|000|001|00000000|00000101|


## Add Reset

![Add Reset](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp3_add_reset.png)
