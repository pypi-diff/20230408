# Comparing `tmp/invoice2data-0.4.3.tar.gz` & `tmp/invoice2data-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invoice2data-0.4.3.tar", last modified: Fri Mar 31 22:24:33 2023, max compression
+gzip compressed data, was "invoice2data-0.4.4.tar", last modified: Sat Apr  8 21:29:05 2023, max compression
```

## Comparing `invoice2data-0.4.3.tar` & `invoice2data-0.4.4.tar`

### file list

```diff
@@ -1,235 +1,235 @@
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.110954 invoice2data-0.4.3/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1078 2023-03-31 21:46:18.000000 invoice2data-0.4.3/LICENSE.txt
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      124 2023-03-31 21:46:18.000000 invoice2data-0.4.3/MANIFEST.in
--rw-r--r--   0 emiel     (1000) emiel     (1000)    10815 2023-03-31 22:24:33.110954 invoice2data-0.4.3/PKG-INFO
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     9742 2023-03-31 21:46:18.000000 invoice2data-0.4.3/README.md
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1657 2023-03-31 22:24:33.111954 invoice2data-0.4.3/setup.cfg
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      442 2023-03-31 21:46:18.000000 invoice2data-0.4.3/setup.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.088954 invoice2data-0.4.3/src/
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.090954 invoice2data-0.4.3/src/invoice2data/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)       45 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/__init__.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.091954 invoice2data-0.4.3/src/invoice2data/extract/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/__init__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)    11901 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/invoice_template.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     4091 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/loader.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.092954 invoice2data-0.4.3/src/invoice2data/extract/parsers/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      135 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/parsers/__init__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      658 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/parsers/__interface__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     7742 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/parsers/lines.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2663 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/parsers/regex.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      437 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/parsers/static.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.092954 invoice2data-0.4.3/src/invoice2data/extract/plugins/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/plugins/__init__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      545 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/plugins/__interface__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      401 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/plugins/lines.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     3503 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/plugins/tables.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.089954 invoice2data-0.4.3/src/invoice2data/extract/templates/
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.092954 invoice2data-0.4.3/src/invoice2data/extract/templates/au/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1375 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/au/au.com.opal.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      484 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/au/au.com.telstra.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.093954 invoice2data-0.4.3/src/invoice2data/extract/templates/be/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1628 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.accor.invest.ibis.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      305 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.boucherie.pochet.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      311 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.cebeo.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      797 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.lampiris.facture-dacompte.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      425 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.lampiris.factuur.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      727 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.lampiris.regularisation.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      306 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.melchior-vins.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      323 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.proximus.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      700 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.scarlet.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      349 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.securex.social.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.093954 invoice2data-0.4.3/src/invoice2data/extract/templates/ch/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      443 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/ch/ch.pcengines.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.098954 invoice2data-0.4.3/src/invoice2data/extract/templates/com/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     5363 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.AzureInterior.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      657 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.amazon.aws.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      531 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.apple.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      212 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.apps4rent.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      485 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.binarylife.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      436 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.bloomberg.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      252 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.cloudns.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      544 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.datadoghq.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      242 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.digitalocean.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      233 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.envato.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      379 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.expressvpn.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1244 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.expressvpn_prio6.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      361 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.ftserussell.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      250 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.github.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      274 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.globalsign.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      368 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.google.adwords.hk.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      199 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.hobohost.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      346 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.jamiepro.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      373 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.linode.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      282 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.microsoftonline.hk-v2017.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      290 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.microsoftonline.hk.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      480 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.mongodb.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      732 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.namecheap.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      239 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.namesilo.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      510 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.newrelic.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1346 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.nl.lenovo.digitalriver.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      445 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.nmmn.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      196 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.nodisto.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      392 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.nyse.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      775 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.oyo.invoice.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      359 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.packtpub.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      579 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.pixartprinting.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      550 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.sammymaystone.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      247 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.scaleway.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      241 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.textmaster.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      388 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.tmx.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      312 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.travis-ci.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      320 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.twitter.de.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      305 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.twitter.uk.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      304 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.twitter.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      231 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.upwork.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      205 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.usersnap.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.098954 invoice2data-0.4.3/src/invoice2data/extract/templates/de/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      342 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.amazon.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      357 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.bettina-kast.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2410 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.digikey.com.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      310 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.hosteurope.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      501 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.notebooksbilligerBillPay.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      276 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.ovh.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      544 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.qualityhosting.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      343 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.united-domains.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.099954 invoice2data-0.4.3/src/invoice2data/extract/templates/es/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      398 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/es/com.pepephone.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      384 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/es/es.supplies24.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.106954 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      484 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/co.mooncard.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      374 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.adobe.ie.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      374 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.akretion.fr.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      431 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.amazon.aws.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      366 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.ateliercopieservice.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      539 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.chauffeur-prive.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      430 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.coriolis.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      387 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.easyjet.fr.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      596 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.eaudugrandlyon.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      315 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.godaddy.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      444 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.google.ie.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      389 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.hootsuite.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      397 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.jeanbesson.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      399 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.ldlc.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      367 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.linkedin.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      377 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.mention.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      421 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.microsoft.ie.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      402 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.myflyingbox.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      402 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.officetimeline.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      481 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.orange-business.mobile.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      363 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.ovh.fr.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      428 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.rs-online.fr.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      464 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.saur.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      383 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.soyoustart.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      358 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.vinci-autoroutes.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2151 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/dolibarr.generique.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      476 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/eu.trainline.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      570 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.actn.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      373 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.airfrance.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      427 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.also.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      376 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.amazon.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      399 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.assurance-epargne-pension.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      597 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.bouyguestelecom.adsl-fiber.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      451 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.bouyguestelecom.mobile.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      531 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.butagaz.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      389 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.chronopost.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      392 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.dirafi.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      351 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.domaine-achat.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      423 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.easytrip.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      471 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.edf.entreprises.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     3648 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.edf.pme.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      450 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.finagaz.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      454 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.fountain.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      951 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.free.adsl-fiber.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      402 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.free.mobile.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      377 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.free.mobile2.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      390 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.futur.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      369 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.ge-iroise.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      393 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.greffe-tc-lyon.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      516 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.hiscox.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      364 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.internetsatellite.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      409 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.jpg.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      515 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.kubii.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      472 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.laposte.boutique.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      383 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.laposte.coliposte.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      572 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.lecab.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      386 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.leroymerlin.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      491 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.maaf.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      373 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.mediapart.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      368 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.moneo-resto.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      551 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.mouser.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      403 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.mycelium-roulement.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      435 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.napsis.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      463 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.nexity.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      445 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.orange.fibre.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      492 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.orange.fixedline.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      366 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.prestaclic.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      475 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.publicationannoncelegale.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      433 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.sfr.adsl-fiber.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      341 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.sfr.mobile.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      423 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.sosh.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      387 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.teledec.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      430 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.topoffice.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      459 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/net.online.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      438 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/fr/net.scaleway.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.108954 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1000 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.action.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1347 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.albron.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2847 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.be.coolblue.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1458 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.begra.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1733 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.blokker.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      685 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.bunq.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      435 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.cpe.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1923 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.farnell.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      918 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.ferbox.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1268 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.gamma.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1689 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.goos.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1190 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.karwei.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      715 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.kav.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1063 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.koffiehenk.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1438 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.praxis.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      475 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.reclameland.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2040 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.saeco.philips.eluscious.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      414 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.simpel.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      868 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.transip.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1681 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.tuynder.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      344 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.vistaprint.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      495 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.vodafone.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      454 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.wasco.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1592 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.weid.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      631 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.yezzer.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      358 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.zinkunie.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.109954 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      786 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.bmw-fs.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      918 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.insert.subiekt-gt.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      662 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.insert.subiekt-nexo.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      687 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.orlen.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      950 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.p4.yml
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1175 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.paypro.yml
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.109954 invoice2data-0.4.3/src/invoice2data/input/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/__init__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     3021 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/gvision.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     3830 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/ocrmypdf.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1399 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/pdfminer_wrapper.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1280 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/pdfplumber.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2057 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/pdftotext.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     4988 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/tesseract.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)      106 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/input/text.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     9892 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/main.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.110954 invoice2data-0.4.3/src/invoice2data/output/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/output/__init__.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1712 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/output/to_csv.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1627 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/output/to_json.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     1916 2023-03-31 21:46:18.000000 invoice2data-0.4.3/src/invoice2data/output/to_xml.py
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.091954 invoice2data-0.4.3/src/invoice2data.egg-info/
--rw-r--r--   0 emiel     (1000) emiel     (1000)    10815 2023-03-31 22:24:33.000000 invoice2data-0.4.3/src/invoice2data.egg-info/PKG-INFO
--rw-r--r--   0 emiel     (1000) emiel     (1000)    11154 2023-03-31 22:24:33.000000 invoice2data-0.4.3/src/invoice2data.egg-info/SOURCES.txt
--rw-r--r--   0 emiel     (1000) emiel     (1000)        1 2023-03-31 22:24:33.000000 invoice2data-0.4.3/src/invoice2data.egg-info/dependency_links.txt
--rw-r--r--   0 emiel     (1000) emiel     (1000)       56 2023-03-31 22:24:33.000000 invoice2data-0.4.3/src/invoice2data.egg-info/entry_points.txt
--rw-r--r--   0 emiel     (1000) emiel     (1000)       86 2023-03-31 22:24:33.000000 invoice2data-0.4.3/src/invoice2data.egg-info/requires.txt
--rw-r--r--   0 emiel     (1000) emiel     (1000)       13 2023-03-31 22:24:33.000000 invoice2data-0.4.3/src/invoice2data.egg-info/top_level.txt
-drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-03-31 22:24:33.110954 invoice2data-0.4.3/tests/
--rw-rw-r--   0 emiel     (1000) emiel     (1000)    13074 2023-03-31 21:46:18.000000 invoice2data-0.4.3/tests/test_cli.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     2173 2023-03-31 21:46:18.000000 invoice2data-0.4.3/tests/test_extraction.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     4930 2023-03-31 21:46:18.000000 invoice2data-0.4.3/tests/test_invoice_template.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     4694 2023-03-31 21:46:18.000000 invoice2data-0.4.3/tests/test_lib.py
--rw-rw-r--   0 emiel     (1000) emiel     (1000)     3291 2023-03-31 21:46:18.000000 invoice2data-0.4.3/tests/test_loader.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.789347 invoice2data-0.4.4/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1078 2023-04-08 21:16:58.000000 invoice2data-0.4.4/LICENSE.txt
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      124 2023-04-08 21:16:58.000000 invoice2data-0.4.4/MANIFEST.in
+-rw-r--r--   0 emiel     (1000) emiel     (1000)    12359 2023-04-08 21:29:05.789347 invoice2data-0.4.4/PKG-INFO
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)    11286 2023-04-08 21:16:58.000000 invoice2data-0.4.4/README.md
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1657 2023-04-08 21:29:05.790347 invoice2data-0.4.4/setup.cfg
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      442 2023-04-08 21:16:58.000000 invoice2data-0.4.4/setup.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.777347 invoice2data-0.4.4/src/
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.778347 invoice2data-0.4.4/src/invoice2data/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)       45 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/__init__.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.779347 invoice2data-0.4.4/src/invoice2data/extract/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/__init__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)    12061 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/invoice_template.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     4091 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/loader.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.779347 invoice2data-0.4.4/src/invoice2data/extract/parsers/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      135 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/parsers/__init__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      658 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/parsers/__interface__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     7742 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/parsers/lines.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2663 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/parsers/regex.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      437 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/parsers/static.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.780347 invoice2data-0.4.4/src/invoice2data/extract/plugins/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/plugins/__init__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      545 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/plugins/__interface__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      401 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/plugins/lines.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     3503 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/plugins/tables.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.777347 invoice2data-0.4.4/src/invoice2data/extract/templates/
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.780347 invoice2data-0.4.4/src/invoice2data/extract/templates/au/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1375 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/au/au.com.opal.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      484 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/au/au.com.telstra.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.781347 invoice2data-0.4.4/src/invoice2data/extract/templates/be/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1628 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.accor.invest.ibis.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      305 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.boucherie.pochet.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      311 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.cebeo.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      797 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.lampiris.facture-dacompte.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      425 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.lampiris.factuur.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      727 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.lampiris.regularisation.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      306 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.melchior-vins.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      323 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.proximus.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      700 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.scarlet.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      349 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.securex.social.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.781347 invoice2data-0.4.4/src/invoice2data/extract/templates/ch/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      443 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/ch/ch.pcengines.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.783347 invoice2data-0.4.4/src/invoice2data/extract/templates/com/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     5363 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.AzureInterior.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      657 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.amazon.aws.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      531 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.apple.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      212 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.apps4rent.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      485 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.binarylife.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      436 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.bloomberg.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      252 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.cloudns.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      544 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.datadoghq.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      242 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.digitalocean.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      233 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.envato.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      379 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.expressvpn.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1244 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.expressvpn_prio6.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      361 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.ftserussell.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      250 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.github.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      274 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.globalsign.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      368 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.google.adwords.hk.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      199 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.hobohost.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      346 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.jamiepro.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      373 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.linode.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      282 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.microsoftonline.hk-v2017.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      290 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.microsoftonline.hk.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      480 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.mongodb.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      732 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.namecheap.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      239 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.namesilo.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      510 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.newrelic.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1346 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.nl.lenovo.digitalriver.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      445 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.nmmn.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      196 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.nodisto.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      392 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.nyse.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      775 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.oyo.invoice.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      359 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.packtpub.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      579 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.pixartprinting.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      550 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.sammymaystone.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      247 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.scaleway.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      241 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.textmaster.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      388 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.tmx.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      312 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.travis-ci.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      320 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.twitter.de.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      305 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.twitter.uk.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      304 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.twitter.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      231 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.upwork.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      205 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.usersnap.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.783347 invoice2data-0.4.4/src/invoice2data/extract/templates/de/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      342 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.amazon.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      357 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.bettina-kast.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2410 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.digikey.com.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      310 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.hosteurope.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      501 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.notebooksbilligerBillPay.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      276 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.ovh.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      544 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.qualityhosting.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      343 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.united-domains.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.783347 invoice2data-0.4.4/src/invoice2data/extract/templates/es/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      398 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/es/com.pepephone.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      384 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/es/es.supplies24.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.787347 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      484 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/co.mooncard.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      374 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.adobe.ie.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      374 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.akretion.fr.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      431 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.amazon.aws.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      366 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.ateliercopieservice.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      539 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.chauffeur-prive.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      430 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.coriolis.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      387 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.easyjet.fr.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      596 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.eaudugrandlyon.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      315 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.godaddy.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      444 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.google.ie.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      389 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.hootsuite.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      397 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.jeanbesson.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      399 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.ldlc.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      367 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.linkedin.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      377 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.mention.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      421 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.microsoft.ie.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      402 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.myflyingbox.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      402 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.officetimeline.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      481 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.orange-business.mobile.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      363 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.ovh.fr.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      428 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.rs-online.fr.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      464 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.saur.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      383 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.soyoustart.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      358 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.vinci-autoroutes.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2151 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/dolibarr.generique.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      476 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/eu.trainline.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      570 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.actn.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      373 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.airfrance.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      427 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.also.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      376 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.amazon.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      399 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.assurance-epargne-pension.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      597 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.bouyguestelecom.adsl-fiber.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      451 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.bouyguestelecom.mobile.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      531 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.butagaz.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      389 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.chronopost.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      392 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.dirafi.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      351 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.domaine-achat.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      423 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.easytrip.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      471 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.edf.entreprises.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     3648 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.edf.pme.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      450 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.finagaz.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      454 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.fountain.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      951 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.free.adsl-fiber.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      402 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.free.mobile.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      377 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.free.mobile2.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      390 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.futur.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      369 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.ge-iroise.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      393 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.greffe-tc-lyon.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      516 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.hiscox.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      364 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.internetsatellite.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      409 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.jpg.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      515 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.kubii.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      472 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.laposte.boutique.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      383 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.laposte.coliposte.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      572 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.lecab.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      386 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.leroymerlin.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      491 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.maaf.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      373 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.mediapart.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      368 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.moneo-resto.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      551 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.mouser.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      403 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.mycelium-roulement.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      435 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.napsis.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      463 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.nexity.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      445 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.orange.fibre.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      492 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.orange.fixedline.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      366 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.prestaclic.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      475 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.publicationannoncelegale.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      433 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.sfr.adsl-fiber.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      341 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.sfr.mobile.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      423 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.sosh.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      387 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.teledec.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      430 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.topoffice.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      459 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/net.online.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      438 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/fr/net.scaleway.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.788347 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1000 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.action.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1347 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.albron.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2847 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.be.coolblue.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1458 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.begra.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1733 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.blokker.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      685 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.bunq.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      435 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.cpe.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1923 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.farnell.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      918 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.ferbox.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1268 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.gamma.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1689 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.goos.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1190 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.karwei.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      715 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.kav.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1063 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.koffiehenk.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1438 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.praxis.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      475 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.reclameland.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2040 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.saeco.philips.eluscious.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      414 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.simpel.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      868 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.transip.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1681 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.tuynder.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      344 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.vistaprint.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      495 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.vodafone.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      454 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.wasco.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1592 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.weid.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      631 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.yezzer.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      358 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.zinkunie.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.788347 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      786 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.bmw-fs.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      918 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.insert.subiekt-gt.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      662 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.insert.subiekt-nexo.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      687 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.orlen.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      950 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.p4.yml
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1175 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.paypro.yml
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.789347 invoice2data-0.4.4/src/invoice2data/input/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/__init__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     3021 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/gvision.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     3830 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/ocrmypdf.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1399 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/pdfminer_wrapper.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1280 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/pdfplumber.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2057 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/pdftotext.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     4988 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/tesseract.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)      106 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/input/text.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)    10155 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/main.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.789347 invoice2data-0.4.4/src/invoice2data/output/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/output/__init__.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1712 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/output/to_csv.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1627 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/output/to_json.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     1916 2023-04-08 21:16:58.000000 invoice2data-0.4.4/src/invoice2data/output/to_xml.py
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.779347 invoice2data-0.4.4/src/invoice2data.egg-info/
+-rw-r--r--   0 emiel     (1000) emiel     (1000)    12359 2023-04-08 21:29:05.000000 invoice2data-0.4.4/src/invoice2data.egg-info/PKG-INFO
+-rw-r--r--   0 emiel     (1000) emiel     (1000)    11154 2023-04-08 21:29:05.000000 invoice2data-0.4.4/src/invoice2data.egg-info/SOURCES.txt
+-rw-r--r--   0 emiel     (1000) emiel     (1000)        1 2023-04-08 21:29:05.000000 invoice2data-0.4.4/src/invoice2data.egg-info/dependency_links.txt
+-rw-r--r--   0 emiel     (1000) emiel     (1000)       56 2023-04-08 21:29:05.000000 invoice2data-0.4.4/src/invoice2data.egg-info/entry_points.txt
+-rw-r--r--   0 emiel     (1000) emiel     (1000)       86 2023-04-08 21:29:05.000000 invoice2data-0.4.4/src/invoice2data.egg-info/requires.txt
+-rw-r--r--   0 emiel     (1000) emiel     (1000)       13 2023-04-08 21:29:05.000000 invoice2data-0.4.4/src/invoice2data.egg-info/top_level.txt
+drwxr-xr-x   0 emiel     (1000) emiel     (1000)        0 2023-04-08 21:29:05.789347 invoice2data-0.4.4/tests/
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)    13074 2023-04-08 21:16:58.000000 invoice2data-0.4.4/tests/test_cli.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     2173 2023-04-08 21:16:58.000000 invoice2data-0.4.4/tests/test_extraction.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     4930 2023-04-08 21:16:58.000000 invoice2data-0.4.4/tests/test_invoice_template.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     4784 2023-04-08 21:16:58.000000 invoice2data-0.4.4/tests/test_lib.py
+-rw-rw-r--   0 emiel     (1000) emiel     (1000)     3291 2023-04-08 21:16:58.000000 invoice2data-0.4.4/tests/test_loader.py
```

### Comparing `invoice2data-0.4.3/LICENSE.txt` & `invoice2data-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/PKG-INFO` & `invoice2data-0.4.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoice2data
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python parser to extract data from pdf invoice
 Home-page: https://github.com/invoice-x/invoice2data
 Author: Manuel Riel
 License: MIT License
 Keywords: pdf,invoicing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
