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
