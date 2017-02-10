###Image Uploads

---

Everything has been text so far, let's add imagery. We have to leave Sublime Text behind and return to the terminal to upload an image to our server.

The SCP command allows secure file copy from your local machine to your AWS server. The syntax for SCP is similar to SSH.

```
scp -i ~/.ssh/identity_file.pem path/to/local/file ubuntu@[IP Address]:/path/to/target/directory
```

For instance, moving a file from your local desktop to your web folder on AWS looks like this.

```
scp -i ~/.ssh/proto_class.pem ~/Desktop/image.jpg ubuntu@12.345.678.999:/var/www/html/
```

Easy!

Now, to include an image in html.

```
<img src="path/name.jpg" />
```

Note again, a self-closing tag. All we need to do is specify a path and filename and the image can be dropped into any other tag on your website.

`<img>` behave similarly to inline elements. They flow like text if place within text, but they can have width and height values associated as well.





