# 👷 WARNING: WORK IN PROGRESS 👷 Get paid for hosting our QA!

Hi there, I'm Дід Alik. I have a hobby project called [Stellar Help Exchange](https://github.com/amissine/shex/blob/main/README.md#presentation "Stellar HEX, work in progress"). As of October 21, 2024, it passes all the integration tests locally. In these tests, the project's website interacts with Stellar HEX users - simulated locally - via [Stellar](https://stellar.org/) testnet.

Before I move the website to production and connect it to Stellar public network, I want to setup a cloud-based QA environment to simulate Stellar HEX users globally. And I shall pay you **HEXA 1000** for hosting a QA hub for us on your [Ubuntu](https://ubuntu.com/) box. It doesn't have to be up 24/7, but when it is, I shall pay you **HEXA 100** each time a tester uses your box to interact with the project's website.

## How to host a QA hub

To clone our QA hub from my Ubuntu box to yours, you have to be a sudoer there. A sudoer does not have to enter a password to execute a `sudo` command. For example, on my box I have account `alik`. To make `alik` a sudoer, I run:

```
echo "alik  ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/alik
```

Please make sure you are a sudoer, then run:

```
git clone git@github.com:didalik/dak.org.qa-host.git
cd dak.org.qa-host.git
bin/setup
```

This will create the `qa` and `tester` accounts on your Ubuntu box. These are regular accounts, unable to run `sudo`. This will also create another, temporary, regular account called `relay`. This account effectively passes your IP address to my box and gets deleted right after.

As soon as my box gets your IP address, it connects to `qa` account on your box and completes the setup. The whole thing takes less than a minute to complete.

You are now hosting yet another QA hub for us. Get paid!

## How to get paid

### Getting paid for setting up a hub

### Getting paid for usage
