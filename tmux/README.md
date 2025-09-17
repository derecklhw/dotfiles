# tmux configuration

## Install

1. Install [tmux](https://github.com/tmux/tmux/wiki/Installing)

2. Copy the `.tmux.conf` file to your home directory.

    ```sh
    cp .tmux.conf ~
    ```

3. Some plugins in `.tmux.conf` require some additional dependencies. Check below plugin's GitHub repositories for more information.
   - [tmux-yank](https://github.com/tmux-plugins/tmux-yank)
   - [tmux-fzf](https://github.com/sainnhe/tmux-fzf)
   - [tmux-autoreload](https://github.com/b0o/tmux-autoreload)

4. Install tpm (tmux plugin manager)

    ```sh
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
    ```

5. **IMPORTANT:** The plugin `tmux-continuum` Automatic tmux start feature will cause an error to systemd in a graphical session. To resolve this, replace the existing systemd tmux service file with the version from this repository while keeping a backup of the original file.

   ```sh
   mv ~/.config/systemd/user/tmux.service ~/.config/systemd/user/tmux.service.backup
   cp tmux.service ~/.config/systemd/user/
   systemctl --user daemon-reload
   ```

## Run

1. Start tmux

    ```sh
    tmux
    ```

2. Install plugins

    ```sh
    prefix + I
    ```
    Note: prefix is `Ctrl + b` by default.
