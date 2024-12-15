# NATS server
Bastille template to install NATS server as jail.


## Bootstrap
Bootstrap the template and create a jail

```shell
bastille bootstrap https://github.com/henomis/nats-jail-template

bastille create nats-jail 14.2-RELEASE 10.0.0.4
```

## Apply template
```shell
bastille template nats-jail henomis/nats-jail-template
```
### Optional ARGS
```shell
--arg NATS_USER=nats        # default as nats
--arg NATS_GROUP=nats       # default as nats
--arg NATS_VERSION=latest   # default as latest
```

## Usage
```shell
bastille service nats-jail nats start       # start as default
bastille service nats-jail nats stop
bastille service nats-jail nats reload      # reload the configuration file
```


## Support
Use the `NATS_VERSION` ARG to deploy a different version of `nats-server`. Please, use Github discussion if you need support.

## License
This template is distributed under the 3-Clause BSD License. See `LICENSE` for more information.