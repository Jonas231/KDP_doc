INTRO-GENERAL INFORMATION
=========================
INTRO-GENERAL INFORMATION - This program is an advanced, interactive
optical design and analysis program. It is used in the design and
analysis of all forms of optical systems. All titles and some data in
tables are shown in BOLD BLUE. The entire text is 9pt. Times New Roman.

INSTALLATION   - For information concerning installation on your
computer, please refer to the installation instructions provided
separately.

GETTING STARTED - This manual is the "PROGRAM REFERENCE MANUAL"
accessible from the program Help menu. It completely describes all
features and commands. There are two separate "TUTORIAL" manuals, also
available in PDF form from the Help menu. There are also "prompting"
guides available in the program HELP menu.

CASE SENSITIVITY - All program textual command input is case
insensitive. Input may be in upper or lower case. All input is converted
to upper case before it is processed. The basic input mode of this
program is textual. Menus are provided for the more commonly used
features.

COMMANDS - All program commands and some command-like auxilliary words
are  indicated in this manual in BOLD RED text.

EXAMPLES  - All program examples are indicated in this manual in BOLD
GREEN text.

GRAPHICAL USER INTERFACE  -  The program Graphical User Interface is
intended to be used by both new users and experienced users, occasional
users and regular users, amatuer users and professional users. It
provides a powerful sub-set of the command driven capabilities of the
program in an intuitive format. It is not intended as a replacement for
the command interface and certainly is not a replacement for the macro
and scripting capabilities inherent in the command interface. The user
is wise to enjoy the GUI and as the occasion permits, explore the
command interface. Switching between the two interfaces is as simple as
moving the cursor to the command line at the bottom of the main program
window and issuing a command followed by the ENTER key.

USER INTERFACE  - After installation, a shortcut to the program icon can
be made and placed on DESKTOP. When it is double clicked, the program
loads and begins to run. The user will see the program output window,
below which appears a one line "command box" with a command history
option via mouse or up and down arrow keys. All typed input to the
program is enetered in that input box. All textual output, which is
intended to be displayed to the screen, will be placed in the main
output window. This output window automatically scrolls as more and more
output is placed in it. At any time, output may be selected with the
mouse or by use of the "select all" menu option and copied into the
CLIPBOARD or printed. The output window scrolling capacity is only
limited by computer memory. The output window history can be cleared at
any time issuing the "CLS" command. The selection of some of the menu
items causes various program documentation documents to be opened and
displayed using Adobe Acrobat Reader. There are command prompting
guides, a tutorial, a reference manual and a list of new features in
each previous program release dating back to version 4.00in the HELP
menu. Hardcopy text output is performed either by copying text from the
output window and pasting it into a word processor or by using the
"OUTPUT LP" and "PRINT" commands described in the CMD section of this
manual. (the "OUTPUT LP" and "PRINT" commands are only available in the
distribution of the program which is under full user support). All
others will need to copy and paste using the CLIPBOARD.  Text output may
also be printed using the “PRINT” option in the File Menu.Whenever a
command generates screen graphics, those graphics are displayed in a
separate window. This window may be moved, re-sized, minimized,
maximized or copied into the CLIPBOARD using standard windows
techniques. Graphics hardcopy  and file output is available via the
"GRAOUT" command described in the GRAPHICS section of  this manual.

PROGRAM CAPACITIES  - The fully supported version of the program,
supports lens databases of up to 500 surfaces, 999 macros, each of which
may have 1024 macro lines, and 75 alternate lens configurations. These
limits can easily be extended should the user require greater capacity.

PROGRAM ORGANIZATION  - This program has a command-driven user
interface. This choice of interface provides maximum user freedom, speed
and control over program execution. Some of the more common program
operations are supported in the GUI interface. Program commands may be
issued and executed in an immediate interactive mode from the keyboard,
they may be strung together in an input data file and read from within
the running program or they may be composed into internal macro programs
using the built-in macro programming language and editor. Macros can be
stored on disk and executed from within the running program at any time.
Macro programs (macros and macro functions) can call other macro
programs in nests up to 20 levels deep. Once created, these macros look
and feel exactly like hard coded program commands. There are also
special macro specific commands which enable a macro to be much more
than just a string of program commands. Full details are given in the
MACRO section of this manual.

