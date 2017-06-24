# Layer24 performance testing using JMeter tool

## Initial setup ##
- Download and install (unpack) Oracle jre
- Add path to java executions into PATH environment variable
- Download and unpack JMeter

### Example for Linux ###

1. Create folder `$HOME/opt`
1. Download respective *.tar.gz file jre from [here](http://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) into `$HOME/opt`
1. Unpack jre: `tar vxzf <your jre>.tar.gz`
1. Create symlink to unpacked jre: ln -s <your jre> jre
1. Add line into your $HOME/.bashrc file: `export PATH=$HOME/opt/jre/bin:$PATH`
1. Download JMeter from [here](http://apache.cp.if.ua//jmeter/binaries/apache-jmeter-3.2.tgz) into `$HOME/opt`
1. Unpack JMeter: `tar vxzf apache-jmeter-3.2.tgz`
1. Create symlink to unpacked jmeter: `ln -s apache-jmeter-3.1 jmeter`
1. Add line into your `$HOME/.bashrc` file: `export PATH=$HOME/opt/jmeter/bin:$PATH`

## Execution ##

Run command:
```bash
  jmeter -t <scenario> -q layer24.properties
```
