# Fastfetch Rice

![preview](screenshots/fastfetch.png)

Custom [fastfetch](https://github.com/fastfetch-cli/fastfetch) config with a custom ASCII logo, made for CachyOS.

## Installation

### 1. Install dependencies
```bash
sudo pacman -S fastfetch
sudo apt install fastfetch
sudo dnf install fastfetch
```

### 2. Clone the repo
```bash
git clone https://github.com/elagape/dotfiles.git ~/dotfiles
```

### 3. Install the config
```bash
mkdir -p ~/.config/fastfetch
cp -r ~/dotfiles/fastfetch/* ~/.config/fastfetch/
```

### 4. Run it
```bash
fastfetch
```

### Optional: symlink instead of copying
Edits in `~/.config/fastfetch` will then update the repo automatically.
```bash
rm -rf ~/.config/fastfetch
ln -s ~/dotfiles/fastfetch ~/.config/fastfetch
```

### Optional: run on every terminal start
```bash
echo "fastfetch" >> ~/.bashrc   # or ~/.zshrc
```

## Files
- `fastfetch/config.jsonc`: main config
- `fastfetch/cachy.txt`: custom ASCII logo
![preview](screenshots/fastfetch.png)

## Notes
The logo path in the config is `~/.config/fastfetch/cachy.txt`, so keep the files together.