--------------

ORGANIZATION OF COMMAND INPUT  - Program command input is performed
through a succession of text commands, each of which may consist of up
to 140 characters, including blanks. All program commands will have one
of the following formats:

1)        Command Word

2)        Command Word + Qualifier Word

3)        Command Word + Alphanumeric String

4)        Command Word + Qualifier Word + Alphanumeric String

5)        Command Word + from 1 to 5 Numeric Words

6)        Command Word + from 1 to 5 Numeric Word + Alphanumeric String

7)        Command Word + Qualifier Word + from 1 to 5 Numeric Words

8)        Command Word + Qualifier Word + from 1 to 5 Numeric Words +
Alphanumeric String

9)        Command Word + ? (special interrogator character)

10)        Command Word + Qualifier Word + ? (special interrogator
character)

All  commands MUST ALWAYS begin with a COMMAND WORD.

COMMAND AND QUALIFIER WORDS  - Command and qualifier words may consist
of up to eight alphanumeric or other special characters, except the
characters ";" and ",". The use of  ";" will be covered later. The comma
"," and the blank " " are used as special command delimiters and may not
be part of the input, except when they appear as part of an alphanumeric
string once that string has begun. The command word is always the first
entry on a command line.  Macro names follow the same rules as command
words, being limited to 8 characters. The command words and qualifier
words may begin with any allowed character. The qualifier word, if
specified, always follows a command word. The first character in a
command word, qualifier word or macro name may not be a digit (0 through
9), a plus "+" or minus "-" sign, a question mark "?" or a decimal point
".". Leading blanks are discarded.

NUMERIC WORDS (NUMERIC INPUT - Up to five numeric words may be used in a
single program command, though many commands do not use all five words.
Each numeric word may be represented by no more than 23 characters,
including a decimal point and an "E" or "D" representing exponential
notation. Input is otherwise free format. All numeric words are stored
internally in double precision. Numeric data is held internally and
transferred in a D23.15 format whenever it is written to or read from
disk in an ASCII format. If explicit exponential notation is not used, a
plus or minus sign can be used to indicate the start of an exponent. If
exponential notation is used, a plus sign is optional. A blank following
a "D" or "E" is treated as a plus sign. The exponent may contain one to
three digits but must not have a magnitude greater than 300. A decimal
point may occur anywhere prior to the start of an exponent. In the
absence of a decimal point, an implied decimal point is understood to
follow the rightmost digit before the exponent. Leading plus signs are
optional.

SPECIAL CHARACTER (" ; ")  - The semicolon " ; " character is used as a
virtual carriage return. It allows for up to 20 program commands to be
issued per 140-character input line. This character can be issued from
any program level, including from within the macro editor. It is
ALWAYS executed immediately. The semicolon is not available as part of
string input. Use a comma instead.

THE ALPHANUMERIC STRING  - Alphanumeric string input can consist of up
to eighty (80) alphanumeric or special characters, excluding ";".
Alphanumeric strings may be input as upper or lower case. In the case of
the comment and message commands ("C" and "M"), the case of the input is
remembered. For all other program commands, program input is
automatically converted to upper case before being processed by the main
program input parser.

SEPARATORS  - A command word and a qualifier word may be separated from
one another by one to eight blank spaces. A command word or a command
word/qualifier word pair may be separated from the first numeric word by
either one to eight blank spaces, a comma or a comma and one to eight
blank spaces. Default numeric input is always indicated by no numeric
input word or by a succession of commas. The formal rule for separating
a command word or a command word/qualifier word combination from a
following alphanumeric string is to use a blank space or a comma
following the command word or command word/qualifier word pair. This
space or comma is then followed by the alphanumeric string. The result
of using ,, to specify default input varies from command to command.

COMMAND EXAMPLES

1) WRITE - (Command Word)

