
# Help Me cook! ~Chef Polly

- *University Name*: http://www.sjsu.edu/
- *Course*: Cloud Technologies
- *Professor* Sanjay Garje
- *ISA*: Divyankitha Urs
- *Group Members*: HYUNWOOK SHIN, MOJDEH KEYKHANZADEH, VIDHI SHARMA, BARKHA CHOITHANI

## Settings

The addresses used in the code are:
- cook.hyunwookshin.com : CNAME for elb fronting the front-end web servers
- cmpe281p2f-351513d65b031117.elb.us-east-2.amazonaws.com : hostname for elb fronting the backend-web servers 
- d36tn81c22y883.cloudfront.net - cloudfront url for mp3 files


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
sudo ./frontend-installer.sh
```
Please note that the hostname to the backend ELB endpoint is hardcoded for this project.
Therefore, you may need to manually change the endpoints, if the backend ELB
server hostname changes.

## Backend installer

Copy bld/backend-installer.sh and the artifact (.tgz) to EC2 instance,
and run the installer. The artifact should be in the same directory as the installer.

```
sudo ./backend-installer.sh aws-key aws-id aws-secret mysqlpasswrd

```
