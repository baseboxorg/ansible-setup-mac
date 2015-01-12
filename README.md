Ansible Inversion Script
===

Description
---

This is a repo for the ansible-pull method of automatic enrivonment setups.

Usage
---

Make sure you have homebrew installed.  The command to do so is:

```ruby -e \
  "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" \
  && brew doctor```

Once that has been done, install ansible:

```brew install ansible```

Then clone this repo and run the playbook:

```cd /tmp && rm -rf ansible-setup-mac && \
  git clone https://github.com/sparcedge/ansible-setup-mac && cd ansible-setup-mac \
  && ansible-playbook vbms.yml -i hosts -K && cd .. && rm -rf ansible-setup-mac```
