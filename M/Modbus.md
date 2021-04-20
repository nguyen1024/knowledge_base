# Modbus

## ...

Instead of an allowed integer range 0-65535, a range -32768 to 32767 is allowed. This is implemented as any received value in the upper range (32768-65535) is interpreted as negative value (in the range -32768 to -1).

Source

* Modbus details
  * https://minimalmodbus.readthedocs.io/en/stable/modbusdetails.html#:~:text=Negative%20numbers%20(INT16%20%3D%20short)&text=Instead%20of%20an%20allowed%20integer,%2D32768%20to%20%2D1).