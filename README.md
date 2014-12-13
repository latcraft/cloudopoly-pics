### INCOMPLETE.

W00t? 
==================

This repository contains description of the second Cloudopoly challenge. Cloudopoly is a set of challenges targeted towards raising awareness of AWS stack. Winners will get prizes from AWS! The first Cloudopoly will have 3 challenges, one per month. By getting 3 times in top 3 you will win a special prize from LatCraft.

Information about the first challenge can be found [here](https://github.com/latcraft/cloudopoly-search)

Problem definition
==================
Create a images processing service that
- Performs image search via [Flickr API](https://www.flickr.com/services/api/flickr.photos.search.html) with the following criteria ADADAXDADA
- Adds [LatCraft logo](https://github.com/latcraft/latcraft.github.io/blob/master/images/logo.png) to the top-right image corner
- Resizes images to 300x300
- Concatenates 10 images by forming bigger 3000x3000 image
- Stores concatenated images to your S3 instance and responds with the links

Expected input: 

        http://<ip address>/search?query=Linux+Ubuntu+MacOs

Expected JSON response:

```
[
   "http://<s3 ip address>>/<<image name>>.<<extension>>", 
   "http://<s3 ip address>>/<<image name>>.<<extension>>",
   ... 7 more entries here
   "http://<s3 ip address>>/<<image name>>.<<extension>>"
]
```

# Requirements

- Any programming language, any operating system
- Deploy your service to *AWS* *EC2* (free tier)
- Use smallest instance type (`t2.micro`)
- Send IP address of your service before `31.02.2015 24:00` to contest@latcraft.lv
- On `02.02.2015 20:00` we start the test! 
 
# Winner election

Web services, which return the expected result faster, will win.

### Good luck!
