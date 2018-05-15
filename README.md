# PS4API 5.01 Server

This project allows you to control PS4 game memory for reading/writing calls.
with this project you can make RTE/RTM tools


## How To Build

use [XVortex SDK](https://github.com/xvortex/ps4-payload-sdk) to compile payload.

## Usage

char sendCommand(char command, void* args);

commands:
    * 'a' attach to game process ( eboot.bin ) and the process will continued.
    * 'c' continue the process.
    * 'd' detach the process.
    * 's' suspend the process.
    * 'u' resume the process.
    * 'k' kill the process (seems not works)
    * 'n' send notification with text.
    * 'r' read memory.
    * 'w' write memory.

args:

    * 'a'(void);
    * 'c'(void);
    * 'd'(void);
    * 's'(void);
    * 'u'(void);
    * 'k'(void);
    * 'n'(char text[]);
    * 'r'(unsigned int length, unsigned long int address);
    * 'w'(unsigned int length, unsigned long int address, char data[]);    



## Credits

- BISOON -> For original [PS4API Source](https://github.com/BISOON/ps4-api-server)
- CTurt -> the SDK.
- Specter -> exploit implementation.
- xvortex
- 2much4u
- [Vultra](https://twitter.com/C0rpVultra)