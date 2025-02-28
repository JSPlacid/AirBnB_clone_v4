# AirBnB clone - Web dynamic

### Concepts
For this project, we expect you to look at this concept:

- [AirBnB clone](https://intranet.alxswe.com/concepts/74)

## Resources
**Read or watch:**

- [Selector](https://intranet.alxswe.com/rltoken/Bl2mJVVG07XCP6E8qtsQMg)
- [Get and set content](https://intranet.alxswe.com/rltoken/oM3b0a0FGTy6AQ_UJ201Yw)
- [Manipulate CSS classes](https://intranet.alxswe.com/rltoken/LL2uScQvjWnj2ZEx2CzxXw)
- [Manipulate DOM elements](https://intranet.alxswe.com/rltoken/6JtTz9SaNX3AyVXht4tMYA)
- [Document ready](https://intranet.alxswe.com/rltoken/1AbzN1nEfBKoSjB-9kjmrA)
- [Introduction](https://intranet.alxswe.com/rltoken/OGDoIOd0cdmwDJFJy4aw5w)
- [GET & POST request](https://intranet.alxswe.com/rltoken/kmBzs_QPD72Oz--Yk80JHw)
- [HTTP access control (CORS)](https://intranet.alxswe.com/rltoken/tzqJx5SS5cF1BW_lAnXqqg)

## General Objectives
- How cool it is to request your own API
- How to modify an HTML element style
- How to get and update an HTML element content
- How to modify the DOM
- How to make a GET request with JQuery Ajax
- How to make a POST request with JQuery Ajax
- How to listen/bind to DOM events
- How to listen/bind to user events

## More Info
### Import JQuery
```
<head>
    <script src="https://code.jquery.com/jquery-3.2.1.min.js"></script>
</head>
```
### Before starting the project…
You will work on a codebase using [Flasgger](https://intranet.alxswe.com/rltoken/VmGDpw_DCN16OJt_UoqsDQ), you will need to install it locally first before starting the RestAPI:
```
$ sudo apt-get install -y python3-lxml
$ sudo pip3 install flask_cors # if it was not installed yet
$ sudo pip3 install flasgger
```
If the RestAPI is not starting, please read the error message. Based on the(ses) error message(s), you will have to troubleshoot potential dependencies issues.

Here some solutions:

jsonschema exception
```
$ sudo pip3 uninstall -y jsonschema 
$ sudo pip3 install jsonschema==3.0.1
```
No module named 'pathlib2'
`$ sudo pip3 install pathlib2`
### Expose ports from your Vagrant
In your Vagrantfile, add this line for each port forwarded

```
# I expose the port 5001 of my vm to the port 5001 on my computer
config.vm.network :forwarded_port, guest: 5001, host: 5001 
```
if you need to expose other ports, same line but you will need to replace the “guest port” (inside your vagrant) and your “host port” (outside your vagrant, used from your browser for example)

It’s important in your project, to use the AirBnB API with the port 5001

![](https://s3.amazonaws.com/intranet-projects-files/concepts/74/hbnb_step5.png)
