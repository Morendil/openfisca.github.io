---
layout: post
title: Time to upgrade Python!
published: true
---
_On January 1st 2019, OpenFisca will stop maintain backward compatibility with Python 2.7. From then, OpenFisca packages will be exclusively based on Python 3.7, or more recent._

**_\[English version below]_**


Bonjour à tou·te·s,


**Au 1er janvier 2019, OpenFisca cessera de maintenir sa rétro-compatibilité avec Python 2.7. Les packages OpenFisca se baseront exclusivement sur Python 3.7, ou plus récent.**


## Impacts


Les versions des packages OpenFisca (Core et France) publiées après le 1er janvier 2019 nécessiteront Python 3.7, ou plus récent.

Les versions des packages OpenFisca publiées avant cette date pourront toujours être utilisées avec Python 2.7.

Les corrections de bugs et nouvelles fonctionnalités ne seront livrées qu’en Python 3.7.


## Pourquoi ce changement ?


Au 1er janvier 2020, la maintenance de Python 2.7 sera arrêtée par la Python Software Foundation.

Dès le 1er janvier 2019, plusieurs librairies employées par OpenFisca (dont NumPy) cesseront de supporter Python 2 (cf. [Core#693](https://github.com/openfisca/openfisca-core/issues/693)).


## Comment passer à Python 3 ?


Pour la plupart des utilisateurs, réinstaller OpenFisca dans un environnement Python 3 est suffisant.

Pour les mainteneurs de packages Python qui dépendent d’OpenFisca, de nombreux outils et ressources sont disponibles pour faciliter le passage d’un code Python 2 à Python 3.


Nous recommandons:

- Le talk de [Try Hunner à la Pycon 2018](http://www.youtube.com/watch?v=klaGx9Q_SOA&t=7m18s) (20 min, en anglais), qui présente les stratégies de migrations, et les principaux outils disponibles.

- Les outils de migrations automatiques, en particulier [futurize](http://python-future.org/futurize.html).

- Pour une migration graduelle, [future](https://pypi.org/project/future/), qui vous permettra d’adapter votre code à Python 3 tout en maintenant temporairement la compatibilité avec Python 2.7.


Dans tous les cas, n’hésitez pas à contacter la communauté pour toutes les questions que vous auriez au cours de ce processus de migration !


À bientôt,

**L’équipe OpenFisca**


**_================== FRENCH VERSION =======================_**


Hello everyone,


**On January 1st 2019, OpenFisca will stop maintain backward compatibility with Python 2.7. From then, OpenFisca packages will be exclusively based on Python 3.7, or more recent.**


## Impact


OpenFisca package versions (Core and France) released after Jan 1st 2019 will need Python 3.7, or more recent.

OpenFisca package versions released before that date will still be usable with Python 2.7.

Bug fixes and new features will only be delivered in Python 3.7.


## Why this change?


On January 1st 2020, the Python Software Foundation will stop maintaining 2.7.

On January 1st 2019, several libraries used by OpenFisca (including NumPy) will stop supporting Python 2.7 (see [Core#693](https://github.com/openfisca/openfisca-core/issues/693))


## How to switch to Python 3?


Most users only need to reinstall OpenFisca in a Python 3 environment to start using the Python 3 version.


For maintainers of Python packages depending on OpenFisca, many tools and resources are available to ease migrating code from Python 2 to Python 3.


We recommend:

- The [Try Hunner talk at Pycon 2018](http://www.youtube.com/watch?v=klaGx9Q_SOA&t=7m18s) (20 min), that introduces migration strategies and the main tools available.

- Automatic migration tools, such as [futurize](http://python-future.org/futurize.html).

- For a gradual migration, [future](https://pypi.org/project/future/) allows you to adapt your code to Python 3 while temporarily maintain compatibility with Python 2.7.


In all cases, don’t hesitate to contact the community if you face issues during the migration process!


See you soon!

**The OpenFisca team**
