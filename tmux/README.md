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

5. **IMPORTANT** If automatic start is enabled in a graphical session, systemd will encounter an error when attempting to start tmux. To resolve this, replace the existing systemd tmux service file (`~/.config/systemd/user/tmux.service`) with the version from this repository. Keep a backup of the original file by renaming it to `~/.config/systemd/user/tmux.service.backup`.

## Run

1. Start tmux

    ```sh
    tmux
    ```

2. Install plugins

    ```sh
    prefix + I
    ```

## Notes

1. `prefix`: `Ctrl + b` by default.
