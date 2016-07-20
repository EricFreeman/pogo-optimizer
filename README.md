# Pokemon GO Optimizer
This tool shows you the IVs and information necessary to determine which Pokemon get ground into candy. Perfect for any trainer aspiring to be the very best.

I have been told that it's a possibility Niantic could get mad at us for using this, but I'll let you know if I hear anything from them. I imagine that it's safe for the time being.

![example](http://i.imgur.com/3V8xw1G.png)

## Setup
So, first of all, you need node.js, protobuf, and git (obviously). I've only tested this on Mac, so if you want to test it on other platforms, be my guest.

Run these commands:

```
git clone https://github.com/justinleewells/pogo-optimizer
cd pogo-optimizer
brew install --devel protobuf
npm install
bower install
node index
```
Now you should have a webserver running. Make sure your phone and computer are connected to the same wireless network.

Next, check your network settings for your internal ip address. Mine was 10.0.1.3. So, I'm going to go add 10.0.1.3:8081 as a proxy to my phone. Next, I'm going to visit 10.0.1.3:3000/ca.pem to accept the certificate.

After accepting the certificate, open Pokemon GO on your phone. After you can see your character walking around, go to localhost:3000 on your laptop. Enjoy.

## TODO

* Remove Pokemon after they have been transferred
* Make client usable while catching Pokemon

## Feature Requests/Suggestions

I'd love to hear what feature requests and suggestions you all have, so feel free to shoot me an email.
