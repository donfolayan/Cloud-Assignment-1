1. **Change directory to the tests directory using absolute pathname:**

    ```bash
    cd /home/altschool/tests
    ```
    ![a](screenshots/a.png)

2. **Change directory to the tests directory using relative pathname (assuming you’re in the home directory):**

    ```bash
    cd tests
    ```
    ![a](screenshots/b.png)

3. **Use echo command to create a file named fileA with text content ‘Hello A’ in the misc directory:**

    ```bash
    echo 'Hello A' > /home/altschool/misc/fileA
    ```
    ![c](screenshots/c.png)

4. **Create an empty file named fileB in the misc directory. Populate the file with a dummy content afterwards:**

    ```bash
    touch /home/altschool/misc/fileB
    echo 'Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.' > /home/altschool/misc/fileB
    ```
    ![d](screenshots/d.png)

5. **Copy contents of fileA into fileC:**

    ```bash
    cp /home/altschool/misc/fileA /home/altschool/misc/fileC
    ```
    ![e](screenshots/e.png)

6. **Move contents of fileB into fileD:**

    ```bash
    mv /home/altschool/misc/fileB /home/altschool/misc/fileD
    ```
    ![f](screenshots/f.png)

7. **Create a tar archive called misc.tar for the contents of misc directory:**

    ```bash
    tar -cvf misc.tar /home/altschool/misc/
    ```
    ![g](screenshots/g.png)

8. **Compress the tar archive to create a misc.tar.gz file:**

    ```bash
    gzip misc.tar
    ```
    ![h](screenshots/h.png)

9. **Create a user and force the user to change his/her password upon login:**

    ```bash
    sudo adduser newuser
    sudo passwd -e newuser
    ```
    ![i](screenshots/i.png)

10. **Lock a user’s password:**

    ```bash
    sudo passwd -l username
    ```
    ![j](screenshots/j.png)

11. **Create a user with no login shell:**

    ```bash
    sudo useradd -s /sbin/nologin username
    ```
    ![k](screenshots/k.png)

12. **Disable password based authentication for ssh (you need to edit the sshd_config file):**

    ```bash
    sudo nano /etc/ssh/sshd_config
    sudo systemctl restart sshd
    ```
    ![l-1](screenshots/l-1.png)
    ![l-2](screenshots/l-2.png)
    ![l-3](screenshots/l-3.png)

13. **Disable root login for ssh (you need to edit the sshd_config file):**

    ```bash
    sudo nano /etc/ssh/sshd_config
    sudo systemctl restart sshd
    ```
    ![m](screenshots/m.png)
