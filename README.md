# ansible-workstation

## Manual set up
* Add GPG and SSH keys
* Make sure sudo is installed and user account can use it
* Install packages
  ```
  sudo apt-get install vim git ansible
  ```


## Run `ansible-pull`
```
ansible-pull -U https://github.com/tprestegard/ansible-workstation.git -i hosts local.yaml --ask-become-pass
```


## Other useful commands
Run ansible from local playbook:
```
ansible-playbook --connection=local --inventory 127.0.0.1, --limit 127.0.0.1 local.yaml -i hosts --ask-become-pass

# NOTE: comma in inventory is important
```

See all ansible facts:
```
ansible -m setup 127.0.0.1
```


## Final manual steps
* Change terminal shortcuts anad color scheme
* Set up LastPass in Chrome: enable native messaging (Click icon -> Account Options -> About LastPass)
* Set up Chrome bookmarks
* Set up Thunderbird
* Copy music and personal directory from external hard drive
* Any graphics card or wireless drivers
* Install games in Lutris
