# Introduction : 

Gelato Networks émerge comme le moteur décentralisé de l'écosystème web3, permettant aux développeurs de créer des **Augmented Smart Contracts**, **Automated**, **Gasless** et **Off-Chain Aware** sur toutes les principales blockchains compatibles avec l'EVM, notamment Ethereum, Polygon, Fantom, Arbitrum, BNB Chain, Optimism, et bien d'autres.

# Que peut-on faire ?

Gelato s'est solidement établi comme une pierre angulaire au sein de la DeFi, étant intégré dans une multitude de protocoles variés au sein de l'écosystème. Son utilisation prolifique dans des scénarios divers, illustre sa polyvalence et son impact significatif, faisant de Gelato un choix incontournable pour les développeurs qui cherchent à optimiser et automatiser divers aspects de leurs applications financières décentralisées :

- Yield Farming
- Oracle
- Algo-Stables
- Bridge
- Gaming
- DeFi
- DEX
- Prediction Market
- DAO
- Lending
- NFT
- Social Media
- Derivatives (TP/SL)

# Comment ça fonctionne ?

Gelato Network agit comme un intermédiaire entre les développeurs cherchant à automatiser des transactions et les opérateurs d'infrastructure exécutant des bots. Les développeurs soumettent des tâches à automatiser sur la plateforme, tandis que les opérateurs exécutent des bots à la recherche de ces tâches. En retour, les opérateurs reçoivent une petite rémunération. Cette approche crée un écosystème où les développeurs peuvent facilement déployer des contrats intelligents automatisés, tandis que les opérateurs sont incités à fournir des services d'exécution fiables. Cette collaboration favorise la création de protocoles web3 décentralisés et robustes.

# Avantages Clés :

1. Pas besoin d'héberger vos propres serveurs sur AWS ou d'autres fournisseurs de cloud

2. Agrégation RPC avec plusieurs solutions de repli

3. Service de relais de transactions fiable qui permet toujours de miner rapidement les transactions

4. Capture automatique des réorganisations (reorgs)

5. Multi-chaîne ; compatible avec les réseaux les plus populaires compatibles avec l'EVM

6. Aucun point de défaillance unique ; plusieurs exécuteurs opèrent dans le monde entier

7. Pas besoin de gérer votre clé privée dans le cloud

8. Couche intégrée de consensus / coordination pour éviter les conditions de concurrence

9. Options de paiement flexibles ; payez avec un solde prépayé ou laissez les transactions se payer elles-mêmes

10. Coût efficace : moins cher que la construction, l'exploitation et la maintenance de serveurs personnalisés

# Economie :

Le Gelato Network est un protocole durable et générateur de revenus. Le réseau est "avide de transactions" - plus les transactions sont automatisées via les services d'infrastructure des exécuteurs, moins ils ont besoin d'être rémunérés par transaction pour couvrir leurs coûts fixes d'infrastructure. Les exécuteurs justifieront les coûts liés à l'exploitation de leur infrastructure par l'augmentation de la quantité de transactions, et non par l'augmentation de la valeur capturée par les transactions individuelles. Cela rend Gelato plus rentable à utiliser pour les applications décentralisées (dApps) que de gérer leur propre système centralisé de gardiens.
En bref il faut que le protocol soit bien implémenté dans l'écosystème web3.

# Architecture :

Tous les services de Gelato s'appuient sur la même architecture centrale du réseau Gelato, chargée de garantir l'exécution correcte et efficace des tâches. Fondamentalement, le Gelato Network doit constamment vérifier si les conditions d'exécution d'une tâche sont remplies. Lorsqu'elles le sont, il exécute la transaction et veille à ce qu'elle soit confirmée de manière rapide et efficace. Le réseau est scindé en 3 groupes :

1. L'**Event Listener** : chargé de monitorer et de surveiller le réseau à la recherche de **Queries**
2. Le **Checker** : définit une logique arbitraire/personnalisée pour vérifier si une tâche Gelato est exécutable à un moment donné. Il définit les conditions requises pour qu'une tâche devienne exécutable.
3. L'**Executor** : est responsable de soumettre de manière fiable des transactions sur la chaîne et de veiller à ce qu'elles soient confirmées aussi rapidement que possible et avec le coût le plus bas.

# Smart Contract :

Les **Smarts Contracts** de Gelato sont sous la norme **EIP-2535** aussi appelé : **Diamond Proxy**.
Qui a pour but de simplifié le développement de **Smart Contract** : 
1. Une seule passerelle pour effectuer des appels de proxy à X contrats d'implémentation.
2. Mise à niveau atomique d'un ou de plusieurs **Smart Contract**.
3. Aucune limite de stockage pour le nombre de contrats d'implémentation que vous pouvez ajouter à votre Diamond.
4. Historique complet de toutes les mises à niveau effectuées sur le Diamond.
5. Possibilité de réduire les **gas fee**.

# Services :

## Rollup as a Service (RaaS) :

1. **Facilité de déploiement :** Gelato offre une interface utilisateur intuitive pour un déploiement sans code, une surveillance et une gestion simples des Rollups Ethereum.
2. **Modularité et Performance :** Gelato RaaS adopte une architecture modulaire offrant des performances améliorées et une personnalisation avec des options évolutives, sécurisées et rentables.
3. **Intégration native d'outils et services :** Gelato RaaS s'intègre nativement à vos outils et services Web3 préférés pour une expérience intégrée de la couche 2.
4. **Fiabilité élevée et Multi-Cloud :** Gelato RaaS propose une infrastructure multi-cloud mondiale, garantissant une disponibilité élevée et une performance constante.

