### One important Setup Step for Git Obsidian is it's SSH Key Accesses.

Source: 
1. https://github.com/denolehov/obsidian-git?tab=readme-ov-file
2. https://publish.obsidian.md/git-doc/Authentication

### Steps:
1. Create SSH Key

### Explanations (Optional)
`ksshaskpass` is a program that provides a graphical interface for entering the SSH key passphrase. Installing it ensures you can enter your passphrase securely whenever required.

To make sure that `ksshaskpass` is used whenever an SSH key passphrase is required, you need to create a symbolic link from `ksshaskpass` to `ssh-askpass`. This tells the SSH client to use `ksshaskpass` for passphrase prompts.

To ensure that Git uses `ksshaskpass` for SSH operations, you need to configure Git to use it as the `core.askPass` helper. This setting makes sure that whenever Git requires a passphrase for an SSH key, it will prompt you using `ksshaskpass`.  

```mermaid

Cre
```