# 2018 Kaleido-NCSU Hackathon

Welcome hackathoners!  This repo is your starting point and your sounding board.  
We've included all the code you need to provision a Kaleido environment and deploy
your first solidity smart contract.  Every program is constructed with a minimalist
straightforward approach, and each includes heavy documentation in an effort to
provide clarity around the Ethereum compatible APIs and Javascript logic.  Feel free to use
these pieces as educational resources or even as the scaffolding for your own project.  
That's what they're here for...

OK, ready to get going?   Follow these simple instructions and we'll have you up and
running in a few minutes.

## Dependencies

Not much, just Node.js to drive the various programs and curl to exercise some basic REST methods:

* [Node.js](https://nodejs.org/en/download/) - we recommend grabbing the latest LTS version
* [curl](https://curl.haxx.se/download.html) - use the appropriate binary for you OS

## Create your Kaleido Account

This is as easy as it gets.  Visit the [Kaleido Console](https://console.kaleido.io/login/signup?orig_url=/) and follow
the instructions to create an account and Kaleido Org.  The UI is very intuitive, but we also have formal reference documentation
[here](http://console.kaleido.io/docs/docs/createnet/) if you get confused on anything.  Once you've generated your
Kaleido Organization, go ahead and log into the console.  Click the **API** tab at the top of the screen and then click the
**GENERATE API KEY** button.  This will create a security token specific to your Kaleido Org, and allows for the resource creation calls to be conducted via our convenient REST API.  Copy the APIKEY and keep it handy, we'll use it in the next step.

## Getting Started

Navigate to your favorite working directory.  Clone this repo and change into it

```sh
git clone https://github.com/kaleido-io/kaleido-hackathon.git  && cd kaleido-hackathon
```

Next we need to install our dependencies.  Take a peek at `package.json` if you want to see the
libraries we're using:

```sh
npm install
```

Cool.  Now we're ready to deploy a Kaleido environment.  Our friend, `setup.js` will do all the heavy lifting
and leave you with your very own blockchain network, fully equipped with memberships, nodes and security
credentials.  Make sure you have that APIKEY from the previous step:

```sh
node setup.js PASTE_YOUR_APIKEY_HERE
```

Give this a minute or two.  It's doing all the resource creation calls and it takes a bit of time
for all the containers to spin up.  