2) WRITE ALL - (Command Word + Qualifier Word)

3) SET , 25.4 - (Command Word + Numeric Word #1)

4) SET A 25.4 - (Command Word + Qualifier Word + Numeric Word #1)

5) M, THE ANSWER IS WRONG - (Command Word + Alphanumeric String)

6) NSUB DV , 12.3 , 4.5 , 6.0,,, - (Command Word + Qualifier Word +
Numeric Input with default values for numeric words 4 and 5)

COMMAND DESCRIPTIONS  - Program commands are always shown in upper case.
Each command is presented in a command shadowed box followed by a
complete description of that command, its use and its effects. In a
textual reference, commands are delimited by double quotation marks. For
example, the command which lists all of the surface data in the current
lens would be denoted in text by "RTG ALL". Minimum use of command
shorthand will be used in this manual to denote required versus optional
input. If a particular input to a command is optional, that fact is
simply stated in the description which follows the command box. An
attempt has been made to write this manual in simple, plain Engish.

--------------

PROGRAM PROMPT - When operating in the command interface mode,the
program screen prompt is a three-character string followed by a colon
":". At this prompt, commands may be typed in followed by the press of
the <ENTER> key. The three-character string preceding the colon
indicates the current program level. The program levels corresponding to
the various prompts are listed in the following table.

======================= =============================
PROMPT CHARACTER STRING PROGRAM LEVEL
CMD                     MAIN or COMMAND
SPE                     SPECTRAL ANALYSIS
MAC                     MACRO INPUT
MED                     MACRO EDIT (MEDIT)
LEN                     LENS INPUT
ULN                     LENS UPDATE
SPS                     SPECIAL SURFACE (SPSRF)
USP                     UPDATE SPECIAL SURFACE
FIT                     SPECIAL FUNCTION FITTING
CFG                     CONFIGS INPUT
UCF                     UPDATE CONFIGS
MER                     MERIT FUNTION INPUT
UMR                     UPDATE MERIT FUNCTION
VAR                     VARIABLES INPUT
UVB                     UPDATE VARIABLES
TVB                     TOLERANCE VARIABLES INPUT
UTV                     UPDATE TOLERANCE VARIABLES
CMP                     COMPENSATION VARIABLES INPUT
UCP                     COMPENSATION VARIABLES UPDATE
TOP                     TOLERANCE OPERAND INPUT
UTP                     TOLERANCE OPERAND UPDATE
FOC                     FOCRIT (FOCUS CRITERIA) INPUT
UFC                     FOCRIT UPDATE
======================= =============================

PROGRAM ORGANIZATIONAL STRUCTURE  - The organizational structure of the
program is conceptually very simple. When the program begins running, a
prompt symbol will be displayed on the computer screen. At this prompt,
you enter a program command and press the <RETURN> or <ENTER> key on the
keyboard. Depending on the nature of the command issued, some action
will be taken by the program. This action may or may not result in
output. When the program begins, it is always at the CMD level. This is
the main, or top, level of the program. Beneath this level are
sub-levels which are used to manage the lens data, optimization files,
tolerancing, macro programming, etc. The organizational flow of the
program is best understood by examining the figure below. Solid lines
represent paths along which the user travels while using the program.
Dashed lines represent internal automatic data flow during program
operation.

--------------

Program Road Map

PROGRAM DISK DIRECTORY STRUCTURE  - During the program installation
process, the root or main directory is created on the target disk drive.
A default root directory name is supplied if you do not specify one.
Several sub-directories are created beneath the main directory. These
directories house the following classes of files:

