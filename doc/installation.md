## Installation

This are instructions on how to install OnEarth on CentOS/RedHat Linux 6.4 or greater.

## Preconditions

* Apache 2.2 or greater
* Python 2.6 or 2.7

## RPM Installation

Download the latest OnEarth release (https://github.com/nasa-gibs/onearth/releases)

Unpackage the release .tar.gz file
```Shell
tar -zxvf onearth-*.tar.gz
```

Install GIBS GDAL with the MRF driver
```Shell
sudo yum -y install gibs-gdal-*
```

Install OnEarth packages
```Shell
sudo yum -y install onearth-*
```

For manual installation or to install or another OS, please refer to the specific component:

* [mod_onearth](../src/modules/mod_onearth/README.md)
* [mod_oems](../src/modules/mod_oems/README.md)
* [mod_oemstime](../src/modules/mod_oemstime/README.md)
* [mrfgen](../src/mrfgen/README.md)
* [OnEarth Layer Configurator](../src/layer_config/README.md)
* [OnEarth Legend Generator](../src/generate_legend/README.md)
* [OnEarth Metrics](../src/onearth_logs/README.md)
* [OnEarth Scripts](../src/scripts/README.md)

## Install Locations

These are the default install locations.

mod_onearth
```
/etc/httpd/modules/mod_twms.so
/etc/httpd/modules/mod_onearth.so
/usr/bin//oe_create_cache_config
/usr/share/onearth/apache/*
/usr/share/onearth/apache/kml/*
```

mod_oems
``
/etc/httpd/modules/mod_oems.so
``

mod_oemstime
``
/etc/httpd/modules/mod_oemstime.so
``

mrfgen
```
/usr/bin/mrfgen
/usr/bin/RGBApng2Palpng
/usr/bin/colormap2vrt.py
/usr/share/onearth/mrfgen/*
```

OnEarth Layer Configurator
```
/usr/bin/oe_configure_layer
/usr/bin/oe_generate_legend.py
/usr/bin/oe_generate_empty_tile.py
/etc/onearth/config/*
```

OnEarth Metrics
```
/usr/bin/onearth_metrics
/etc/onearth/metrics/*
```

OnEarth Demo
```
/usr/share/onearth/demo/*
/etc/httpd/conf.d/on_earth-demo.conf
```

OnEarth Mapserver
```
/usr/bin/legend
/usr/bin/mapserv
/usr/bin/msencrypt
/usr/bin/scalebar
/usr/bin/shp2img
/usr/bin/shptree
/usr/bin/shptreetst
/usr/bin/shptreevis
/usr/bin/sortshp
/usr/bin/tile4ms
/usr/lib64/libmapserver.so*
/usr/include/mapserver/*
/usr/lib64/python2.6/site-packages/_mapscript*
/usr/lib64/python2.6/site-packages/mapscript*
```

## Next Steps

* [Configuration](configuration.md)
* [Creating Image Archive](archive.md)


## Contact

Contact us by sending an email to
[support@earthdata.nasa.gov](mailto:support@earthdata.nasa.gov)
