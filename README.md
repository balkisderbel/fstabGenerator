# Fstab Generator

Fstab Generator is a small Python script to write and generate /etc/fstab files based on yaml file on Unix-like systems.

NOTE : This script has been designed to configure fstab from scratch only based on YAML so make sure all entry points are included in YAML .

### How To Use This

- Make sure Python is installed on your system.
- install dependencies package.
- run script with sudo privileges user.
- priority and attribute should be Observed like sample yaml structure.
- Root-reserve Option Run **tune2fs** **command** to enable ext4 feature on Disk partition, you can disable it by removing this tag on the YAML file.
- Dump and Pass Options are **disabled** by default (0).

### Usage

1. Run `git clone https://github.com/balkisderbel/fstabGenerator.git` 
2. Run `pip install -r requirements.txt` to install dependencies
3. Run `python fstab.py file.yaml`
4. check out the /etc/fstab and if everything is right use `mount -a` or Restore a backup file if something is wrong.



