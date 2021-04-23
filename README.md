# ACI JSON Grabber

The aci-json-grabber is a collective of ansible tasks that will query your ACI fabric and save the output as a collection of .json files.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Tested working with Ansible 3.3

Debian
```
sudo apt install python3-pip
sudo -H pip3 install ansible
```

MacOS  
Use homebrew
```
brew install ansible
```

### Installation of Playbook
Be advised, this playbook contains `vars_prompt` and requires user input

```
Copy the playbook folder to your ansible controller
```

### Execution

From within the aci-json-grabber folder, issue the following command.


For Password Based Authentication
```
ansible-playbook -i aci_hosts grab-json-aci.yml
```

Upon execution, the playbook will ask for the user input.


### Details

Running the playbook will create a folder called `ansible_json_payload` that contains .json files, in your user’s home directory.  After the play completes, check your home directory for the folder with the files. The users home directory is referenced with `~/`


### Built With

* [Ansible](https://www.ansible.com/)


### Authors

* **James Kayser** - *Initial work* - [kayserj](https://github.com/kayserj)

### License

GNU GPLv3


