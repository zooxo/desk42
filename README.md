# DESK42 - Spreadsheet, Text, Graphics, Games and More for the DM42

# ... COMING SOON ...


```


DESK42 - Spreadsheet, Text, Graphics, Games and More for the DM42


____________________

 PREAMBLE
____________________

The DM42 calculator is a genuine device. A brilliant LCD display, good keys, a
USB disk and a powerful processor - all low powered by a single battery cell.
On the stable operating system (DMCP) runs Free42 - a perfect simulator of the
legendary HP42 calculator. As the DM42 is an "open system" it is possible to run
other software on top of the operating system (DMCP). And that is, where DESK42
comes in.
DESK42 is an extensive collection of applications that can be started by a
common user interface (DESK). It offers mathematical, text, graphics and useful
assistant applications - and even some games.
Finally a dream became true: The DM42 as essential tool in every cockpit. The
E6B application offers many utilities needed by pilots. Many thanks to
Jim B. Williams for contributing the needed expert knowhow, many ideas and
endless patience when discussing aviation topics with a rookie like me.

Have fun!
deetee



____________________

 INSTALLATION
____________________

Please note that you will loose all user data of your DM42 (ie. user programs or
settings) - make a backup!

Install DESK42:

 * First load DESK42-xxx.pgm and (for desired later back switch to DM42)
   DM42-x.xx.pgm (technical.swissmicros.com/dm42/firmware/) to the root directory
   of the USB disk.
 * In your DM42 calculator goto SETUP (SHIFT-0)
 * Enter menu point [5. System >]
 * Goto system menu with [2. Enter System Menu]
 * Leave DM42 and switch back to the operating system (DMCP) with
   [3. Reset to DMCP menu]
 * Load another program with [3. Load Program]
 * Select the DESK42 program [DESK42-xxx.pgm]
 * [Confirm with ENTER]
 * [Press any key to start]
 * [Press EXIT to continue ...]
 * You are running DESK42 - have fun!

Reinstall DM42:

 * Switch back to the operating system (DMCP) with DESK>OS (F6, F6).
 * Load another program with [3. Load Program]
 * Select the DM42 program [DM42-x.xx.pgm]
 * [Confirm with ENTER]
 * [Press any key to start]
 * [Press EXIT to continue ...]
 * You are running DM42 - thanks for trying DESK42


____________________

 DESK
____________________

DESK is the hub and application launcher. It offers 18 quick keys (1-9 and SHIFT
1-9) to launch selected applications as well as a hierarchical menu system via
function keys for global settings. Finally DESK can exit DESK42 and switch back
to the operating system (DMCP) of the DM42 calculator.


____________________

 STATUS LINE
____________________


____________________

 STAX
____________________

STAX is the standard scientific RPN calculator of DESK42. Many routines of STAX
are used in other applications. To quit STAX press F1 - please note to reset a
function menu with UP or DOWN.
Conversions (F3, CONV) are always made in both directions - that means converting
a<>b results the a-unit in Y and b-unit in X.
DISP (Shift+E) changes the display mode of STAX regarding the displayed precision
or the use of a 'curtain' for small stacks.
A stored value (STO, RCL) will be indicated in the status line with 'M'.

STAX supports following functions:
  0...9.      Number input
  ENTER, R/S  Enter number (lift stack) or duplicate TOS
  + - * /     Basic operation
  BACKSPACE   Clear last entry (while number input) or TOS
  CLEAR       Clear stack and statistics register
  E           Push Y*10^X to the stack
  +/-         Negate TOS (ends number input)
  X<>Y        Swap last stack register
  SUM+ SUM-   Adds/removes data to/from statistics register
  BasicMath   1/X SQRT LOG LN POW SQR 10^X e^X
  STO RCL     Stores TOS or push strored number to stack (store 0 to delete)
  ROT         Rotate last 3 stack elements
  Trig        SIN COS TAN ASIN ACOS ATAN
  COMPLEX     Convert polar to rectangular and back
  % PI        Percent, PI
  XEQ         Integer
  Shift+XEQ   ln(GAMMA)
  LASTx       Push last ENTERed number to stack

  F1 QUIT     Exit STAX
  F2 HYP      Hyperbolic functions
  F3 CONV     Conversions (Polar/rect, hms/h, °C/°F, kg/lbs, cn/in, l/gal)
  F4 STAT     Statisitic/misc functions
              AVG|S ... Mean value, standard deviation
              LRa|b ... Line best fit y=ax+b
              nP|Cr ... Permutations (nPr), Combinations (nCr)
              P|Cdf ... Propability Density (PDF), Cumulative Distribution (CDF)
              ln(!) ... Gamma function
              INT   ... Integer value of TOS
  F6 HEX      Toggle HEX and DEC mode (=BASE, Shift-4)


____________________

 E6B
____________________

The E6B flight computer is a legendary circular slide rule used in aviation.
DESK42 has all capabilities (and more) of E6B for flight planning. The expert
know-how for this application was contributed by Jim B. Williams, an approved
flight engineer. He has logged several thousand hours of flight time over the
past 64 years, is a certified FAA Ground School Instructor and has developed
multiple aviation/navigation spreadsheets for VFR pilots.

All tools of E6B are ordered in 17 pages (browse with F5, F6 or F4):
  1...4 Dead Reckoning
  5     Distance/Time/Speed or Fuel/Time/FuelBurnRate calculations
  6     Unit conversion for Distance or Speed
  7     Unit conversion for Fuel
  8     Unit conversion for Temperature
  9     Estimated Time of Arrival (ETA) calculation for the flight leg
  10    ZULU time (UTC) conversion of the local time
  11    Traffic Pattern Heading display
  12    Head/Cross Wind (X-Wind) calculations
  13    Distance to Horizon estimation
  14    Pressure Altitude calculation
  15    Density Altitude calculation
  16    True Altitude calculation
  17    True Air Speed (TAS) calculation

Every number input cell can be edited with an RPN calculator (using the routines
and behavior of STAX). That means you can calculate your desired number in the
input cell before committing (UP or DOWN key) it to the E6B calculation. In
addition every number on a page can be copied (F2) to the stack an can be used
(pasted) in any other input cell.
To exit/quit E6B to DESK press QUIT (F1).


____________________

 HP-35
____________________

This is the emulation of the legendary HP-35 pocket calculator, that was
introduced by Hewlett-Packard in January 1972.
Much later Peter Monta, Jacques Laporte and Pietro de Luca managed to run the
HP-35-ROM on other platforms. And the footprint of this calculator is incredible
small with 768/1536 words/bytes (ROM) and less than 10 Kilobytes of flash memory
(for the whole calculator application).

Please note that HP-35 doesn't use shifted keys. The SHIFT key is used to toggle
between the (smaller) original full precision display of the top of the stack
and the big 8-digit display. The latter one is complemented with a full
precision top of stack view in an additional status line.
This additional status line also displays an executed stacklift, a stored number
and the use of the recorder (see below) by showing a REC or PLAY sign.

The calculator is complemented by an useful "Key Recorder" which "feeds" the
emulator with key presses. With the SIGMA key the user can start or stop
recording (up to 50) key presses - the XEQ key executes the recorded key press
series.

But there are also many key series prerecorded that can be selected with extra
function keys (use the UP and DOWN keys to switch between different function
keys:
  * Hyperbolic functions (SINH, COSH, TANH and inverse)
  * Additional math functions
    - Polar/Rectangular conversions
    - Present value (interest rate, time periods -> present value)
    - Normal distribution (CDF/PDF)
    - LN! ... ln(gamma()) function (factorial)
    - Quadratic equation (p, q)
  * Unit conversions (length weight, volume, temperature). Please note that
    the conversions are always made in both directions. The X-register always
    display the metric unit and the Y-register the english one (use SWAP key).

Please note that it is not possible to record pre recorded functions.

Original HP35 display and keyboard layout:
     _________________________
    |                         |
    |     -1.234567890-12     |
    |_________________________|
    |                         |
    | X^Y  log  ln   e^X  CLR |
    | SQRT arc  sin  cos  tan |
    | 1/X  X><Y ROT  STO  RCL |
    | E-N-T-E-R CHS  EEX  CLX |
    |   -     7     8     9   |
    |   +     4     5     6   |
    |   *     1     2     3   |
    |   /     0     .     PI  |
    |_________________________|





```

