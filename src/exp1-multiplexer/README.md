# Multiplexer

Multiplexing is the generic term used to describe the operation of sending one or more analogue or digital signals over a common transmission line at different times or speeds and as such, the device we use to do just that is called a Multiplexer.

![Multiplexer](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_multiplexer.png)


## Add Circuit

![Add Circuit](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_add_circuit.png)

## Place Gates

First place four `AND Gate`s, set `Number Of Inputs` to `2`, then label them from `U1` to `U4`. Then place a `NOT Gate`, label it `U5`. Finally place two `OR Gate`s, set `Number Of Inputs` to `2`, then label them `U6` and `U7`. To make it more beautiful, I set `Gate Size` to `Narrow`.

![Place Gates](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_place_gates.png)

## Add Terminals

Add five inputs and two outputs.

![Add Terminals](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_add_terminals.png)

## Connection

Use line to connect them, set label for all terminals.

![Connection](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_connection.png)

## Test

Now we can test the circuit, set `A` to `00`, `B` to `11` and `S` to `1`, the result is shown on the following image.

![Test](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_test.png)


|No|A|B|S|Z(expect)|Z(actual)|
|-|-|-|-|-|-|
|1|00|01|1|01|01|
|2|00|10|1|10|10|
|3|00|11|1|11|11|
|4|01|00|0|01|01|
|5|10|00|0|10|10|
|6|11|00|0|11|11|

So the expect == actual, test has successfully been done.

## Edit Circuit Appearence

Right click `mux2`, then left click `Edit Circuit Appearence`.

![Edit Circuit Appearence](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_edit_circuit_appearence.png)


## Use `mux2`

After packaging `mux2`, we can use it in other circuit.

![Use mux2](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_use_mux2.png)

We can use two 2-bit `mux2` to make a 4-bit `mux2`.

![mux2 4bit](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_mux2_4bit.png)


# Comparator

After learning how to package circuit, I try to make a comparator, like the picture follows:

![Comparator Demo](https://cdn.jsdelivr.net/gh/mmdjiji/logisim-learning@main/assets/exp1_comparator_demo.png)

I did four model, see source here:

* [parallel_signed_4-bit_comparator](parallel_signed_4-bit_comparator.circ)
* [parallel_unsigned_4-bit_comparator](parallel_unsigned_4-bit_comparator.circ)
* [serial_signed_4-bit_comparator](serial_signed_4-bit_comparator.circ)
* [serial_unsigned_4-bit_comparator](serial_unsigned_4-bit_comparator.circ)
