# Summary
This is a simple skeleton project (empty workspace) for you to use when tackling javascript challenges either on your own or for the coding part of an interview. 

Simple javascript apps are good for interacting with REST services and having a quick setup to solve problems without a lot of setup. Unfortunately people often get tripped up with security issues preventing their projects from working. This skeleton structure solves most of those pitfalls. 

# Web browser
You will need a web browser. Chrome, Firefox, Safari, Microsoft Edge are all good choices. You probably already have one of these installed. 

# Web server
You will also need to launch a simple web server. That's because features of your app won't work accessing files on disk without going through a local web server. Easiest way is with Python. At the time of writing, both Python 3 and 2 are popular and work great. Here's how to launch a server with each one

Python 3:
python -m http.server 8000

Python 2:
python -m SimpleHTTPServer 8000

For more in-depth discussion see this article:
https://developer.mozilla.org/en-US/docs/Learn/Common_questions/set_up_a_local_testing_server

# Text Editor
You can use any tool for text editing but avoid word processors like Microsoft Word. If you don't have a favorite, I suggest Microsoft "Visual Studio Code." It's fast, lean, and works well. It even detects Javascript syntax errors as you type. Get it here: 
https://code.visualstudio.com

# CORS workaround
CORS stands for "Cross Origin Resource Sharing" which is a fancy way of trying to protect website resources from being used across websites. Often times, it's a mistake on the setup of the end server but it can be troubling to not be able to access a public REST service because of CORS errors. Fortunately there is a workaround that allows you to forward your requests through a local service to avoid CORS problems. Use the sub directory called "cors_anywhere" and run the command from your prompt or terminal: 
node cors-anywhere.js

You will then be able to preface your REST URL with: http://localhost:8080/

Note: you'll need Node.js installed first. More info can be found here:
https://github.com/Rob--W/cors-anywhere

Happy coding!