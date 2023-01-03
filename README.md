![ansiblelint](https://github.com/cschindlbeck/ansible-awesome-cli/actions/workflows/ansible-lint.yml/badge.svg)

Ansible Awesome CLI Role
=========

Installs awesome modern cli tools that replace old legacy cli tools. Improves speed and usability.

|Tool|Description|Replaces/Enhances|
|---|---|---|
|[fzf](https://github.com/junegunn/fzf)| Fuzzy finder|CTRL-R|
|[Zoxide](https://github.com/ajeetdsouza/zoxide)|Smart cd|cd|
|[Ripgrep](https://github.com/BurntSushi/ripgrep) |Recursive fuzzy search| grep|
|[Fd](https://github.com/sharkdp/fd)|Find entries in filesystem|find|
|[bat](https://github.com/sharkdp/bat)|cat with syntax highlighting |cat|
|[tldr](https://github.com/tldr-pages/tldr)| simpler, more approachable complement to traditional man pages|man|
|[sd](https://github.com/chmln/sd)|Find and replace|sed|

TODO: 
- cargo install
- sd
- fd
- difftastic
- fzf

Tested on Ubuntu 20.04 and 22.04

Requirements
------------

cargo?

Role Variables
--------------

None

Dependencies
------------

cargo?

Example Playbook
----------------

Add this to your requirements.txt:

```yaml
- name: ansible-awesome-cli
  src: https://github.com/cschindlbeck/ansible-awesome-cli.git
  version: v0.0.1
  scm: git
```

and install it via 

```sh 
ansible-galaxy install -r requirements.txt
```

Include the role then as such:

```yaml
    - hosts: all
      roles:
         - ansible-awesome-cli
```

License
-------

MIT
