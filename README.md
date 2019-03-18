# is-password-safe
This command takes the supplied password, hashes it with SHA-1 and submits the first 5 characters to the pwnedpasswords API (https://haveibeenpwned.com/Passwords), then compares the results with the full hash. If a match is found it will warn you that the password is compromised, else it will tell you that your password is safe.

## Requirements
This command makes use of my `ansiprintf` command which you can get here: https://github.com/Toxyl/ansiprintf

# WARNING!
Using this will leave a trace in your bash history from which an attacker could read your plaintext password. It is advisable to clear the history after using this tool (`echo > ~/.bash_history`) and then close the current terminal (as long as it's open the `history` command will still show the history. There might be more places where this is logged, so keep that in mind!
