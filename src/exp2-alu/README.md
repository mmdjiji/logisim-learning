# ALU

ALU (arithmetic logic unit) is a combinational digital circuit that performs arithmetic and bitwise operations on integer binary numbers.

![ALU](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp2_alu.png)

## Definition

### Inputs

|Field|Description|
|-|-|
|Number A|An 32-bit number|
|Number B|An 32-bit number|
|aluc|Control Signal|

### Outputs
|Field|Description|
|-|-|
|alu_out|Result|
|zero|Zero Flag (ZF)|
|over|Over Flag (OF)|

### The `aluc` field
|aluc|Operation|
|-|-|
|000|Addition|
|001|Subtraction|
|010|Or|
|011|And|


## The Circuit

![The Circuit](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp2_the_circuit.png)

## Test

|No.|Operation|A|B|cin_add/cin_sub|aluc|zero|over|alu_out|
|-|-|-|-|-|-|-|-|-|
|1|A+B|AAAA5555|5555AAAA|0|000|0|0|FFFFFFFF|
|2|A+B|AAAA5555|5555AAAA|1|000|1|0|00000000|
|3|A-B|AAAA5555|5555AAAA|0|001|0|1|5554AAAB|
|4|A-B|AAAA5555|5555AAAA|1|001|0|1|5554AAAA|
|5|A or B|AAAA5555|5555AAAA|-|010|0|0|FFFFFFFF|
|6|A and B|AAAA5555|5555AAAA|-|011|1|0|00000000|
