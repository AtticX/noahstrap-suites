# noahstrap-suites

Tools for creating linux images (suites) for noah.

## Creating an Ubuntu image

This repository includes tools to create an Ubuntu image (suite) for noah. It must be run on an Ubuntu machine.

1. Install prerequisites

```
sudo apt-get install debootstrap
```

2. Clone the repository

```
git clone https://github.com/linux-noah/noahstrap-suites.git
```

3. Execute the proper script

```
cd noahstrap-suites
sudo mksuite.ubuntu       # for creating an ubuntu (normal) image
sudo mksuite.ubuntu-dev   # for creating an ubuntu developer image
```

4. (Optional) Copy the files into the web server folder

```
mkdir /var/www/html/noah-blob
cp ubuntu.tar.gz      /var/www/html/noah-blob
cp ubuntu-dev.tar.gz  /var/www/html/noah-blob
```

5. (Optional) Modify the `SUITES` file and the `noahstrap` script.
