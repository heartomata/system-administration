# Computer Administration Environment Setup
- Go to root, since sudo is not preinstalled.
    ```
    $ su -
    ```
- Install sudo.
    ```
    $ pkg install sudo
    ```
- Remember to install vim. (Recommanded)
    ```
    $ pkg install vim
    ```
- Edit sudo user to give the previledge.
    ```
    $ visudo
    ```

    - Uncomment here.
        ```
        ## Same thing without a password
        %wheel ALL=(ALL) NOPASSWD: ALL
        ```
    
- Create a directory /home/judge/.ssh since it is not exist at first.
    ```
    $  mkdir .ssh
    ```
- Install the public key.
    ```
    $  fetch https://people.cs.nctu.edu.tw/~fyli/nasa/nasakey.pub
    $  cat nasakey.pub >> /home/judge/.ssh/authorized_keys
    ```
- Go to /usr/local/etc/wireguard/.
- Creat a file "wg0.conf" and edit it.
    ```
    $ vim wg0.conf
    ```
    - Edit it in the following form.
        ```
        $ vim wg0.conf
        ``` 
    
- Install wireguard.
    ```
    $ pkg install wireguard
    ```

- Install wireguard.
    ```
    $ pkg install wireguard
    ```