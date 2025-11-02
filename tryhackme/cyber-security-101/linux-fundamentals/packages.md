# Packages

Software exists in `apt` repositories. Whilst you can install software using package installers such as `dpkg`, when using apt your software will get checked for updates when you update your system.

The integrity of what you download is guaranteed by the use of GPG (GNU Privacy Guard). These keys are a safety check and should match up to what your system trusts.

To add a GPG key, e.g. for Sublime Text 3, run `wget -qO - https://download.sublimetext.com/sublimehq-pub.gpg | sudo apt-key add -`.

It's good practice to have a separate file for every different community/third party repository in `/etc/apt/sources.list.d/`, e.g. `sublime-text.list`.

After adding something to the list, run `apt update`. After that you can install the software you have trusted.

You can also use `add-apt-repository` and use it with the `--remove` flag to reverse.
