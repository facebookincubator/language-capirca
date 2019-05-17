# Capirca syntax highlighting for Atom  

Adds syntax highlighting for Capirca filetypes in Atom. Capirca is an open source standard for writing vendor-neutral firewall policies as originally released by Google: https://github.com/google/capirca

## Features
Included with this package are the following:

 - Syntax highlighting for many different term keywords, comments, network and service group definitions, accept/deny statements, and header values.
 - The following filetypes will be automatically highlighted: `.pol`, `.inc`, `.net`, and `.svc`. 
 - [Atom code snippets](http://flight-manual.atom.io/using-atom/sections/snippets/) are included to make writing terms, network definitions, and service definitions easier.

Here's a preview with the Dark Room Contrast theme:
![screen shot 2017-05-30 at 3 04 09 pm](https://cloud.githubusercontent.com/assets/7231007/26607065/764c22f8-4549-11e7-9275-ac3c28079954.png)

## Installation
Simply open up settings in Atom (`Cmd-,`), go to `Install`, and search the `packages` section for `language-capirca`. It's a one click install from there.   

## Snippets
The following snippets are included, as you type in a file with the Capirca syntax selected, you'll see these options show up in the typeahead suggestion window:

Snippet  |  Typeahead keyword  |  Expansion
-------- | ------- | --------
New Term  |      term  |  A full term with several of the common keywords
New Header  |      header  |  A header with a default target
New Include  |      include   |   `#include include.inc`
New Network Group  |      net   |  `NAME = member1`
New Service Group  |      svc   |  `NAME = member1`
Single TCP Port  |      tcp   |  `port/tcp`
TCP Port Range  |      tcpr   |  `port1-port2/tcp`
Single UDP Port  |      udp   |  `port/udp`
UDP Port Range  |      udpr   |  `port1-port2/udp`
Source Address  |      source-address   |  `source-address:: address_group`
Source Port  |      source-port   |  `source-port:: service_group`
Destination Address  |      destination-address   |  `destination-address:: address_group`
Destination Port  |      destination-port   |  `destination-port:: service_group`
TCP Protocol  |      protocol   |  `protocol:: tcp`
UDP Protocol  |      protocolu   |  `protocol:: udp`
Comment  |      comment   |  `comment:: "text"`
Accept Action  |      action   |  `action:: accept`
Deny Action  |      actiond   |  `action:: deny`
Counter  |      counter   |  `counter:: name`
Expiration  |      expiration   |  `expiration: 2020-01-01`
Logging  |      logging   |  `logging:: true`

## Contributing
The CONTRIBUTING.md file has all the information you need to help out if you find a bug or have a new feature you want to add.

## License
`language-capirca` is BSD-licensed.
