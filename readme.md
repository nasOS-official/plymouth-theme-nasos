# nasOS plymouth theme

## Installing

```
git clone https://github.com/nasOS-official/plymouth-theme-nasos
sudo cp plymouth-theme-nasos /usr/share/plymouth/themes/
sudo plymouth-set-default-theme -R plymouth-theme-nasos
```

## Testing

### Testing in tty session:
1. Press **ctrl+alt+f3**
2. Execute commands
```
sudo plymouthd
plymouth --show-splash
```
3. If you see a loading animation, press **ctrl+alt+f3** and execute the command
```
plymouth --quit
```
### Testing in xorg:
1. Install **plymouth-x11**
```
sudo apt-get install plymouth-x11 #on debian based distros
#or 
yay -S plymouth-x11 #on archlinux based distros
#or 
sudo dnf install plymouth-x11 #on rpm based distros
```
2. Install [plymouth-preview](https://github.com/eylles/plymouth-preview)
```
git clone https://github.com/eylles/plymouth-preview
cd plymouth-preview
chmod +x ./install.sh
./install.sh
```
3. Execute command
```
sudo plymouth-preview 10 #preview plymouth for 10 seconds
```
## Screenshots

![Bootscreen](./screenshots/bootscreen.png "Bootscreen")
