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
Jim B. Williams for contributing the needed expert know-how, many ideas and
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
are used in other applications. To quit STAX press F1 - use UP or DOWN to exit
a function menu.

Conversions (F3, CONV) are always made in both directions - that means converting
a<>b results the a-unit in Y and b-unit in X.
DISP (Shift+E) changes the display mode of STAX regarding the displayed precision
or the use of a 'curtain' for less filled stacks.

A stored value (STO, RCL) will be indicated in the status line with 'M'.

STAX supports calculating with complex numbers. To execute the next keypress as
complex operation press COMPLEX (Shift+STO) or simply XEQ. Please note that the
imaginary part (or angle) of a number is located in the Y register of the stack
while the real part (or absolute value) is located in the X register.

In addition STAX provides an useful "Key Recorder" which "plays" recorded key
presses. Record key presses with PRGM (Shift + R/S) and stop recording with PRGM
or R/S. Execute the recorded key presses (up to 50) with R/S.

STAX status line indicators
  M              Value (except 0) stored
  CPX            Execute next operation with complex numbers
  STOP PLAY REC  Key recorder indicator
  X              HEX mode

STAX supports following functions:
  0~9.         Number input
  ENTER        Enter number (lift stack) or duplicate TOS
  + - * /      Basic operation
  BACKSPACE    Clear last entry (while number input) or TOS
  CLEAR        Clear stack and statistics register
  E            Push Y*10^X to the stack
  +/-          Negate TOS (ends number input)
  X<>Y         Swap last stack register
  SUM+ SUM-    Adds/removes data to/from statistics register
  BasicMath    1/X SQRT LOG LN POW SQR 10^X e^X
  STO RCL      Stores TOS or push strored number to stack (store 0 to delete)
  ROT          Rotate last 3 stack elements
  Trig         SIN COS TAN ASIN ACOS ATAN
  COMPLEX XEQ  Execute the next key as complex number operation (see below)
  % PI         Percent, PI
  Shift+XEQ    ln(GAMMA)
  LASTx        Push last ENTERed number to stack
  PRGM R/S     Record key presses or run recorded key presses

  F1 QUIT      Exit STAX
  F2 HYP       Hyperbolic functions
  F3 CONV      Conversions (Polar/rect, hms/h, °C/°F, kg/lbs, cn/in, l/gal)
  F4 STAT      Statisitic/misc functions
               AVG|S ... Mean value, standard deviation
               LRa|b ... Line best fit y=ax+b
               nP|Cr ... Permutations (nPr), Combinations (nCr)
               P|Cdf ... Propability Density (PDF), Cumulative Distribution (CDF)
               ln(!) ... Gamma function
               INT   ... Integer value of TOS
  F5           Physical constant (see below)
  F6 HEX BASE  Toggle HEX and DEC mode

Complex number operations (XEQ + ...):
  UP           Convert to polar coordinates
  DOWN         Convert to rectangular coordinates
  BasicMath    + - * /  1/X SQRT LOG LN POW SQR 10^X e^X
  Trig         SIN COS TAN ASIN ACOS ATAN
  Misc         +/- BACKSPACE ENTER SWAP STO RCL LASTx

Physical constants (F5);
  c    299792458         Speed of light
  g    9.80665           Acceleration of gravity
  G    6.67430e-11       Newton constant of gravity
  Vm   0.02271095464     Molar volume of ideal gas
  NA   6.02214076e23     Avogadro constant
  Rinf 10973731.568160   Rydberg constant
  h    6.62607015e-34    Planck constant
  Phi0 2.067833848e-15   Magnetic flux quantum
  a0   5.29177210903e-11 Bohr radius
  k    1.380649e-23      Boltzmann constant
  R    8.314462618       Molar gas constant
  F    96485.33212       Faraday constant
  t    273.15            Celsius temperature
  atm  101325            Standard atmosphere
  e    1.602176634e-19   Elementary charge
  eps0 8.8541878128e-12  Vacuum electric permittivity
  mu0  1.25663706212e-6  Vacuum magnetic permeability
  Z0   376.730313668     Impedance of vacuum
  mU   1.6605390666e-27  Atomic mass constant
  re   2.8179403262e-15  Electron radius
  me   9.1093837015e-31  Electron mass
  mp   1.67262192369e-27 Proton mass
  mn   1.67492749804e-27 Neutron mass
  mmu  1.883531627e-28   Muon mass
  muB  9.2740100783e-24  Bohr magneton
  muN  5.0507837461e-27  Nuclear magneton
  mue  -9.2847647043e-24 Electron magnetic moment
  mup  1.41060679736e-26 Proton magnetic moment
  mun  -9.6623651e-27    Neutron magnetic moment
  mumu -4.4904483e-26    Muon magnetic moment
  alph 7.2973525693e-3   Fine structure constant
  sigm 5.670374419e-8    Stefan-Boltzmann constant
  G0   7.748091729       Conductance quantum
  gamp 2.6752218744e8    Proton gyromagnetic ratio
  C1   3.741771852e-16   First radiation constant
  C2   1.438776877e-2    Second radiation constant


____________________

 E6B
____________________

The E6B flight computer is a legendary circular slide rule used in aviation.
DESK42 has all capabilities (and more) of E6B for flight planning. The
know-how for this application was contributed by Jim B. Williams. Jim has
logged several thousand hours of flight time over the past 64 years, is a
certified FAA Ground School Instructor and has developed multiple
aviation/navigation spreadsheets for VFR pilots.

The DESK42 E6B application has been created and developed to aid the VFR pilot
with flight planning, take-off, enroute, and landing calculations. Although the
app has been tested extensively and is believed to be bug free, there is always
the possibility of an error in the software. It is therefore recommended that
the pilot double check by other means the critical output data for safety’s
sake. If any error(s) are found, please contact the developer so that the
program can be corrected.

All tools of E6B are ordered in 17 pages (browse with F5, F6 or F4):
  1~4  Dead Reckoning
  5    Distance/Time/Speed or Fuel/Time/FuelBurnRate calculations
  6    Unit conversion for Distance or Speed
  7    Unit conversion for Fuel
  8    Unit conversion for Temperature
  9    Estimated Time of Arrival (ETA) calculation for the flight leg
  10   ZULU time (UTC) conversion of the local time
  11   Traffic Pattern Heading display
  12   Head/Cross Wind (X-Wind) calculations
  13   Distance to Horizon estimation
  14   Pressure Altitude calculation
  15   Density Altitude calculation
  16   True Altitude calculation
  17   True Air Speed (TAS) calculation

Every number input cell can be edited with an RPN calculator (using the routines
and behavior of STAX). That means you can calculate your desired number in the
input cell before committing (UP or DOWN key) it to the E6B calculation. In
addition all numbers on a page can be copied (F2) to the stack an can be used
(pasted) in any other input cell.
To exit/quit E6B to DESK press QUIT (F1).


____________________

 HP-35
____________________

This is the emulation of the legendary HP-35 pocket calculator, that was
introduced by Hewlett-Packard in January 1972.
Much later PeOCter Monta, Jacques Laporte and Pietro de Luca managed to run the
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