## 1Balance :

Système unifié de paiements multi-chaînes de Gelato Aperçu Lorsque vous utilisez chacun des services de Gelato, vous devez payer deux types de frais :

1. Les **gas fees** de vos transactions exécutées.
2. Les frais de service - abonnements Gelato ou primes en pourcentage sur les **gas fee** de chaque transaction. 1Balance facilite le paiement de tous vos frais sur l'ensemble des réseaux que vous utilisez, depuis un solde unique et facile à gérer.

## Account Abstraction / Smart wallet :

### Avantage clés :

1. Entièrement programmable.
2. Logique de vérification et de récupération arbitraire.
3. Opération multiples
4. Transactions sans frais

## Relay SDK :

Avec Gelato Relay, nous facilitons l'envoi de transactions pour les utilisateurs, même sans solde de jeton natif. Par exemple, un utilisateur peut payer les **gas fee** en utilisant le jeton qu'il souhaite échanger. Nous passons d'un modèle où l'utilisateur envoie la transaction lui-même à un modèle où l'utilisateur signe un message standardisé transmis à un relayer. Le relayer vérifie la signature de l'utilisateur et transmet le message on-chain.

Gelato Relay assure le relais des transactions de l'utilisateur on-chain, offrant des transactions sans **gas fee** sécurisées pour une expérience utilisateur fluide. Cela ouvre la porte à de nouvelles expériences web3, permettant aux utilisateurs de payer en signant un simple message, ou de laisser les frais de transaction être pris en charge par le développeur. Tant que les frais de gaz sont couverts par l'un des modes de paiement pris en charge par Gelato, le reste est géré de manière fiable, rapide et sécurisée.

## Web3 Functions :

Gelato offre la possibilité de connecter des API en dehors de la blockchain, de les lire et de les exécuter sur la blockchain, le tout automatisé grâce à ses services. Bien que cela reste une fonctionnalité puissante, elle demeure complexe, réservée exclusivement aux développeurs passionnés par l'innovation dans le monde de la blockchain.

## VRF (Verifiable Random Function)

Dans le monde de la cryptographie et des applications décentralisées, le hasard joue un rôle crucial. Bien que le hasard soit un concept fondamental, parvenir à une imprévisibilité authentique de manière transparente et vérifiable sur la blockchain est un défi. C'est là qu'intervient Gelato VRF (Verifiable Random Function) - un outil conçu pour fournir une imprévisibilité robuste avec une vérifiabilité inhérente.



# Gnosis Safe :

Nous vous recommandons d'utiliser notre application personnalisée au sein de ***Gnosis Safe*** pour une connexion plus fiable et une expérience utilisateur plus fluide. Wallet Connect rencontre parfois des problèmes et n'est pas recommandé.

# Token :

Gelato a été conçu dès le départ comme un projet open source et orienté communauté. Le protocole est pensé pour être détenu par ceux qui l'utilisent le plus, plaçant ainsi le pouvoir entre les mains des utilisateurs. Pour concrétiser cette vision, le Gelato DAO a été créé, alimenté par le token Gelato (GEL), servant d'outil d'alignement des incitations au sein du réseau.

1. Gouvernance : Tous les détenteurs de tokens peuvent voter sur les propositions dans le Gelato DAO, permettant une prise de décision collaborative sur le protocole. Les développeurs utilisant Gelato pour automatiser leurs fonctions auront un rôle prépondérant dans la gouvernance.
2. Mise en jeu : Les Executors, chargés de l'exécution des transactions, doivent acquérir et mettre en jeu des $GEL pour participer et gagner des récompenses. La mise en jeu permet de réserver des "slots" pour obtenir l'exclusivité des frais pendant une période donnée.

La réduction potentielle de la mise des Executors vise à décourager les comportements indésirables. Le Gelato DAO surveillera et régulera, renforçant la responsabilité des Executors. Le staking GEL peut être similaire à ETH 2.0, et des services comme Lido pourraient émerger pour les détenteurs passifs.

Le Gelato DAO permet aux parties prenantes de superviser les bots, assurant leur bon fonctionnement. L'offre initiale de Gelato Token est de 420 690 000, avec la possibilité d'émission de tokens supplémentaires après deux ans par vote des détenteurs.

## Token Contract :

| Blockchain  | Contract  |
|---|---|
|Ethereum (ERC20)|0x15b7c0c907e4C6b9AdaAaabC300C08991D6CEA05|
|Fantom|0x15b7c0c907e4C6b9AdaAaabC300C08991D6CEA05|
|Polygon|0x15b7c0c907e4C6b9AdaAaabC300C08991D6CEA05|


# Conclusion :

Gelato Networks émerge comme un projet résolument axé sur la technologie et les développeurs, apportant des innovations techniques significatives dans l'écosystème blockchain. Son positionnement unique en tant que pionnier dans son domaine se traduit par l'absence de concurrents directs, témoignant de la singularité de son offre.

 L'absence de concurrents combinée à des partenariats de plus en plus substantiels souligne la confiance croissante de l'industrie dans le projet. Le token GEL, au cœur du système, se distingue en tant qu'outil véritablement utile, conférant aux détenteurs un rôle actif dans la gouvernance et les décisions clés du réseau.

Gelato Networks s'inscrit ainsi comme une force innovante, propulsant l'écosystème blockchain vers de nouveaux horizons tout en fournissant aux développeurs les outils nécessaires pour façonner l'avenir de la technologie décentralisée.