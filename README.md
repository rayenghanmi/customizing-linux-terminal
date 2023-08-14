# Customizing linux terminal
### Here you'll learn how to customize your linux terminal
![Screenshot from 2023-08-14 08-16-43](https://github.com/rayenghanmi/customizing-linux-terminal/assets/108760398/c02d63c2-211a-4982-b0d9-4b24ee0b0741)

**Prerequisites:**
- A terminal, Obviously :smile: (I'll be using Gnome terminal as an example).
- Starship installed, if you don't have it installed, [learn how to install starship](https://starship.rs/#prerequisites).
- Shell color scripts, I'm using [Derek Taylor's configs](https://gitlab.com/dwt1/shell-color-scripts#installing-shell-color-scripts-on-fedora).
- Fortune and lolcat.

### And now let's get started:

**1. Open your terminal and type:**
```bash
nano .bashrc
```
- Then hit enter and past the following lines at the end of your .bashrc:
```bash
colorscript -r
fortune | lolcat -g ba50a1:8350ba -h 1 -v 1
```
**2. After setting up everything correctly you should get something like this after relaunching your terminal:**

![Screenshot from 2023-08-14 08-35-16](https://github.com/rayenghanmi/customizing-linux-terminal/assets/108760398/f85a3bb9-df3c-4bb4-a098-65eb9601a7a9)
**3. Now you need to configure your starship's config file:**
- Open up a terminal window and type
```bash
git clone https://github.com/rayenghanmi/dotfiles.git
```
- Then:
```bash
cd dotfiles/

cp starship.toml ~/.config/starship.toml
```

> [!IMPORTANT]
> Keep in mind that you need to use a [Nerd font](https://www.nerdfonts.com/font-downloads) on your terminal for the starship customizations to work.

**4. Relaunch your terminal and everything should be ok:**

![Screenshot from 2023-08-14 08-16-43](https://github.com/rayenghanmi/customizing-linux-terminal/assets/108760398/c02d63c2-211a-4982-b0d9-4b24ee0b0741)

> [!NOTE]
> If you're facing any problem, don't hesitate to [contact me](https://rayenghanmi.github.io/#discord-bot).
