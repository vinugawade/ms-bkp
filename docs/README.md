# MySQL Database Backup Script 🗄️

![Linux](https://img.shields.io/badge/Linux-white?style=flat-square&logo=linux&logoColor=black)
![MacOS](https://img.shields.io/badge/MacOS-white?style=flat-square&logo=apple&logoColor=black)
![Windows](https://img.shields.io/badge/Windows-white?style=flat-square&logo=windows&logoColor=black)
![Windows](https://img.shields.io/badge/Bash-white?style=flat-square&logo=gnu-bash&logoColor=black)

![GitHub issues](https://img.shields.io/github/issues/vinugawade/ms-bkp?style=flat-square)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/vinugawade/ms-bkp?style=flat-square)
![GitHub last commit](https://img.shields.io/github/last-commit/vinugawade/ms-bkp?style=flat-square)

If you need to backup MySQL databases on a Linux system, the `ms-bkp` script provides an easy-to-use solution. It allows you to export databases, skip specific ones, and set the destination path for the backup.

---

## Installation 🚀

1. **Clone the Repository:**
    - Clone the [ms-bkp](https://github.com/vinugawade/ms-bkp) repository to your local machine using the following command:

    ```bash
    git clone https://github.com/vinugawade/ms-bkp.git
    ```

2. **Move the Script to a Global Location:**
    - Move the script to a global location on your system using the following command:

    ```bash
    sudo mv /location/of/ms-bkp /usr/local/bin
    ```

3. **Set Script Permissions:**
    - Allow everyone to execute the script by choosing one of the following commands:

    ```bash
    sudo chmod +x /location/of/ms-bkp
    ```

    OR

    ```bash
    sudo chmod 0755 /location/of/ms-bkp
    ```

4. **Add to $PATH:**
    - Add `/usr/local/bin` to your `$PATH`. If you use the Bash shell, execute the command:

    ```bash
    export PATH=$PATH:/usr/local/bin
    ```

    OR

    ```bash
    export PATH=$PATH:/location/of/ms-bkp
    ```

    This will set the variable name, potentially in a file like `~/.bash_profile`, `~/.bashrc`, or `~/.profile`. If you're unsure where to put it, `~/.bashrc` is a good choice.

> **You may need to restart your shell for this to take effect.**

---

## Script Options 🎛️

The `ms-bkp` script supports the following options:

- `-u, --user`: MySQL username
- `-p, --password`: MySQL password
- `-o, --only`: Export only the specified database
- `-s, --skip`: Skip specified databases during export (comma-separated)
- `-d, --dest`: Destination path for the backup (default: ~/Downloads)

---

## Usage 🛠️

Now you can use the script from anywhere in the terminal. Below are some examples.

```bash
ms-bkp -u your_mysql_user -p your_mysql_password -o your_database_name
```

```bash
ms-bkp -u your_mysql_user -p your_mysql_password -s db1,db2,db3 -d /path/to/backup
```

Check below attached GIF.

![Run ms-bkp script](assets/images/..)

---

## Maintainer 👨🏻‍💻

<a href="https://vinux.in">
  <img
    src="https://api.daily.dev/devcards/c8457c6e687d407197d39cfaf513c57a.png?r=qqh"
    width="400"
    height=""
    alt="Vinay Gawade's Dev Card"
  />
</a>

Built With 💙✨ By <a href="https://github.com/vinugawade">Vinay Gawade</a>.

<a href="https://www.linkedin.com/in/vinu-gawade" target="_blank">
  <img
    src="https://github.com/vinugawade/vinugawade/blob/main/assets/images/media/LinkedIn.png?raw=true"
    alt="LinkedIn Logo"
    width="150"
    height=""
  />
</a>
<a href="https://www.buymeacoffee.com/vinaygawade" target="_blank">
  <img
    src="https://github.com/vinugawade/vinugawade/blob/main/assets/images/media/Bmc.png?raw=true"
    alt="Buy Me a Coffee Logo"
    width="150"
    height=""
  />
</a>
<a href="https://twitter.com/VinuGawade" target="_blank">
  <img
    src="https://github.com/vinugawade/vinugawade/blob/main/assets/images/media/Twitter.png?raw=true"
    alt="Twitter Logo"
    width="150"
    height=""
  />
</a>

---

## License 🛂

![LICENSE](https://img.shields.io/github/license/vinugawade/ms-bkp?style=flat-square)

This project is licensed under the [LICENSE](https://github.com/vinugawade/ms-bkp/blob/master/LICENSE) file associated with this repository.
