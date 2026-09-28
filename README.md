# Network Analysis with Wireshark

Laboratoire pédagogique d'observation des protocoles et de diagnostic réseau avec Wireshark. Les captures doivent provenir exclusivement de systèmes personnels autorisés, du laboratoire ou de sources explicitement légales.

## Objectif

- reconnaître les échanges ARP, DNS, TCP, ICMP et HTTP/HTTPS ;
- construire des filtres d'affichage lisibles ;
- relier une capture à un symptôme réseau ;
- distinguer contenu observable, métadonnées et trafic chiffré ;
- rédiger une analyse reproductible sans exposer de données sensibles.

## Architecture

Un client, un service de test et éventuellement une passerelle de laboratoire sont reliés à un réseau virtuel isolé. Wireshark capture uniquement sur une interface appartenant à l'auteur du lab.

`TODO: ajouter le schéma correspondant à l'environnement réellement utilisé.`

## Environnement technique

- Wireshark : `TODO: version à compléter après installation.`
- systèmes : `TODO: à compléter après réalisation du lab.`
- réseau virtuel privé ;
- service HTTP local facultatif pour les comparaisons HTTP/HTTPS.

## Prérequis

- autorisation de capturer le trafic étudié ;
- interface du laboratoire clairement identifiée ;
- absence de comptes réels, cookies ou données personnelles ;
- synchronisation horaire ;
- stockage des PCAP hors Git tant qu'ils n'ont pas été contrôlés.

## Mise en place

1. Créer un réseau isolé et démarrer les hôtes de test.
2. Fermer les applications inutiles pour réduire le bruit.
3. Choisir l'interface exacte dans Wireshark.
4. Capturer une courte fenêtre autour de l'action prévue.
5. Arrêter puis sauvegarder localement la capture.
6. Analyser avec les filtres documentés.
7. Anonymiser et vérifier avant toute publication.

## Tests réalisés

| Scénario | But | État |
|---|---|---|
| ARP | observer résolution MAC et cache | TODO |
| DNS | suivre requête, réponse et code retour | TODO |
| TCP | analyser handshake, ACK et fermeture | TODO |
| ICMP | mesurer réponse et erreur de test | TODO |
| HTTP/HTTPS | comparer contenu clair et métadonnées TLS | TODO |
| dépannage | isoler DNS, routage ou port indisponible | TODO |

## Sécurité mise en œuvre

- capture limitée au réseau autorisé ;
- aucun contournement de chiffrement ;
- PCAP exclus par défaut du dépôt ;
- contrôle des chaînes, cookies, noms et adresses avant publication ;
- scénarios orientés compréhension et dépannage, pas interception de tiers.

## Résultats

`TODO: à compléter après exécution des scénarios. Aucun résultat n'est inventé.`

## Compétences développées

Analyse de trames, filtres Wireshark, compréhension TCP/IP, résolution DNS, diagnostic méthodique, traitement responsable des données réseau et rédaction technique.

## Captures d'écran

`TODO: ajouter des captures réelles et anonymisées dans captures/ après réalisation du lab.`

## Difficultés rencontrées

`TODO: documenter les difficultés réelles : mauvais choix d'interface, bruit, DNS en cache, chiffrement ou absence de paquets.`

## Axes d'amélioration

- reproduire les scénarios sur IPv6 ;
- comparer capture côté client et côté serveur ;
- analyser retransmissions et latence dans un environnement contrôlé ;
- produire une grille de diagnostic réutilisable.


