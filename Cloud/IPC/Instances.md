---
title: Infomaniak Public Cloud - Gestion des instances
description: Créer et gérer les instances
published: true
date: 2021-11-04T15:50:38.458Z
tags: infomaniak, public-cloud, cloud, ipc, vm, instance
editor: markdown
dateCreated: 2021-11-04T12:38:36.261Z
---

# Horizon
# Créer une instance
## Rendez vous dans la section 'Instance' et cliquez sur `Lancer une instance`
![infomaniak-publiccloud_5_1.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_1.png =1300x)

### Nommez votre instance, choississez le nombre et cliquez sur `suivant`
![infomaniak-publiccloud_5_2.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_2.png =600x)

### Selectionnez l'image et cliquez sur `Suivant`
![infomaniak-publiccloud_5_3.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_3.png =600x)

### Choissisez la configuration souhaitée et cliquez sur `Suivant`
![infomaniak-publiccloud_5_4.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_4.png =600x)


### Puis le réseau et cliquez sur `Suivant`
![infomaniak-publiccloud_5_5.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_5.png =600x)


### Vous pouvez modifier les autres options ou directement cliquer sur `Lancer l'instance`
![infomaniak-publiccloud_5_6.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_6.png =600x)


> Votre instance est démarrée !
> ![infomaniak-publiccloud_5_7.png](/images/cloud/infomaniak-public-cloud/5/infomaniak-publiccloud_5_7.png =1300x)
{.is-success}

> Vous ne pouvez pas encore vous y connecter en SSH, il vous manque la configuration d'un groupe de sécurité ! Voir ce tutoriel : 
{.is-warning}
 - [🛡️ Les groupes de sécurité *Comprendre et utiliser le firewall et ses règles*](/Cloud/Cloud/IPC/Security-Groups)
{.links-list}

# CLI
## Lister les configurations disponibles

## Lister les réseaux disponibles

## Créer une instance
```bash
openstack server create
    (--image <IMAGE> | --volume <VOLUME>)
    --flavor <FLAVOR>
    [--security-group <SECURITY_GROUP>]
    [--key-name <KEY_NAME>]
    [--network <NETWORK>]
    <SERVER_NAME>
```
> **--image *IMAGE***
> - Créer un disque de démarrage du serveur à partir de cette image (nom ou ID)
>
> **--volume *VOLUME***
> - Créez un serveur en utilisant ce volume comme disque de démarrage (nom ou ID).
>
> **--flavor *FLAVOR***
> - Créer un serveur avec cette configuration (nom ou ID)
>
> **--security-group *SECURITY_GROUP***
> - Groupe de sécurité à attribuer à ce serveur (nom ou ID) (répétez l'option pour définir plusieurs groupes)
>
> **--key-name *KEY_NAME***
> - Paire de clés à injecter dans ce serveur 
>
> **--network *NETWORK***
> - Créez une carte réseau sur le serveur et connectez-la au réseau. (nom ou ID)
>
> ***SERVER_NAME***
> - Nom du serveur à créer
>
> 	.
{.is-info}

## Lister les instances

## Supprimer une instance


