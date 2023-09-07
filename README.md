---
license: The Base 42 by η Δεμερζελ is licensed under a Creative Commons Attribution 4.0 International License. You should have received a copy of the license along with this work. If not, see http://creativecommons.org/licenses/by/4.0/.
status: WIP
---
# The Base 42
## An encoding/decoding proposal for bit strings of an arbitrary length and online streams of bits

Here we propose the following Number System to encode binary data:

|Base 10 number  |ASCII characters |Base 42 digit  |Unicode code pages |       bits[^bits]|notes  |
|----------------|-----------------|---------------|-------------------|------------------|-------|
|0               |0                |0              |U+0030             |                 0|       |
|1               |1                |1              |U+0031             |                 1|       |
|2               |2                |2              |U+0032             |                10|       |
|3               |3                |3              |U+0033             |                11|       |
|4               |4                |4              |U+0034             |               100|       |
|5               |5                |5              |U+0035             |               101|       |
|6               |6                |6              |U+0036             |               110|       |
|7               |7                |7              |U+0037             |               111|       |
|8               |8                |8              |U+0038             |              1000|       |
|9               |9                |9              |U+0039             |              1001|       |
|10              |A, a             |A              |U+0041, U+0061     |              1010|       |
|11              |B, b             |B              |U+0042, U+0062     |              1011|       |
|12              |C, c             |C              |U+0043, U+0063     |              1100|       |
|13              |D, d             |D              |U+0044, U+0064     |              1101|       |
|14              |E, e             |E              |U+0045, U+0065     |              1110|       |
|15              |F, f             |F              |U+0046, U+0066     |              1111|       |
|16              |G, g             |G              |U+0047, U+0067     |             10000|       |
|17              |H, h             |H              |U+0048, U+0068     |             10001|       |
|18              |   i             |i              |        U+0069     |             10010| [^1]  |
|19              |J, j             |J              |U+004A, U+006A     |             10011|       |
|20              |K, k             |K              |U+004B, U+006B     |             10100|       |
|21              |L                |L              |U+004C             |             10101| [^2]  |
|22              |M, m             |M              |U+004D, U+006D     |             10110|       |
|23              |N, n             |N              |U+004E, U+006E     |             10111|       |
|24              |   o             |o              |U+004F, U+006F     |             11000| [^3]  |
|25              |P, p             |P              |U+0050, U+0070     |             11001|       |
|26              |Q, q             |Q              |U+0051, U+0071     |             11010|       |
|27              |R, r             |R              |U+0052, U+0072     |             11011|       |
|28              |S, s             |S              |U+0053, U+0073     |             11100|       |
|29              |T, t             |T              |U+0054, U+0074     |             11101|       |
|30              |U, u             |U              |U+0055, U+0075     |             11110|       |
|31              |V, v             |V              |U+0056, U+0076     |             11111|       |
|32              |W, w             |W              |U+0057, U+0077     |             11111|       |
|33              |X, x             |X              |U+0057, U+0077     |            100000|       |
|34              |Y, y             |Y              |U+0058, U+0078     |            100001|       |
|35              |Z, z             |Z              |U+0059, U+0079     |            100010|       |
|36              |&#x0060;         |&#x0060;       |U+0060             |            100011| [^TBD]|
|37              |&#x007C;         |&#x007C;       |U+007C             |            100100| [^TBD]|
|38              |-                |-              |U+002D             |            100101| [^TBD]|
|39              |.                |.              |U+002E             |            100110| [^TBD]|
|40              |_                |_              |U+005F             |            100111| [^TBD]|
|41              |~                |~              |U+007E             |            101000| [^TBD]|

---
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons Licence" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.

[^1]: [LATIN CAPITAL LETTER I][U+0049] in some fonts may be confused with [DIGIT ONE][U+0031];
[^2]: [LATIN SMALL LETTER L][U+006C] in some some fonts may be confused with [DIGIT ONE][U+0031];
[^3]: [LATIN CAPITAL LETTER O][U+004F] in some fonts may be confused with [DIGIT ZERO][U+0030];
[^bits]: leftmost bit is the first bit in the string or stream, rightmost — the last;
[^TBD]: it is desired that symbols here do not interfere with formatting in popular data transfer formats like yaml, json, xml

[Unicode Basic Latin ASCII]: https://unicode.org/charts/PDF/U0000.pdf
[U+0030]: https://symbl.cc/en/0030/
[U+0031]: https://symbl.cc/en/0031/
[U+0049]: https://symbl.cc/en/0049/
[U+006C]: https://symbl.cc/en/006C/
[U+004F]: https://symbl.cc/en/004F/
