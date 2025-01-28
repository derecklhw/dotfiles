# tmux configuration

## Install

1. Install [tmux](https://github.com/tmux/tmux/wiki/Installing)

2. Copy the `.tmux.conf` file to your home directory.

    ```sh
    cp .tmux.conf ~
    ```

3. Install tpm (tmux plugin manager)

    ```sh
    git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
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

## Notes

1. `prefix`: `Ctrl + b` by default.
2. Below plugins require additional dependencies. Check the plugin's GitHub page for more information and don't forget to run `prefix+I` again after you install the additional dependencies.
   - tmux-yank
   - tmux-fzf
   - tmux-autoreload
