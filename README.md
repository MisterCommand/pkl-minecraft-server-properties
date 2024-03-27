A Minecraft Java Edition [server.properties](https://minecraft.wiki/w/Server.properties) configuration template written in [Pkl](https://github.com/apple/pkl).

## About Pkl
[https://pkl-lang.org/index.html](https://pkl-lang.org/index.html)

## Usage
### Install Pkl
Please follow this [guide](https://pkl-lang.org/main/current/pkl-cli/index.html#installation) to install Pkl CLI in your machine.

### Amend the template
Download this repository, create a new pkl file and amend this template. [Docs](https://pkl-lang.org/main/current/language-tutorial/02_filling_out_a_template.html).


```pkl
// server.pkl

amends "serverTemplate.pkl"

// This would override the default MOTD
`motd` = "Welcome to the server!"
```

### Generate server.properties
Generate the `server.properties` file with your amendments by the [Pkl CLI](https://pkl-lang.org/main/current/pkl-cli/index.html).

`$ pkl eval -f properties server.pkl`

## Examples
### Generate default server.properties
The values of the default `server.properties` file are determined according to the [Minecraft Wiki](https://minecraft.wiki/w/Server.properties) as of version `24w04a`.

`$ pkl eval -f properties serverTemplate.pkl`

Please rename the file to `server.properties`.
