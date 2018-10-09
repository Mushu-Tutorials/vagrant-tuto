# vagrant-tuto

Les __box__ sont les OS que l'on souhaite installer sur les VM. La plupart sont référencé sur ce [site](http://www.vagrantbox.es/) mais peuvent ne pas être à jour. Préférez une recherche _"vagrant box [la-box-que-je-veux]"_ si vous souhaitez être à jour.

## Commandes Vagrant

- `vagrant --version`
- `vagrant init` : sans attributs, génère le fichier `Vagrantfile` mais qu'il faudra configurer ([voir ici](#vagrantfile)) ensuite
- `vagrant init [nom-de-ma-box] [url-de-ma-box]` ou `vagrant init [version-de-ma-box]` : nom-de-ma-box(vagrant-tuto) / url-de-ma-box(https://atlas.hashicorp.com/debian) / version-de-ma-box(debian/stretch64)


## Vagrantfile

- 
```ruby
# Ici mettre la version de la box souhaitée (debian/stretch64)
# config.vm.box = "debian/stretch64"
config.vm.box = "base"
```