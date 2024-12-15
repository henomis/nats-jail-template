# NATS server
Bastille template to install NATS server as jail.


## Bootstrap
```shell
bastille bootstrap https://github.com/henomis/nats-jail-template
```

## Apply template
```shell
bastille template $JAIL henomis/nats-jail-template
```

## Usage
```shell
bastille service $JAIL nats stop
bastille service $JAIL nats start
bastille service $JAIL nats reload    # reload the configuration file
```

## Support
This repository will try to provide the latest NATS version, since Bastille doens't support versioning for git bootstrap so far. Please, use Github discussion if you need support.

## License
This template is distributed under the 3-Clause BSD License. See `LICENSE` for more information.