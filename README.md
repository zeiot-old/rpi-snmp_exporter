# RPI Prometheus snmp exporter

* Master : [![Circle CI](https://circleci.com/gh/zeiot/rpi-snmp_exporter/tree/master.svg?style=svg)](https://circleci.com/gh/zeiot/rpi-snmp_exporter/tree/master) [![Build Status](https://travis-ci.org/zeiot/rpi-snmp_exporter.svg?branch=master)](https://travis-ci.org/zeiot/rpi-snmp_exporter)
* Develop : [![Circle CI](https://circleci.com/gh/zeiot/rpi-snmp_exporter/tree/develop.svg?style=svg)](https://circleci.com/gh/zeiot/rpi-snmp_exporter/tree/develop) [![Build Status](https://travis-ci.org/zeiot/rpi-snmp_exporter.svg?branch=develop)](https://travis-ci.org/zeiot/rpi-snmp_exporter)

Docker image of [Prometheus snmp exporter][] to use on a [Raspberry PI][].

Configure binfmt-support on the Docker host (works locally or remotely, i.e: using boot2docker):

    $ docker run --rm --privileged multiarch/qemu-user-static:register --reset

Then you can run an armhf image from your x86_64 Docker host :

    $ make run version=1.0

Or build :

    $ make build version=1.0


# Supported tags

* [![](https://images.microbadger.com/badges/version/zeiot/rpi-snmp_exporter.svg)](http://microbadger.com/images/zeiot/rpi-snmp_exporter "Get your own version badge on microbadger.com")


## License

See [LICENSE](LICENSE) for the complete license.


## Changelog

A [ChangeLog.md](ChangeLog.md) is available.


## Contact

Nicolas Lamirault <nicolas.lamirault@gmail.com>


[Raspberry PI]: https://www.raspberrypi.org/
[Prometheus snmp exporter]: https://github.com/prometheus/snmp_exporter
