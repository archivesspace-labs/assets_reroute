ArchivesSpace Assets Reroute Plugin 
======================================


This is a plugin to reroute the Rails asset pipeline in the ASpace frontend and
public UI to use plugin assets. It's specificly designed to allow plugin assets
to be servered by Tomcat7. 

[Additional Information About Running Under
Tomcat](https://github.com/archivesspace/archivesspace/blob/master/README_TOMCAT.md)

[SUBSCRIBE TO UPDATES](https://github.com/archivesspace/assets_reroute/commits/master.atom)

Usage
-----

Access the ArchivesSpace plugins directory.

```
cd /path/to/archivesspace/plugins
```

Download using git (recommended)
--------------------------------

```
git clone https://github.com/archivesspace/assets_reroute.git 
```

Download using zip
------------------

```
wget https://github.com/lyrasis/assets_reroute/archive/master.zip
unzip master.zip
mv assets_rerout-master assets_reroute 
```

Enable the plugin
-----------------

Edit `config.rb` and append:

```
AppConfig[:plugins] << "assets_reroute"
```

Then restart ArchivesSpace.

Upgrades
--------

Stop ArchivesSpace.

**Git**

Enter the `assets_reroute` directory:

```
git pull origin master
```

**Zip**

Enter the `plugins` directory and remove the existing maintenance plugin:

```
rm -rf assets_rerout 
```

Now repeat the download / install steps as above (for zip).

**Complete the upgrade**

Restart ArchivesSpace.

---
