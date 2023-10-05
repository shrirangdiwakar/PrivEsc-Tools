There are many scripts that you can execute on a linux machine which automatically enumerate sytem information, processes, and files to locate privilege escalation vectors. Here are a few:

- [LinPEAS - Linux Privilege Escalation Awesome Script](https://github.com/carlospolop/PEASS-ng/tree/master/linPEAS)

    ```powershell
    wget "https://github.com/carlospolop/PEASS-ng/releases/latest/download/linpeas.sh" -O linpeas.sh
    curl "https://github.com/carlospolop/PEASS-ng/releases/latest/download/linpeas.sh" -o linpeas.sh
    ./linpeas.sh -a #all checks - deeper system enumeration, but it takes longer to complete.
    ./linpeas.sh -s #superfast & stealth - This will bypass some time consuming checks. In stealth mode Nothing will be written to the disk.
    ./linpeas.sh -P #Password - Pass a password that will be used with sudo -l and bruteforcing other users
    ```