+----------------------------------+----------------------------------+
| DIRECTORY NAME                   | FILE CLASSES STORED              |
+----------------------------------+----------------------------------+
| \\LIBSPO                         | All the files associated with    |
|                                  | ray spot diagrams.               |
+----------------------------------+----------------------------------+
| \\LIBAUT                         | All the files associated with    |
|                                  | the optimization process.        |
+----------------------------------+----------------------------------+
| \\LIBGLA                         | All of the optical material      |
|                                  | glass catalogs are stored here   |
|                                  | in binary and ASCII format.      |
|                                  | Located here are the .EXE files  |
|                                  | which rebuild a binary glass     |
|                                  | catalog file from the ASCII      |
|                                  | version. This allows the user to |
|                                  | update the glass catalogs. The   |
|                                  | procedure for doing this update  |
|                                  | is described in the file         |
|                                  | GLAUP.DOC which is also stored   |
|                                  | in this directory.               |
+----------------------------------+----------------------------------+
| \\LIBLxx (These are the          | All the files associated with    |
| directory names of the           | the lens manufacturer lenses are |
| manufacturer lens libraries.)    | stored in these directories.     |
+----------------------------------+----------------------------------+

--------------

PROGRAM FILES  - The following files are stored in the main program
directory or in one of its sub-directories:

+----------------------+----------------------------------------------+
| PRINTER.TXT          | Printer file created by the program.         |
+----------------------+----------------------------------------------+
| PUNCHFILE.DAT        | Auxiliary data transfer file created by the  |
|                      | program.                                     |
+----------------------+----------------------------------------------+
| CARDTEXT.DAT         | Auxiliary data transfer file created by the  |
|                      | program.                                     |
+----------------------+----------------------------------------------+
| EDITTEXT.DAT         | Editor file used with a DOS editor and the   |
|                      | "EDIT" command.                              |
+----------------------+----------------------------------------------+
| DEFAULTS.DAT         | A user-created file containing program       |
|                      | commands which the user wishes to run        |
|                      | automatically when the program starts. The   |
|                      | commands included in the default version of  |
|                      | this file are: "OUT TP" and "IN TP" .        |
+----------------------+----------------------------------------------+
| TAB.DAT              | Table Writer file                            |
+----------------------+----------------------------------------------+
| DATA.DAT             | Functional fitting data file                 |
+----------------------+----------------------------------------------+
| SPD.DAT, LSF.DAT     | MTF, Line Spread Function files              |
+----------------------+----------------------------------------------+
| RAYS.DAT, FIELDS.DAT | Field and ray definition files               |
+----------------------+----------------------------------------------+
| AUTO.DAT, AUTO2.DAT  | Optimization save files                      |
+----------------------+----------------------------------------------+
| OPDDAT.DAT           | OPD fitting files                            |
+----------------------+----------------------------------------------+
| APMAP.DAT            | Pupil apodization file                       |
+----------------------+----------------------------------------------+
| FOOT1.DAT            | Beam footprint file                          |
+----------------------+----------------------------------------------+

BATCH MODE OPERATION  - The program is primarily intended to be used in
an interactive setting. There are; however, situations where the program
may need to be run in a BATCH mode. To do this, prepare an ASCII file
named BATCH.DAT which contains all of the program commands which are to
be executed. Place it in the main program directory. Include an "EXIT"
statement as the last entry in this file. Next, either type "PRG BATCH"
at the DOS command prompt or at the RUN line. The program will execute
all of the commands in the BATCH.DAT file.

THE PROGRAM AS A SUBROUTINE  - In some special situations, the program
may be available as a callable subroutine. If you don't have the program
in that form, then you probably are not going to get the program in that
form. When the program is callable as a subroutine, all screen input and
output operations are turned off. Graphics output is limited in that no
program manipulation of the NEUTRAL.DAT file is possible via the VIE and
GRAOUT commands. No operating system commands can be executed in this
mode from inside the program. All such actions are to be programmed by
the user in non-program related subroutines. When the program is run as
a subroutine, it automatically runs in the above described BATCH mode.

OPTICAL DEFINITIONS - The following section has been asked for by
several users. It is intended to provide a short review of the "optical
definitions" assumed by the program.

Local Optical Axes  - The program assumes, at the origin or "vertex" of
every surface in a lens prescription, that there exists a right handed
rectangular "local" coordinate system. In the absence of surface tilts
and decentrations, the positive local Z-axis is perpendicular to the
surface and points to the right. The positive Y-axis is "up" and the
positive X-axis is "into" the page or screen.

