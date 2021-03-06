# A3 Server Manager V2.0 (Discarded/Legacy)

A3 Server Manager is a simple to use server manager for your ArmA 3 server on Linux. It is build with Node.js and runs from your terminal.

## How to use

### Installation

#### IMPORTANT: Don't run this as root!

```
$ adduser --gecos "" steam && \
usermod -aG sudo steam && \
su steam
```

#### 1. Install Node.js (Recommended: [NVM](https://github.com/creationix/nvm#install-script))

```
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.11/install.sh | bash
$ nvm install --lts
$ nvm use --lts
```

#### 2. Clone repo

```
$ git clone https://github.com/schrobo/a3-server-manager-legacy.git
```

### Commands

#### List of all commands

```
$ node app.js
```

#### Install manager

```
$ node app.js install
```

#### Update server and mods

```
$ node app.js update [profile] -a
```

#### Update server

```
$ node app.js update [profile] -s
```

#### Update mods

```
$ node app.js update [profile] -m
```

#### Start server

```
$ node app.js start [profile]
```

#### Start headless client

```
$ node app.js start [profile] -hc [ip]
```

## Roadmap

### V1.0

#### Features

- [X] SteamCMD installation
- [X] ArmA 3 server installation
- [X] ArmA 3 mod installation
- [X] SteamCMD updates
- [X] ArmA 3 server updates
- [X] ArmA 3 mod updates
- [X] ArmA 3 mod settings
- [X] ArmA 3 mod lowercase
- [X] Copy ArmA 3 keys
- [X] Start ArmA 3 server
- [X] Start ArmA 3 server with mods

#### Commands

- [X] node app.js install "USERNAME" "PASSWORD"
- [X] node app.js update "USERNAME" "PASSWORD"
- [X] node app.js start

#### Mods settings

- [X] Mod configuration inside app.js:

```
{
    "@CBA_A3": "450814997",
    "@ACE": "463939057"
}
```

### V2.0

#### Features

- [X] Easier and more intuitive operation
- [X] Configuration inside settings.json:
- [X] "Profiles" for different server configurations
- [ ] ~~Different server.cfg for different profiles~~
- [X] Run profile as headless client
- [X] "Advanced"/Better commands

#### Commands

- [X] node app.js install
- [X] node app.js update [profile] -s/-m/-a
- [X] node app.js start [profile] (-hc [ip])

### V3.0

#### Features

- [ ] ~~Run on all OS~~

### V4.0

#### Features

- [ ] ~~Run in GUI and CLI~~
