# Cuztomize-Bash-with-Oh-My-Posh 🎨
Guide to customize bash in Ubuntu Distro

**Instructions** 📋

Open your terminal and type the following command:

| Instrucciones                                                                                              |
|------------------------------------------------------------------------------------------------------------|
| **1️⃣ Install Oh My Posh**                                                                                      |
|    sudo wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/posh-linux-amd64 -O /usr/local/bin/oh-my-posh` |
||
| **2️⃣ Download themes**                                                                                         |
|    Create a directory in root: `mkdir ~/.poshthemes`                                                     |
|    Download themes: `wget https://github.com/JanDeDobbeleer/oh-my-posh/releases/latest/download/themes.zip -O ~/.poshthemes/themes.zip` |
|    Unzip the file: `unzip ~/.poshthemes/themes.zip -d ~/.poshthemes`                                     |
|    Grant permissions: `chmod u+rw ~/.poshthemes/*.json`                                            |
|    Delete zip: `rm ~/.poshthemes/themes.zip`                                                             |
||
| **3️⃣ Test the changes:** |
|`eval "$(oh-my-posh --init --shell bash --config ~/.{theme_name}.omp.json)"`          |
||
| **4️⃣ Download Fonts with your favorite tool:**                                                                 |
|    * Download the font **Meslo** or **Hack Nerd Font** and unzip it in **"~/.fonts"**, if the directory does not exist create it in the root with the command `"mkdir .fonts"` |
|    * Update the font cache: `fc-cache -fv`                                                                 |
||
| **5️⃣ Add on .bashrc file:**                                                                                    |
|    * Open your **.bashrc** file and add a new line with the following text: `eval "$(oh-my-posh --init --shell bash --config ~/.poshthemes/theme_name.omp.json)"` |
|    * Choose the theme you like and replace the text **theme_name** of the previous line                    |
||
| **6️⃣ Load the changes with:** `source .bashrc`                                                                 |


## My recommended themes ❤️‍🔥

1. Clean-detailed
2. Atomic 
3. Cattpuccin
4. Night-owl
5. Powerlevel10k_modern

### Visit the Oh My Posh website to see more themes: [Themes](https://ohmyposh.dev/docs/themes)
