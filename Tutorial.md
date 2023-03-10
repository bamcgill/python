Download and install VSCode


Launch VS Code.
Open the Command Palette (Cmd+Shift+P) and type 'shell command' to find the Shell Command: Install 'code' command in PATH command.
macOS shell commands

Restart the terminal for the new $PATH value to take effect. You'll be able to type 'code .' in any folder to start editing files in that folder.
Note: If you still have the old code alias in your .bash_profile (or equivalent) from an early VS Code version, remove it and replace it by executing the Shell Command: Install 'code' command in PATH command.

Alternative manual instructions
Instead of running the command above, you can manually add VS Code to your path, to do so run the following commands:

cat << EOF >> ~/.bash_profile
# Add Visual Studio Code (code)
export PATH="\$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"
EOF
Start a new terminal to pick up your .bash_profile changes.

Note: The leading slash \ is required to prevent $PATH from expanding during the concatenation. Remove the leading slash if you want to run the export command directly in a terminal.

Note: Since zsh became the default shell in macOS Catalina, run the following commands to add VS Code to your path:

cat << EOF >> ~/.zprofile
# Add Visual Studio Code (code)
export PATH="\$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"
EOF