Sequential Database  - The pth of rays traced through lens database
sequential. From surface 0, "the object surface" to "surface 1" to
"surface 2" and to each next surface and then to the final surface in
the database. The relative positions of each surface may be established
in either a "local" sense or a "global" sense. Most of the time, the
"local" sense is the easiest way to establish these relationships. In
the "local" sense, surface 1 is positioned relative to surface 0,
surface 2 relative to surface 1 and so on. The relative position of a
"following" surface is established with a "thickness" or TH
specification and by decentration and surface tilt commands relative to
the previous surface.

Surface Tilts  - A following surface may be reoriented with repect to
the previous surface by assigning surface tilts. When this is done, the
order in which the tilts are applied is generally ALPHA (about the
X-axis), then BETA about the new Y-axis and then GAMMA about the new
Z-axis. There are exceptions. The angular sign conventions are such that
ALPHA and BETA are left-handed positive and GAMMA is right-handed
positive. Figures illustrating these conventions can be found in the
Lens Database section of this manual This sign convention agrees with
CODE-V and ACCOS-V. In ZEMAX, the ALPHA and BETA sign conventions are
right-handed positive.

Paraxial Optical Axis  - Paraxial optical ray tracing is the result of a
linearization of the trigonometric ray tracing equations in which the
SINE and TANGENT of all angles is replace by their angular value in
radians and the COSINE is replace by 1.0. The paraxial ray trace ignores
surface decentrations and tilts. The paraxial optical axis therefore
passes through the center of all lens database surfaces.

--------------

Real Optical Axis  - The real optical axis has more than one definition
depending upon program ray trace settings.

If real ray aiming is turned off with the AIMRAY OFF command (not the
default condition), then the real ray optical axis is defined by the
path of the ray which originates at the center of the object surface
(generally surface 0) and passes through the center of surface 1. The
path of this ray, through the rest of the surfaces is considered to be
the "gut ray" and defines the optical axis of the system.

If real ray aiming is turned on with the AIMRAY ON command (the default
condition), then:

If there is no clear aperture assigned to the "reference surface", the
real optical axis is defined by the path of the ray which originates at
the center of the object surface (generally surface 0) and passes
through the center of the "reference surface". The ray is iteratively
aimed during this process. The path of this ray, through the rest of the
surfaces is considered to be the "gut ray" and defines the optical axis
of the system. The reference surface (see the REFS command) may be
assigned to be any surface betweem the object surface and the image
surface. In almost all cases, it should be the same surface defined to
be the aperture stop (see the ASTOP command).

If there is a clear aperture assigned to the "reference surface", the
real optical axis is defined by the path of the ray which originates at
the center of the object surface (generally surface 0) and passes
through the center of the clear aperture assigned to the "reference
surface". The ray is iteratively aimed during this process. This clear
aperture may even be decentered and tilted and the ray will still go
through the center of the clear aperture. The path of this ray, through
the rest of the surfaces is considered to be the "gut ray" and defines
the optical axis of the system. The reference surface (see the REFS
command) may be assigned to be any surface betweem the object surface
and the image surface. In almost all cases, it should be the same
surface defined to be the aperture stop (see the ASTOP command).

Real Ray Trace  - Real single trigonometric rays are traced with the
paradigm of reference object heights (or angles) and reference aperture
heights (see the SCY, SCX, SAY and SAX commands). These are single X and
Y values are stored with the lens. To specify a location in the object
surface from which rays originate, the FOB (Fractional OBject height)
command is used to establish a starting point relative to the reference
object height (or angle) values. FOB input values may be of any value
and are not limited to lie betweem -1 and 1. The RAY command is then
used to specify the relative position in the reference surface, vie the
reference aperture heights through which a ray will pass (if ray aiming
is on) or the relative position in surface 1 if ray aiming is off.

Reflections  - Every time a ray strikes and interacts with a reflector,
the ray's local n-direction cosine is essentially reversed and the sign
of the refractive index is reversed. This is common practice in all
optical design programs.

.. container::
