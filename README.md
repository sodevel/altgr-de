# Deutsch (AltGr Akzenttasten)

In the Windows German keyboard layout `Deutsch` the keys `´` (acute accent), `` ` `` (grave accent), `^` (circumflex accent)
are dead keys, this can be cumbersome for certain tasks, e.g. programming. Based on the idea of the
[`United States (International) with AltGr dead keys`](https://github.com/thomasfaingnaert/win-us-intl-altgr) keyboard layout,
in the keyboard layout `Deutsch (AltGr Akzenttasten)` these keys are regular keys by default, they become dead keys only
in combination with `AltGr`. Otherwise, this layout is identical to the keyboard layout `Deutsch`.

## Usage

Install the keyboard layout and add the keyboard `Deutsch (AltGr Akzenttasten)` to your current locale.

## Binary Installation

This is the easiest way, use the latest installer from the [Releases](https://github.com/sodevel/altgr-de/releases) page.

**NOTICE:** The keyboard layout is connected to the German system locale `Deutsch`, if this locale is not present
            on your system, it will get added as well and show up in the language toolbar. If this is not desired,
            you have to compile an own installer from source and connect it to the desired system locale.

## Source Compilation

To compile the keyboard layout source file, you have to install the [Microsoft Keyboard Layout Creator (MSKLC) Version 1.4](https://www.microsoft.com/en-us/download/details.aspx?id=102134).
The keyboard layout source file does not contain a locale definition, hence MSKLC will use the current system locale for the created installer.
Ensure that your system is currently using the desired locale and start MSKLC. Use `File | Load Source File...` and select `altgr-de.klc`.
Create the installer by using `Project | Build DLL and Setup Package`, install the keyboard layout by starting the created `setup.exe`.
