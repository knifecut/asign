#Calcular la disponibilidad del sistema si tenemos dos réplicas de cada elemento (en total 3 elementos en cada subsistema).

##Ejercicio 1

| Availability % | 1 Component | 2 Components | 3 Components   |
| -------------- | ----------- | ------------ | -------------- |
| Web            |    85,00%   |  97,750000%  |  99.66250000%  |
| Application    |    90,00%   |  99.000000%  |  99.90000000%  |
| Database       |    99.90%   |  99.999900%  |  99.99999999%  |
| DNS            |    98.00%   |  99.960000%  |  99.99920000%  |
| Firewall       |    85.00%   |  97.750000%  |  99.66250000%  |
| Switch         |    99.00%   |  99.900000%  |  99.99990000%  |
| Data Center    |    99.99%   |  99.999999%  | 100.00000000%  |
| ISP            |    95.00%   |  99.750000%  |  99.98750000%  |
| System Avaib.  |    59.87%   |  94.301929%  |  99.21351551%  |

General Case:

As = Acn-1 + ((1 - Acn-1) * Acn)

Example Web:

Web1 	= 85%
Web2 	= 85% + (1-85%) * 85% = 97.75%
Web3 	= 97.75% + (1-97.75%) * 85% = 99.6625%
