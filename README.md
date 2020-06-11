# ERC20-OZ-SDK
How to deploy an ERC20 smart contract using the [OpenZeppelin SDK](https://github.com/OpenZeppelin/openzeppelin-sdk).

## Install
First, install [Node.js](http://nodejs.org/) and [npm](https://npmjs.com/). Then, install the OpenZeppelin SDK running:

```
npm install -g @openzeppelin/cli
```

> If you get an `EACCESS permission denied` error while installing, please refer to the [npm documentation on global installs permission errors](https://docs.npmjs.com/resolving-eacces-permissions-errors-when-installing-packages-globally). Alternatively, you may run `sudo npm install --unsafe-perm --global @openzeppelin/cli`, but this is highly discouraged, and you should rather either use a node version manager or manually change npm's default directory.

## Setup
I recommend using the OpenZeppelin SDK through the `openzeppelin SDK` command line interface.

To start, create a directory for the project and access it:

```
mkdir TestERC20Token
cd TestERC20Token
```

Use `npm` to create a `package.json` file:

```
npm init -y
```

And initialize the OpenZeppelin SDK project:

```
npx oz init
```

Now it is possible to use `openzeppelin deploy` to create instances for these contracts that 
later can be upgraded, and many more things.

Run `openzeppelin --help` for more details about thes and all the other functions of the
OpenZeppelin CLI.