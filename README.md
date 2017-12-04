
# Help Me cook! ~Chef Polly

- *University Name*: http://www.sjsu.edu/
- *Course*: Cloud Technologies
- *Professor* Sanjay Garje
- *ISA*: Divyankitha Urs
- *Group Members*: HYUNWOOK SHIN, MOJDEH KEYKHANZADEH, VIDHI SHARMA, BARKHA CHOITHANI

## To build existing artifiacts

There is only one artificats for our project. To build the artifacts
please use the following.

```
cd src
make clean
make all

```
Please find the .tgz file generated by the make process.

## Frontend installer

Copy bld/frontend-installer.sh and the artifact (.tgz) to EC2 instance,
and run the installer. The artifact should be in the same directory as the installer.

```
./frontend-installer.sh
```

## Backend installer

Copy bld/backend-installer.sh and the artifact (.tgz) to EC2 instance,
and run the installer. The artifact should be in the same directory as the installer.

```
./backend-installer.sh aws-key aws-id aws-secret mysqlpasswrd

```