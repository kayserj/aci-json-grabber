# ACI JSON Grabber

The aci-json-grabber is a collective of ansible tasks that will query your ACI fabric and save the output as a collection of .json files.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Must have a working version of Ansible 2.9 or similar.  
Has not yet been tested on version 3.0 or above.  


### Installation of Playbook

```
Just copy the playbook folder to your ansible controller
```

### Execution

From within the aci-json-grabber folder, issue the following command.


For Password Based Authentication
```
ansible-playbook -i aci_hosts grab-json-aci.yml --tags pass
```

Upon execution, the playbook will ask for user input.


### Details

Running the playbook will create a folder of .json files in your user’s home directory.  After the play completes, check your home directory for the folder with the files. The users home directory is referenced with `~/`


### Built With

* [Ansible](https://www.ansible.com/)


### Authors

* **James Kayser** - *Initial work* - [kayserj](https://github.com/kayserj)

### License

GNU GPLv3


