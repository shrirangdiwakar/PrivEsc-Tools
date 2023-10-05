## Tools

There are many scripts that you can execute on a linux machine which automatically enumerate sytem information, processes, and files to locate privilege escalation vectors. Here are a few:

- [LinPEAS - Linux Privilege Escalation Awesome Script](https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS)

    ```powershell
    wget "https://github.com/carlospolop/PEASS-ng/releases/latest/download/linpeas.sh" -O linpeas.sh
    curl "https://github.com/carlospolop/PEASS-ng/releases/latest/download/linpeas.sh" -o linpeas.sh
    ./linpeas.sh -a #all checks - deeper system enumeration, but it takes longer to complete.
    ./linpeas.sh -s #superfast & stealth - This will bypass some time consuming checks. In stealth mode Nothing will be written to the disk.
    ./linpeas.sh -P #Password - Pass a password that will be used with sudo -l and bruteforcing other users
    ```

- [LinuxSmartEnumeration - Linux enumeration tools for pentesting and CTFs](https://github.com/diego-treitos/linux-smart-enumeration)

    ```powershell
    wget "https://raw.githubusercontent.com/diego-treitos/linux-smart-enumeration/master/lse.sh" -O lse.sh
    curl "https://raw.githubusercontent.com/diego-treitos/linux-smart-enumeration/master/lse.sh" -o lse.sh
    ./lse.sh -l1 # shows interesting information that should help you to privesc
    ./lse.sh -l2 # dump all the information it gathers about the system
    ```

- [LinEnum - Scripted Local Linux Enumeration & Privilege Escalation Checks](https://github.com/rebootuser/LinEnum)
    
    ```powershell
    ./LinEnum.sh -s -k keyword -r report -e /tmp/ -t
    ```

- [BeRoot - Privilege Escalation Project - Windows / Linux / Mac](https://github.com/AlessandroZ/BeRoot)
- [linuxprivchecker.py - a Linux Privilege Escalation Check Script](https://github.com/sleventyeleven/linuxprivchecker)
- [unix-privesc-check - Automatically exported from code.google.com/p/unix-privesc-check](https://github.com/pentestmonkey/unix-privesc-check)
- [Privilege Escalation through sudo - Linux](https://github.com/TH3xACE/SUDO_KILLER)
