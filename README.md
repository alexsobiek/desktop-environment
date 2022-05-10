# Desktop Environment
A side project to dive more into working with Linux as a desktop operating system. 

### Motivation
I've been using various desktop environments (with floating window managers, I can't see myself using a tiling WM) on 
Debian distros and Arch for about a half year. Performance and reliability have been solid, but I've yet to find a DE that
I can genuinely say looks amazing visually. I'm currently using Cinnamon on Arch and I've gotten very used to it, but I
want something better looking.

### Development
I've contemplated using Flutter or Tauri for graphical elements, but since I am more comfortable with web
development, things will be done with Tauri for now. As for window management, I wanted something functional but
bare-bones and Openbox is a good fit.

## Building/Running in an existing DE
### Dependencies
- Tauri
- Rust/Cargo
- Xephyr
- Openbox

### Notes
There is the `xephyr.sh` script that will handle setting everything up in a Xephyr environment.

#### Current Openbox Users Warning
Because `openbox-session` does not take any command line arguments, this script WILL break any existing Openbox
configurations in `~/.config/openbox`. If you are using Openbox, make a new user and launch the script as that user
to preserve your configuration. 
