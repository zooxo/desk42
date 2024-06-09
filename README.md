# DESK42 - Calculator, Spreadsheet, Text, Graphics, Games and More for the DM42

# ... COMING SOON ...

![Desk42_on_Plane](https://github.com/zooxo/desk42/assets/16148023/96ae46b2-377a-499d-bb97-9d65989375ed)
The DM42 running DESK42 (E6B) in action in the cockpit of a Piper Warrior taking off from Brigham City, Utah (BMC) viewing the Wasatch Mountains on left crosswind off of Runway 17.  (© 2024 by Jim Williams)

![desk42](https://github.com/zooxo/desk42/assets/16148023/94213748-9ab6-4633-9bc6-1081f0df63a6)

```

DESK42 - Calculator, Spreadsheet, Text, Graphics, Games and More for the DM42



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

Desk menu:
  DESK  Global settings
        COLOR  Set background color for DESK
        FPS    Set speed (frames per second) for various applications
        KEYin  Set preferred text input mode (see chapter TEXT INPUT MODE)
        Dfmt   Set date format in status line (YMD, MDY, DMY)
        OS     Leave DESK42 to OS (DMCP)
  APP   Menu to launch all possible applications
  SNIP  Perform a screenshot with a delay of 5 seconds (wait for beep)
  INFO  DESK42 info

____________________

 STATUS LINE
____________________

The top line offers information about the system, the running application and
its settings.
The symbol and number at the most right position shows the battery status (where
the number 9 indicates a full battery or a power connection).
The next indicators show date (YYMMDD, MMDDYY or DDMMYY - toggle with DFmt) and
time (in 24 hour format).
The central part of the top line gives you information about the status of the
system (ie shift key or text input method).
The left side of the status line gives you information about the running app
(name, status, indicators).

____________________

 TEXT INPUT METHOD
____________________

When pressing ALPHA (Shift+ENTER) a function key menu pops up to select the
desired text input method (123, ABC, KBD or ASC):
  123  Number keys enter number - other keys like "ABC"
  ABC  Alpha keys (Shift for capital letters)
  KBD  Virtual keyboard (DESK/kbd.txt) in top 3 key rows (Shift QUIT to leave)
  ASC  Select character from ascii table (numpad as cursor, key 5 selects)

Please note that the used text input method will be indicated in the central
part of the status line (1, alpha, keyboard, table).


____________________

 STAX
____________________

STAX is the standard scientific RPN calculator of DESK42. Many routines of STAX
are used in other applications. To quit STAX press F1 - use UP or DOWN to exit
a function menu.

Conversions (F3, CONV) are always made in both directions - that means
converting a<>b results the a-unit in Y and b-unit in X.
DISP (Shift+E) changes the display mode of STAX regarding the displayed
precision or the use of a 'curtain' for less filled stacks.

A stored value (STO, RCL) will be indicated in the status line with 'M'.

STAX supports calculating with complex numbers. To execute the next keypress as
complex operation press COMPLEX (Shift+STO) or simply XEQ. Please note that the
imaginary part (or angle) of a number is located in the Y register of the stack
while the real part (or absolute value) is located in the X register.

STAX provides an useful "Key Recorder" which "plays" recorded key presses.
Record key presses with PRGM (Shift + R/S) and stop recording with PRGM or R/S.
Execute the recorded key presses (up to 50) with R/S.
Additionally finding the root (SOLVER), calculating an integral (INTEGRAL) or
printing a graph (PRINT) is supported (if the recorded keys represent a
function).

STAX status line indicators
  M              Value (except 0) stored
  CPX            Execute next operation with complex numbers
  STOP PLAY REC  Key recorder indicator
  X              HEX mode

STAX supports following functions:
  0~9.         Number input
  ENTER        Enter number (lift stack) or duplicate TOS
  X<>Y         Swap last stack register
  LASTx        Push last ENTERed number to stack
  +/-          Negate TOS (ends number input)
  E            Push Y*10^X to the stack
  BACKSPACE    Clear last entry (while number input) or TOS
  CLEAR        Clear stack and statistics register
  + - * /      Basic operation
  STO RCL      Stores TOS or push strored number to stack (store 0 to delete)
  ROT          Rotate last 3 stack elements
  Trig         SIN COS TAN ASIN ACOS ATAN
  SUM+ SUM-    Adds/removes data to/from statistics register
  BasicMath    % PI 1/X POW SQRT SQR LOG 10^X LN e^X
  COMPLEX XEQ  Execute the next key as complex number operation (see below)
  Shift+XEQ    ln(GAMMA)
  PRGM R/S     Record key presses or run recorded key presses
  SOLVER       Find root of recorded function (preenter a start value)
  INTEGRAL     Integral of recorded function (preenter limits a and b)
  PRINT        Plot a graph (preenter limits a and b) with 100x48 pixel

  F1 QUIT      Exit STAX
  F2 HYP       Hyperbolic functions
  F3 STAT      Statisitic/misc functions
               AVG|S ... Mean value, standard deviation
               LRa|b ... Line best fit y=ax+b
               nP|Cr ... Permutations (nPr), Combinations (nCr)
               P|Cdf ... Propability Density (PDF), Cumulative Distribution (CDF)
               LN(!) ... Gamma function
               INT   ... Integer value of TOS
  F4 CONV      Conversions (Polar/rect, hms/h, °C/°F, kg/lbs, cm/in, l/gal)
  F5           Physical constant (see below)
  F6 HEX BASE  Toggle HEX and DEC mode

Complex number operations (XEQ + ...):
  UP           Convert to polar coordinates
  DOWN         Convert to rectangular coordinates
  BasicMath    + - * /  1/X SQRT LOG LN POW SQR 10^X e^X
  Trig         SIN COS TAN ASIN ACOS ATAN
  Misc         ENTER SWAP +/- BACKSPACE STO RCL LASTx

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

Example: Curve sketching (y=x*x-2)
  * Record function: PRGM (Shift+R/S) x² 2 - R/S
  * Calculate y(5): 5 R/S
  * Calculate (positive) root: 8 (positive start value) SOLVER (Shift+7)
  * Calculate integral between 0 and root: 0 ENTER 2 SQRT INTEGRAL (Shift+8)
  * Plot function between -2 and 2: 2 +/- 2 PRINT (Shift+-)


____________________

 RAX
____________________

RAX is the spreadsheet application of DESK42. When starting RAX you are in the
navigation mode. The number keys work as cursor pad (see below). The navigation
mode is also active when you refer in a formula to a specific cell.

Navigation Numpad/Cursorpad:
  7 Home  8 Up     9 PgUp
  4 Left  5 Enter  6 Right
  1 End   2 Down   3 PgDn

Keys in navigation mode:
  1~9      Navigation - cursor pad
  BSP      Delete cell
  ENTER    Edit selected cell
  STO      Define and edit a new text cell
  CONVERT  (Shift+5) Hardcopy cell value

  F1       QUIT RAX
  F2       FILE operation (New, Open, Save, SaveAs)
  F3 F4    COPY and PASTE the selected cell
  F5 F6    Change displayed spreadsheet format

Keys in edit mode (ENTER to select and quit):
  F1       QUIT edit mode
  F2 OP    Spreadsheet operations
     GET   References (REF/RCL, IND) regular or indirect (push col and row)
     STACK Stack operations (CLR, DROP, ENTER, RCL)
     STAT  Functions with referenced areas (COUNT, SUM, MIN/MAX, AVG, LRa|b)
     COND  Conditions (IF, ELSE, THEN, <, =, >)
     INF   Infinitesimal operations (MIN/MAX/PLOT, SLOPE, SOLVE, INT, DEQ))
  F3 FN    (STAX) Functions (HYP, STAT, CONV, CONST, MAT) ... see STAX
  F5/F6    Cursor left/right
  BSP      Clear command left to cursor
  CLEAR    Clear complete formula
  RCL      Reference
  R/S      Separate numbers (enter)

Matrix funktions (MAT):
    DET   Determinant (from)
    TRANS Transpose (from, to)
    INV   Inverse (from, to)
    MULT  Multiply (from1, from2, to)
    SUB   Substract (from1, from2, to)
    ADD   Add (from1, from2, to)
  Please note that RAX deals with 3x3 matrices only - smaller matrices can be
  a subset.
  A reference to a matrix references to the first matrix cell [1|1].
  Matrix functions that create a new matrix write 3x3 (hard coded) values to
  the spreadsheet at the target cell (to) if there is sufficient room on the
  spreadsheet. Please be careful using these commands without a target cell to
  not overwrite existing contents of the spreadsheet.
  Please note that all matrix functions leave the determinant value on the stack.

Indirect references (IND) refer to row and column number from the stack.
A condition (< = >) compares two stack values - returns 1 (true) or 0 (false)
Due to FORTH a conditional function consists of:
  <condition> IF <true-branch> ELSE(optional) <false-branch> THEN
MIN/MAX/PLOT pushes minimal and maximal plot values to the stack and plots the
function when leaving the edit mode (ENTER).
The INF functions evaluate a cell containing a function (REF to function)
which depends itself to a referenced cell (REF to x). In some cases additional
REFerences are required (ie x-value-range).
DEQ solves a differential equation (REF to function, x, y, x-target) y'=f(x,y)
with given start value y(x0) due to Runge-Kutta with 4th order (RK4). DEQ
calculates the solution function (y value for the targeted x).


____________________

 FLEX
____________________

The calculator FLEX has the look and feel of STAX, but actually calculates
with the (first) cells of a RAX spreadsheet. Hence you can see and (with XEQ
or STACK>EDIT) edit the formula that yields the result.

Please note that numbers without a terminating ENTER (after using SWAP or ROT)
will be treated as not closed numbers (ie "2 ENTER 1 SWAP +" yields 24 =12*2).
Please note that DISP (Shift+E) toggles the display format.
Please note that leaving FLEX always clears all variables.


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
  0    Table of pages (9 fast keys to E6B categories)
  1    Dead Reckoning 1: Select route input (page 2) and desired units
  2    Dead Reckoning 2: Insert coordinates or course/distance
       Latitude/Longitude repectively True Course and Distance
  3    Dead Reckoning 3: Insert other data
       Magnetic Variation, True Air Speed, Fuel Burn Rate,
       Wind Direction and Wind Velocity
  4    Dead Reckoning 4: Results
       Magnetic Heading, Distance, Ground Speed, Leg Time and Leg Fuel
  5    Estimated Time of Arrival (ETA) calculation for the flight leg
       Init/Start Time, Leg Time, ETA
  6    ZULU Time (UTC) Conversion of Local Time
       Init/Start Time, Time Zone (main airport of time zone, keys 4 or 6)
  7    Temperature Conversion
       Fahrenheit, Celsius, Kelvin
  8    Pressure Altitude Calculation
       Airport Elevation, Altimeter Settings (Hg), Pressure Altitude
  9    Density Altitude Calculation
       Pressure Altitude, OAT (Outside Air Temperature), Density Altitude
  10   True Altitude Calculation
       OAT (Outside Air Temperature), Pressure Altitude, Indicated Altitude,
       Ground Station Altitude, Corrected Altitude
  11   True Air Speed (TAS) Calculation
       Pressure Altitude, OAT (Outside Air Temperature),
       IAS (Indicated Airspeed), TAS (True Air Speed)
  12   Distance to Horizon Estimation
       AGL (Above Ground Level) Altitude
  13   Traffic Pattern Heading
       Runway Number, Entry, Down Wind, Base, Finial
  14   Head/Cross Wind (X-Wind) Calculations
       Runway Number, Wind Direction, Wind Velocity, Head/Tail Wind, Cross Wind
  15   Unit Conversion for Fuel
       Imperial Gallons, US Gallons, Litres
  16   Unit Conversion for Distance or Speed
       Distance (Nautical Miles, Statute Miles, Kilometres)
       Speed (Knots, Miles per Hour, Kilometres per Hour)
  17   Distance/Time/Speed or Fuel/Time/FuelBurnRate calculations

Every number input cell can be edited with an RPN calculator (using the routines
and behavior of STAX). That means you can calculate your desired number in the
input cell before committing it to the E6B calculation (UP or DOWN key). In
addition all numbers on a page can be copied (F2) to the stack an can be used
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


____________________

 TEX
____________________

TEX is a simple text editor. It offers 2 font sizes (F4) and indicates text size
(status line) and current text line (meter bar). Navigation can be done with the
UP/DOWN/F5/F6 keys - with SHIFT PgUp/PdDown/Home/End will be performed.
Backspace deletes a character - SHIFT-Backspace deletes the current line.
Please note that there are restrictions to file size (4096 bytes) and characters
per line (128).


```

