Ansible Fedora Software
=========

Deploy and configure software using dnf, pip, pipx and flatpaks. The role is used with `ansible-pull` to configure fedora systems.

Role Variables
--------------
|Variable | Location | Purpose |
|---------|----------|---------|
|packages | vars/main.yml | List of packages to be installed via package manager `dnf`, `yum` |
|flatpaks | vars/main.yml | List of flatpak applications to get installed |
|pip_pkgs | vars/main.yml | List of packages to be installed with `pip` |
|dnf | defaults/main.yml | Settings for `dnf.conf` |
|omz_git_repo | defaults/main.yml | GitHub Repo Path for oh-my-zsh |
|zsh_user_git_repo | defaults/main.yml | GitHub Repo for `omz` plugins |

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - fedora-software
