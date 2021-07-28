# Make AWS Instance on Cloudberry (Call_Planning)

## Step 1- In Putty

``` r
	- ec2-user
	- sudo su
	- ls
	- cd /home/R_0222PH3626/
	- ls
	- cd T1\'21\ OAPI\ CP/
	- ls
```

## Step 2-  In Rstudio

``` r
	- Create New folder for Running Month of Dashboard
		-Go to Rstudio
		-Copy existing month folder and Rename it with Current one
		-Delete all files from Input folder
```


## Step 3- In Putty
	
  ``` r
	- cd May_21_Rexulti_Dashboard/Inputs/
	- sftp gentstusr@192.48.142.53
	- Password: gentst123
```

It will login to /Inbound/Irep/

``` r
	- ls
	- pwd # look into Working Directory
	- cd CallPlanEff
	- ls
```

	## To Copy files from server
  ``` r
	- mget *
  ```
  
#EC2 S3 Transfer
```bash
aws s3 cp "/home/R_0222NJ3701/T1'21 OAPI CP/May_21_Rexulti_Dashboard/Inputs/" "s3://aws-a0166-glbl-00-p-s3b-otsk-awb-data07/R_0222NJ3701/T1'21 OAPI NS CP/Rexulti Dashboard May'21/Inputs/" --recursive

Run p02 till line no- 230 / 235, then execute p03 and p04 then again Run p02 full
```