@@ -55,14 +55,63 @@
 Go from PDF files to this:
 
     {'date': (2014, 5, 7), 'invoice_number': '30064443', 'amount': 34.73, 'desc': 'Invoice 30064443 from QualityHosting', 'lines': [{'price': 42.0, 'desc': u'Small Business StandardExchange 2010\nGrundgeb\xfchr pro Einheit\nDienst: OUDJQ_office\n01.05.14-31.05.14\n', 'pos': u'7', 'qty': 1.0}]}
     {'date': (2014, 6, 4), 'invoice_number': 'EUVINS1-OF5-DE-120725895', 'amount': 35.24, 'desc': 'Invoice EUVINS1-OF5-DE-120725895 from Amazon EU'}
     {'date': (2014, 8, 3), 'invoice_number': '42183017', 'amount': 4.11, 'desc': 'Invoice 42183017 from Amazon Web Services'}
     {'date': (2015, 1, 28), 'invoice_number': '12429647', 'amount': 101.0, 'desc': 'Invoice 12429647 from Envato'}
 
+```mermaid
+flowchart LR
+
+    InvoiceFile[fa:fa-file-invoice Invoicefile\n\npdf\nimage\ntext] --> Input-module(Input Module\n\npdftotext\ntext\npdfminer\npdfplumber\ntesseract\ngvision)
+
+    Input-module --> |Extracted Text| C{keyword\nmatching}
+
+    Invoice-Templates[(fa:fa-file-lines Invoice Templates)] --> C{keyword\nmatching}
+
+    C --> |Extracted Text + fa:fa-file-circle-check Template| E(Template Processing\n apply options from template\nremove accents, replaces etc...)
+
+    E --> |Optimized String|Plugins&Parsers(Call plugins + parsers)
+
+    subgraph Plugins&Parsers
+
+      direction BT
+
+        tables[fa:fa-table tables] ~~~ lines[fa:fa-grip-lines lines]
+
+        lines ~~~ regex[fa:fa-code regex]
+
+        regex ~~~ static[fa:fa-check static]
+
+ 
+
+    end
+
+    Plugins&Parsers --> |output| result[result\nfa:fa-file-csv,\njson,\nXML]
+
+ 
+
+ click Invoice-Templates https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md
+
+ click result https://github.com/invoice-x/invoice2data#usage
+
+ click Input-module https://github.com/invoice-x/invoice2data#installation-of-input-modules
+
+ click E https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#options
+
+ click tables https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#tables
+
+ click lines https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#lines
+
+ click regex https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#regex
+
+ click static https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#parser-static
+
+```
+
 ## Installation
 
 1.  Install pdftotext
 
 If possible get the latest
 [xpdf/poppler-utils](https://poppler.freedesktop.org/) version. It's
 included with macOS Homebrew, Debian and Ubuntu. Without it, `pdftotext`
```

### Comparing `invoice2data-0.4.3/README.md` & `invoice2data-0.4.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,63 @@
 Go from PDF files to this:
 
     {'date': (2014, 5, 7), 'invoice_number': '30064443', 'amount': 34.73, 'desc': 'Invoice 30064443 from QualityHosting', 'lines': [{'price': 42.0, 'desc': u'Small Business StandardExchange 2010\nGrundgeb\xfchr pro Einheit\nDienst: OUDJQ_office\n01.05.14-31.05.14\n', 'pos': u'7', 'qty': 1.0}]}
     {'date': (2014, 6, 4), 'invoice_number': 'EUVINS1-OF5-DE-120725895', 'amount': 35.24, 'desc': 'Invoice EUVINS1-OF5-DE-120725895 from Amazon EU'}
     {'date': (2014, 8, 3), 'invoice_number': '42183017', 'amount': 4.11, 'desc': 'Invoice 42183017 from Amazon Web Services'}
     {'date': (2015, 1, 28), 'invoice_number': '12429647', 'amount': 101.0, 'desc': 'Invoice 12429647 from Envato'}
 
+```mermaid
+flowchart LR
+
+    InvoiceFile[fa:fa-file-invoice Invoicefile\n\npdf\nimage\ntext] --> Input-module(Input Module\n\npdftotext\ntext\npdfminer\npdfplumber\ntesseract\ngvision)
+
+    Input-module --> |Extracted Text| C{keyword\nmatching}
+
+    Invoice-Templates[(fa:fa-file-lines Invoice Templates)] --> C{keyword\nmatching}
+
+    C --> |Extracted Text + fa:fa-file-circle-check Template| E(Template Processing\n apply options from template\nremove accents, replaces etc...)
+
+    E --> |Optimized String|Plugins&Parsers(Call plugins + parsers)
+
+    subgraph Plugins&Parsers
+
+      direction BT
+
+        tables[fa:fa-table tables] ~~~ lines[fa:fa-grip-lines lines]
+
+        lines ~~~ regex[fa:fa-code regex]
+
+        regex ~~~ static[fa:fa-check static]
+
+ 
+
+    end
+
+    Plugins&Parsers --> |output| result[result\nfa:fa-file-csv,\njson,\nXML]
+
+ 
+
+ click Invoice-Templates https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md
+
+ click result https://github.com/invoice-x/invoice2data#usage
+
+ click Input-module https://github.com/invoice-x/invoice2data#installation-of-input-modules
+
+ click E https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#options
+
+ click tables https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#tables
+
+ click lines https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#lines
+
+ click regex https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#regex
+
+ click static https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#parser-static
+
+```
+
 ## Installation
 
 1.  Install pdftotext
 
 If possible get the latest
 [xpdf/poppler-utils](https://poppler.freedesktop.org/) version. It's
 included with macOS Homebrew, Debian and Ubuntu. Without it, `pdftotext`
```

### Comparing `invoice2data-0.4.3/setup.cfg` & `invoice2data-0.4.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [metadata]
 name = invoice2data
 author = Manuel Riel
 description = Python parser to extract data from pdf invoice
-version = 0.4.3
+version = 0.4.4
 url = https://github.com/invoice-x/invoice2data
 keywords = 
 	pdf
 	invoicing
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Environment :: MacOS X
```

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/invoice_template.py` & `invoice2data-0.4.4/src/invoice2data/extract/invoice_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                     optimized_str_for_parser = optimized_str
                 if "parser" in v:
                     # parser is required and may require additional options
                     # e.g. "parser: regex" requires "regex: [pattern]"
                     if v["parser"] in PARSERS_MAPPING:
                         parser = PARSERS_MAPPING[v["parser"]]
                         value = parser.parse(self, k, v, optimized_str_for_parser)
-                        if value:
+                        if value or value == 0.0:
                             output[k] = value
                         else:
                             logger.warning("Failed to parse field %s with parser %s", k, v["parser"])
                     else:
                         logger.error("Field %s has unknown parser %s set", k, v["parser"])
                 else:
                     logger.error("Field %s doesn't have parser specified", k)
@@ -276,8 +276,10 @@
             logger.error(
                 "Unable to match all required fields. "
                 "The required fields are: {0}. "
                 "Output contains the following fields: {1}.".format(
                     required_fields, fields
                 )
             )
+            missing = set(required_fields) - set(fields)
+            raise ValueError("Unable to parse required field(s): {0}".format(missing))
             return None
```

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/loader.py` & `invoice2data-0.4.4/src/invoice2data/extract/loader.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/parsers/__interface__.py` & `invoice2data-0.4.4/src/invoice2data/extract/parsers/__interface__.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/parsers/lines.py` & `invoice2data-0.4.4/src/invoice2data/extract/parsers/lines.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/parsers/regex.py` & `invoice2data-0.4.4/src/invoice2data/extract/parsers/regex.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/plugins/__interface__.py` & `invoice2data-0.4.4/src/invoice2data/extract/plugins/__interface__.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/plugins/tables.py` & `invoice2data-0.4.4/src/invoice2data/extract/plugins/tables.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/au/au.com.opal.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/au/au.com.opal.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.accor.invest.ibis.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.accor.invest.ibis.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.lampiris.facture-dacompte.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.lampiris.facture-dacompte.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.lampiris.regularisation.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.lampiris.regularisation.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/be/be.scarlet.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/be/be.scarlet.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.AzureInterior.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.AzureInterior.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.amazon.aws.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.amazon.aws.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.apple.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.apple.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.datadoghq.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.datadoghq.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.expressvpn_prio6.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.expressvpn_prio6.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.namecheap.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.namecheap.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.nl.lenovo.digitalriver.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.nl.lenovo.digitalriver.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.oyo.invoice.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.oyo.invoice.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.pixartprinting.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.pixartprinting.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/com/com.sammymaystone.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/com/com.sammymaystone.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.digikey.com.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.digikey.com.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/de/de.qualityhosting.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/de/de.qualityhosting.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.chauffeur-prive.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.chauffeur-prive.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/com.eaudugrandlyon.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/com.eaudugrandlyon.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/dolibarr.generique.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/dolibarr.generique.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.actn.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.actn.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.bouyguestelecom.adsl-fiber.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.bouyguestelecom.adsl-fiber.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.butagaz.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.butagaz.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.edf.pme.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.edf.pme.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.free.adsl-fiber.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.free.adsl-fiber.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.hiscox.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.hiscox.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.kubii.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.kubii.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.lecab.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.lecab.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/fr/fr.mouser.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/fr/fr.mouser.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.action.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.action.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.albron.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.albron.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.be.coolblue.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.be.coolblue.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.begra.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.begra.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.blokker.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.blokker.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.bunq.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.bunq.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.farnell.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.farnell.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.ferbox.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.ferbox.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.gamma.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.gamma.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.goos.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.goos.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.karwei.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.karwei.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.kav.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.kav.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.koffiehenk.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.koffiehenk.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.praxis.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.praxis.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.saeco.philips.eluscious.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.saeco.philips.eluscious.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.transip.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.transip.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.tuynder.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.tuynder.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.weid.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.weid.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/nl/nl.yezzer.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/nl/nl.yezzer.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.bmw-fs.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.bmw-fs.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.insert.subiekt-gt.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.insert.subiekt-gt.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.insert.subiekt-nexo.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.insert.subiekt-nexo.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.orlen.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.orlen.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.p4.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.p4.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/extract/templates/pl/pl.paypro.yml` & `invoice2data-0.4.4/src/invoice2data/extract/templates/pl/pl.paypro.yml`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/input/gvision.py` & `invoice2data-0.4.4/src/invoice2data/input/gvision.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/input/ocrmypdf.py` & `invoice2data-0.4.4/src/invoice2data/input/ocrmypdf.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/input/pdfminer_wrapper.py` & `invoice2data-0.4.4/src/invoice2data/input/pdfminer_wrapper.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/input/pdfplumber.py` & `invoice2data-0.4.4/src/invoice2data/input/pdfplumber.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/input/pdftotext.py` & `invoice2data-0.4.4/src/invoice2data/input/pdftotext.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/input/tesseract.py` & `invoice2data-0.4.4/src/invoice2data/input/tesseract.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/main.py` & `invoice2data-0.4.4/src/invoice2data/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,17 +84,19 @@
 
         formatter = logging.Formatter(self.FORMAT)
         return formatter.format(record)
 
 
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(ColorLogFormatter())
-logger.addHandler(stream_handler)
 logger.propagate = False
 
+if not logger.handlers:
+    logger.addHandler(stream_handler)
+
 
 def extract_data(invoicefile, templates=None, input_module=None):
     """Extracts structured data from PDF/image invoices.
 
     This function uses the text extracted from a PDF file or image and
     pre-defined regex templates to find structured data.
 
@@ -289,33 +291,37 @@
 
     # Load internal templates, if not disabled.
 
     if not args.exclude_built_in_templates:
         templates += read_templates()
     output = []
     for f in args.input_files:
-        res = extract_data(f.name, templates=templates, input_module=input_module)
-        if res:
-            logger.info(res)
-            output.append(res)
-
-            kwargs = copy.deepcopy(res)
-            for key, value in kwargs.items():
-                if type(value) is list and len(value) >= 1:
-                    kwargs[key] = value[0]
-            for key, value in kwargs.items():
-                if type(value) is datetime.datetime:
-                    kwargs[key] = value.strftime('%Y-%m-%d')
-            if args.copy:
-                filename = args.filename.format(**kwargs)
-                shutil.copyfile(f.name, join(args.copy, filename))
-            if args.move:
-                filename = args.filename.format(**kwargs)
-                shutil.move(f.name, join(args.move, filename))
-        f.close()
+        try:
+            res = extract_data(f.name, templates=templates, input_module=input_module)
+            if res:
+                logger.info(res)
+                output.append(res)
+
+                kwargs = copy.deepcopy(res)
+                for key, value in kwargs.items():
+                    if type(value) is list and len(value) >= 1:
+                        kwargs[key] = value[0]
+                for key, value in kwargs.items():
+                    if type(value) is datetime.datetime:
+                        kwargs[key] = value.strftime('%Y-%m-%d')
+                if args.copy:
+                    filename = args.filename.format(**kwargs)
+                    shutil.copyfile(f.name, join(args.copy, filename))
+                if args.move:
+                    filename = args.filename.format(**kwargs)
+                    shutil.move(f.name, join(args.move, filename))
+            f.close()
+        except Exception as e:
+            logger.critical("Invoice2data failed to process %s. \nError message: %s", f.name, e)
+            continue
 
     if output_module is not None:
         output_module.write_to_file(output, args.output_name, args.output_date_format)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `invoice2data-0.4.3/src/invoice2data/output/to_csv.py` & `invoice2data-0.4.4/src/invoice2data/output/to_csv.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/output/to_json.py` & `invoice2data-0.4.4/src/invoice2data/output/to_json.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data/output/to_xml.py` & `invoice2data-0.4.4/src/invoice2data/output/to_xml.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/src/invoice2data.egg-info/PKG-INFO` & `invoice2data-0.4.4/src/invoice2data.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invoice2data
-Version: 0.4.3
+Version: 0.4.4
 Summary: Python parser to extract data from pdf invoice
 Home-page: https://github.com/invoice-x/invoice2data
 Author: Manuel Riel
 License: MIT License
 Keywords: pdf,invoicing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: MacOS X
@@ -55,14 +55,63 @@
 Go from PDF files to this:
 
     {'date': (2014, 5, 7), 'invoice_number': '30064443', 'amount': 34.73, 'desc': 'Invoice 30064443 from QualityHosting', 'lines': [{'price': 42.0, 'desc': u'Small Business StandardExchange 2010\nGrundgeb\xfchr pro Einheit\nDienst: OUDJQ_office\n01.05.14-31.05.14\n', 'pos': u'7', 'qty': 1.0}]}
     {'date': (2014, 6, 4), 'invoice_number': 'EUVINS1-OF5-DE-120725895', 'amount': 35.24, 'desc': 'Invoice EUVINS1-OF5-DE-120725895 from Amazon EU'}
     {'date': (2014, 8, 3), 'invoice_number': '42183017', 'amount': 4.11, 'desc': 'Invoice 42183017 from Amazon Web Services'}
     {'date': (2015, 1, 28), 'invoice_number': '12429647', 'amount': 101.0, 'desc': 'Invoice 12429647 from Envato'}
 
+```mermaid
+flowchart LR
+
+    InvoiceFile[fa:fa-file-invoice Invoicefile\n\npdf\nimage\ntext] --> Input-module(Input Module\n\npdftotext\ntext\npdfminer\npdfplumber\ntesseract\ngvision)
+
+    Input-module --> |Extracted Text| C{keyword\nmatching}
+
+    Invoice-Templates[(fa:fa-file-lines Invoice Templates)] --> C{keyword\nmatching}
+
+    C --> |Extracted Text + fa:fa-file-circle-check Template| E(Template Processing\n apply options from template\nremove accents, replaces etc...)
+
+    E --> |Optimized String|Plugins&Parsers(Call plugins + parsers)
+
+    subgraph Plugins&Parsers
+
+      direction BT
+
+        tables[fa:fa-table tables] ~~~ lines[fa:fa-grip-lines lines]
+
+        lines ~~~ regex[fa:fa-code regex]
+
+        regex ~~~ static[fa:fa-check static]
+
+ 
+
+    end
+
+    Plugins&Parsers --> |output| result[result\nfa:fa-file-csv,\njson,\nXML]
+
+ 
+
+ click Invoice-Templates https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md
+
+ click result https://github.com/invoice-x/invoice2data#usage
+
+ click Input-module https://github.com/invoice-x/invoice2data#installation-of-input-modules
+
+ click E https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#options
+
+ click tables https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#tables
+
+ click lines https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#lines
+
+ click regex https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#regex
+
+ click static https://github.com/invoice-x/invoice2data/blob/master/TUTORIAL.md#parser-static
+
+```
+
 ## Installation
 
 1.  Install pdftotext
 
 If possible get the latest
 [xpdf/poppler-utils](https://poppler.freedesktop.org/) version. It's
 included with macOS Homebrew, Debian and Ubuntu. Without it, `pdftotext`
```

### Comparing `invoice2data-0.4.3/src/invoice2data.egg-info/SOURCES.txt` & `invoice2data-0.4.4/src/invoice2data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/tests/test_cli.py` & `invoice2data-0.4.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/tests/test_extraction.py` & `invoice2data-0.4.4/tests/test_extraction.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/tests/test_invoice_template.py` & `invoice2data-0.4.4/tests/test_invoice_template.py`

 * *Files identical despite different names*

### Comparing `invoice2data-0.4.3/tests/test_lib.py` & `invoice2data-0.4.4/tests/test_lib.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,27 +86,30 @@
         to_csv.write_to_file(dump_dict, file_path)
         self.assertTrue(os.path.exists(file_path), "File not made")
         os.remove(file_path)
 
     def test_extract_data_pdfminer(self):
         pdf_files = get_sample_files('.pdf')
         for file in pdf_files:
-            print("Testing pdfminer with file", file)
-            try:
-                res = extract_data(file, None, pdfminer_wrapper)
-                print(res)  # Check why logger.info is not working, for the time being using print
-            except ImportError:
-                # print("pdfminer module not installed!")
-                self.assertTrue(False, "pdfminer is not installed")
-                self.assertTrue(type(res) is str, "return is not a string")
+            if file.endswith("NetpresseInvoice.pdf"):
+                print("Testing pdfminer with file", file)
+                try:
+                    res = extract_data(file, None, pdfminer_wrapper)
+                    print(res)
+                except ImportError:
+                    self.assertTrue(False, "pdfminer is not installed")
+                    self.assertTrue(type(res) is str, "return is not a string")
 
     @needs_pdfplumber
     def test_extract_data_pdfplumber(self):
         pdf_files = get_sample_files('.pdf')
         for file in pdf_files:
+            if not file.endswith("FlipkartInvoice.pdf"):
+                continue
+            print("Testing pdfplumber with file", file)
             extract_data(file, None, pdfplumber)
 
     def test_tesseract_for_return(self):
         png_files = get_sample_files('.png')
         for file in png_files:
             if tesseract.to_text(file) is None:
                 self.assertTrue(False, "Tesseract returned None")
```

### Comparing `invoice2data-0.4.3/tests/test_loader.py` & `invoice2data-0.4.4/tests/test_loader.py`

 * *Files identical despite different names*

