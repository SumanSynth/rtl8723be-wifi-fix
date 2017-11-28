# rtl8723be-wifi-fix

Some hp laptops with "Realtek rtl8723be" wifi card, have problem with signal strength and antenna problem.
This repository provides an automated fix for the problem by installing the latest drivers provided by [this](https://github.com/lwfinger/rtlwifi_new) repo and making the necessary configurations.

## Important 
Disable secure boot in BIOS to run wifi card driver properly.

## How to install
run in terminal:


    git clone https://github.com/sumancvb/rtl8723be-wifi-fix.git
    
    cd rtl8723be-wifi-fix
    
    sudo chmod +x rtl8723be.sh
    
    ./rtl8723be.sh
    
    
Sit back and relax! After installation of driver it will ask to reboot pc:

Enter 1 to reboot now:

    1

Enter 2 to reboot later:

    2

Enjoy your wifi !


## Still wifi is not working

Edit "rtl8723be.sh" to change antenna selection, default it will set antenna 2, for my laptop(15ab522tx)

if antenna 2 doesn't work, set ant_sel=1 .

![Alt text](image.png?raw=true "Optional Title")
