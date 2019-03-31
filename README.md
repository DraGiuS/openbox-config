# Небольшое описание к видео

[Установка и настройка i3](https://www.youtube.com/watch?v=clizwONNhMI)

Склонировать два репозитория и перенести нужные конфиги.

```bash
sudo pacman -S wget git
git clone https://github.com/ctlos/openbox-config.git
git clone https://github.com/creio/dots.git
```

Установим пакеты и пакетный менеджер `yay`.

```bash
wget git.io/yay.sh && sh yay.sh
yay -S i3-gaps rofi xfce4-terminal mpd ncmpcpp compton ttf-font-awesome polybar-git oh-my-zsh-git
```

В конфиге i3 закомментируйте лишние строки в автостарте, все из коробки работает с xfce4-terminal.

Установка плагинов для zsh.

```bash
sudo git clone https://github.com/zdharma/fast-syntax-highlighting.git /usr/share/oh-my-zsh/custom/plugins/fast-syntax-highlighting

sudo git clone https://github.com/zsh-users/zsh-syntax-highlighting.git /usr/share/oh-my-zsh/custom/plugins/zsh-syntax-highlighting

sudo git clone https://github.com/zsh-users/zsh-autosuggestions.git /usr/share/oh-my-zsh/custom/plugins/zsh-autosuggestions
```

Изменяем шелл, на zsh.

`chsh -s /bin/zsh`