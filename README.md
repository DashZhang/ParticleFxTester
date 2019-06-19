# Particles Effects Tester
GTAV Particles Effects Tester for FiveM development

## Installation
### Download
```
cd resources/[test]
git clone git@github.com:DashZhang/ParticleFxTester.git
```
### Configuration

* update your Particles Effects list if necessary, I'm using the one from [here](https://gist.github.com/alexguirre/af70f0122957f005a5c12bef2618a786)

* add the following line to your server.cfg
```
start ParticleFxTester
```

## Usage

This resource adds a new chat command `/particles`, which loop through all the fx containing the `keyword` at certain `scale`
```
/particles [keyword] [scale]
```
After each fx is played in-game, a chat message will be added, indicating the fx number, fx name and method (either looped or non-looped)

**!** There are more than 2000 fx, if you set `keyword=''` or ignore this parameter, it's gonna take a while

## Notice

This is tested on a Linux server, if you have a Windows server you would probably need to change some parameters for the string parsing part to make it work. I'll be happy to merge it in.

## Thanks

* alexguirre for [Particles Effects Dump](https://gist.github.com/alexguirre/af70f0122957f005a5c12bef2618a786)
* Vespura for particle fx [Lua Example](https://vespura.com/particle-list/)