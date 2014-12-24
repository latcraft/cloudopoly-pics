W00t? 
==================

This repository contains description of the second Cloudopoly challenge. Cloudopoly is a set of challenges targeted towards raising awareness of AWS stack. Winners will get prizes from AWS! The first Cloudopoly will have 3 challenges, one per month. By getting 3 times in top 3 you will win a special prize from LatCraft.

Information about the first challenge can be found [here](https://github.com/latcraft/cloudopoly-search).

Problem definition
==================
Create an image processing service which:
- Accepts a set of bit.ly identifiers that point to JPG images with 2048 x 1365 resolution
- Resolves URIs (`1uCqioJ` resolves to `http://bit.ly/1uCqioJ`) and uploads images to your S3 instance. Before uploading, [LatCraft logo](logo.png) should be added to the top-right corner of every image (feel free to convert logo to more convenient format if neccessary)
- Concatenates 10 logo-marked images (in whatever order) by forming large 20480 x 13650 image
- Uploads concatenated image to your S3 instance
- Responds with links to 11 uploaded images

Expected input: 

        http://<ip address>/process?images=1uCqioJ+1sqlimo+1uADAkJ+1BHryP2+13koVon+1uCqTGX+16jnrfk+1wsy1sC+1wN7idN+1uADWb8

Expected JSON response:

```
[
   "http://<s3 ip address>>/1uCqioJ.jpg", 
   "http://<s3 ip address>>/1sqlimo.jpg", 
   ... 7 more links here
   "http://<s3 ip address>>/1uADWb8.jpg",    
   "http://<s3 ip address>>/concatenated.jpg"       
]
```

# Requirements

- Any programming language, any operating system
- Deploy your service to *AWS* *EC2* (free tier)
- Use smallest instance type (`t2.micro`)
- Send IP address of your service before `02.02.2015 18:00` to contest@latcraft.lv
- On `02.02.2015 20:00` we start the test! 
 
# Winner election

Web services, which return the expected result faster, will win.

### Good luck!
