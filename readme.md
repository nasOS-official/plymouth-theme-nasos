# nasOS plymouth theme

## Contents<a name="contents"></a> 

* [Contents](contents)
* [Installing](installing)
* [Testing](testing)
  * [Testing in tty session](tty_testing)
  * [Testing in xorg](xtesting)
* [Screenshots](screenshots)

## Installing <a name="installing">1</a> 

```
git clone https://github.com/nasOS-official/plymouth-theme-nasos
sudo cp plymouth-theme-nasos /usr/share/plymouth/themes/
sudo plymouth-set-default-theme -R plymouth-theme-nasos
```

## Testing <a name="testing">1</a> 

### Testing in tty session:<a name="tty_testing"></a> 
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
### Testing in xorg:<a name="xtesting"></a> 
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
## Screenshots<a name="screenshots"></a> 

![Bootscreen](./screenshots/bootscreen.png "Bootscreen")
