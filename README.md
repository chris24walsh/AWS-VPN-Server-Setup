# This repo was forked from https://github.com/webdigi/AWS-VPN-Server-Setup
All credit for the cloudformation template goes to webdigi. Please see original repo for further information.

# Dependencies
- aws account
- [aws cli](https://aws.amazon.com/cli/)
- freenom account
- [freenom-dns](https://www.npmjs.com/package/freenom-dns), requires node.js and npm installed first

# Rolling out your own private VPN server on AWS cloud in 10 minutes
I've created helper bash scripts to allow rolling out the VPN from the local client CLI.

1. Rename vars.example to vars and fill in all parameters.
2. Login to freenom-dns in cli, using ```freenom-dns login```.
3. Run start-vpn to create the VPN stack, and set the dns record.
4. Use delete-vpn to remove the stack when you are done.
5. Enjoy and share!

# TODO
- Allow script to prompt choices/inputs for stack parameters, if not present from vars file
- Investigate using docker to speed up the deployment of the VPN
- Auto delete VPN stack after interval of disuse, to save AWS costs

### License
Licensed under the [MIT license](https://github.com/chris24walsh/AWS-VPN-Server-Setup/blob/master/LICENSE.txt).
