
We're looking for a more realistic distribution of activity throughout the year

<br><br>

## Getting Started

If you're on Windows™,
<br>[setup the Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

If you haven't already,
<br>[install git](https://github.com/git-guides/install-git)

<br>

1. Open your command-line
<br>& navigate to whatever folder you prefer

2. [Fork this project](https://docs.github.com/en/free-pro-team@latest/github/getting-started-with-github/fork-a-repo) on GitHub

2. Download your new copy of this project

```shell
git clone https://github.com/<your-github-username>/commit-bot.git
```

**Don't forget to include your username**

3. Test run the script
<br>in case you need to fix permissions issues

```shell
/bin/bash ./commit-bot/bot.sh
```

4. [Open your crontab](https://www.howtogeek.com/101288/how-to-schedule-tasks-on-linux-an-introduction-to-crontab-files/) to set a trigger

```shell
crontab -e
```

> NOTE:
> <br>If this makes your screen almost blank
> <br>with no toolbar of keys to navigate,
> <br>you've probably entered the text editor Vim
> <br>
> <br>Remember, press "i" to start [i]nserting text
> <br>
> <br>When you're finished,
> <br>press "Esc" repeatedly until nothing happens
> <br>
> <br>Then type ":wq" to save & quit
> <br>or ":q!" to quit without saving

5. Add this line to [schedule every 10pm or whenever](https://crontab.guru/#0_22_*_*_*)

```shell
0 22 * * * /bin/bash /:D/github/committy-bot/bot.sh
```

**Do not forget to include the correct folder path**

> NOTE:
> <br>Make sure you save your changes
> <br>on your way out!
