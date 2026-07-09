# XNOVA
### Écosystème de Minage Déflationniste DePIN sur BNB Chain, Base & Polygon

**Whitepaper v1.0 — Juillet 2026**

---

## Avertissement

Ce document est fourni à titre purement informatif et ne constitue pas un conseil financier, d'investissement ou juridique. XNOVA est un token utilitaire porté par sa communauté. Les actifs cryptographiques sont volatils et comportent des risques. Effectuez toujours vos propres recherches (DYOR) avant tout achat de token, activation de Boost, ou mint de NFT.

---

## Table des matières

1. Résumé
2. Introduction
3. Le Problème
4. La Solution XNOVA
5. Fonctionnement du Minage
6. Tokenomics
7. Le Mécanisme de Burn
8. Écosystème
9. Architecture Technique
10. Sécurité et Confiance
11. Feuille de Route
12. Adresses des Contrats et Vérification
13. Divulgation des Risques
14. Conclusion

---

## 1. Résumé

XNOVA est un écosystème de minage déflationniste inspiré du modèle DePIN (Decentralized Physical Infrastructure Network), construit sur BNB Chain, avec une expansion en cours vers Base et Polygon. Contrairement aux modèles traditionnels de yield farming ou de staking qui reposent sur l'émission de nouveaux tokens pour verser des récompenses, le mécanisme de minage de XNOVA est entièrement financé par l'achat de « Boosts » et de NFT par les utilisateurs. Chaque unité de BNB dépensée pour activer un Boost ou minter un NFT est directement convertie en liquidité permanente et irrécupérable sur PancakeSwap, les tokens LP résultants étant immédiatement brûlés. Cela crée un plancher de liquidité en croissance constante, qui ne peut jamais être retiré — ni par l'équipe, ni par qui que ce soit — associé à une offre de tokens plafonnée et non re-mintable, dont 50 % a été brûlé au lancement.

XNOVA n'est pas qu'un simple token ; il constitue la base d'un écosystème plus large comprenant un agrégateur DEX multi-chaînes (xNovaSwap), une plateforme de lancement équitable de meme tokens (NOVAFUN), une place de marché NFT (Kovyn), un portefeuille sous forme d'extension navigateur (XNEO Wallet), une plateforme de chat communautaire Web3 (XNova Chat), une console IA réservée aux détenteurs du token (XNOVA AI), et une blockchain EVM propriétaire disposant de son propre explorateur et de son propre faucet (XNova Chain).

## 2. Introduction

L'espace du minage et du « GameFi » dans le Web3 a été saturé de projets promettant des rendements élevés financés par des émissions de tokens non viables, où les premiers participants profitent au détriment des suivants. La plupart de ces projets partagent trois points de défaillance :

- **Des émissions de récompenses inflationnistes** qui diluent la valeur des détenteurs au fil du temps
- **Une liquidité non verrouillée ou verrouillée temporairement**, pouvant à terme être retirée par l'équipe
- **Une tokenomics opaque**, non vérifiable on-chain

XNOVA a été conçu spécifiquement pour éliminer ces trois points de défaillance dès le premier jour.

## 3. Le Problème

La plupart des plateformes de « minage » ou de « Boost » dans le Web3 fonctionnent aujourd'hui selon l'un de ces deux modèles défaillants :

1. **Modèles d'émission de type Ponzi** — les dépôts des nouveaux utilisateurs servent à payer les rendements des utilisateurs précédents, sans création de valeur réelle, jusqu'à l'effondrement du modèle.
2. **Liquidité verrouillée (et non brûlée)** — les équipes verrouillent les tokens LP pour une durée fixe (par exemple 100 jours, 1 an, voire 100 ans), mais un verrouillage n'est pas permanent. Les verrouillages peuvent expirer, être prolongés frauduleusement, ou contournés si le contrat de verrouillage lui-même est compromis ou constitue un proxy contrôlé par l'équipe.

Ces deux modèles reposent sur la confiance accordée à une équipe ou à un service de verrouillage tiers. XNOVA supprime entièrement cette dépendance.

## 4. La Solution XNOVA

XNOVA remplace la liquidité « verrouillée » par une liquidité « brûlée » — une garantie fondamentalement plus solide.

| Modèle | La liquidité peut-elle un jour être retirée ? |
|---|---|
| Liquidité non verrouillée | Oui, à tout moment |
| Liquidité verrouillée pour une durée (ex. 100 ans) | Oui, une fois le verrouillage expiré, ou si le contrat de verrouillage est compromis |
| **Tokens LP brûlés (modèle XNOVA)** | **Non — jamais, en aucune circonstance** |

Lorsque des tokens LP sont envoyés vers une adresse de burn (un portefeuille sans clé privée connue, par exemple `0x000...dEaD` ou une adresse nulle équivalente), ils deviennent définitivement et mathématiquement irrécupérables. Il ne s'agit pas d'une politique ou d'une promesse — c'est une garantie cryptographique appliquée par la blockchain elle-même, celle-là même qui sécurise le token.

À chaque achat d'un Boost de minage ou mint d'un NFT Supporter NFT par un utilisateur, 100 % du BNB reçu est converti en liquidité XNOVA/BNB sur PancakeSwap V2, et les tokens LP résultants sont brûlés. Cela signifie que :

- La profondeur du pool de liquidité ne fait que croître — elle ne diminue jamais.
- Il n'existe aucun scénario, malveillant ou non, dans lequel cette liquidité pourrait être retirée.
- Chaque achat effectué sur la plateforme renforce directement et durablement le plancher de prix du token.

## 5. Fonctionnement du Minage

```
1. Achetez un Boost avec du BNB
   Les utilisateurs activent le minage en achetant des
   packages Boost en BNB.

2. Minez des tokens XNOVA
   Les Boosts génèrent des récompenses en XNOVA au fil du temps,
   proportionnellement à votre investissement.

3. BNB → Liquidité
   100 % du BNB de chaque achat de Boost est converti en
   liquidité XNOVA/BNB sur PancakeSwap V2.

4. Tokens LP Brûlés
   Les tokens LP générés par cette liquidité sont immédiatement
   et définitivement brûlés — ni verrouillés, ni soumis à vesting.
   Disparus pour toujours.

5. Offre Déflationniste
   Combinée au burn de 50 % de l'offre au lancement, l'offre
   en circulation et la liquidité de XNOVA n'évoluent que dans
   un seul sens : à la baisse, et vers une sécurité toujours plus
   permanente.
```

Les récompenses de minage sont distribuées à partir de l'allocation dédiée « Mining Rewards » (20 % de l'offre totale), via le smart contract officiel de minage, au fil du temps, en fonction de la taille et de la durée du Boost actif de l'utilisateur.

## 6. Tokenomics

**Offre Totale :** Fixe — aucune fonction de mint n'existe dans le contrat. L'offre ne peut que diminuer.

| Allocation | % de l'Offre Totale | Objectif |
|---|---|---|
| 🔥 Brûlé au Lancement | 50 % | Retiré définitivement de l'offre lors du TGE. Vérifiable sur BscScan. |
| 💧 Liquidité (continue) | 25 % | Amorcée initialement puis continuellement renforcée par les achats de Boost/NFT. LP brûlée à chaque ajout. |
| ⛏️ Récompenses de Minage | 20 % | Distribuée au fil du temps aux mineurs actifs via le contrat de minage officiel. |
| 👨‍🚀 Équipe | 5 % | Provenant exclusivement de la taxe de vente de 5 % — et non d'une allocation initiale. Soumise à vesting/verrouillage pour financer le développement continu. |

**Adresse du Contrat (BNB Chain) :**
`0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69`

**Contrat de Minage :**
`0x06fe516f7631983cbf15626263bbdd97671f7735`

## 7. Le Mécanisme de Burn

Le principe fondamental de confiance de XNOVA repose sur son burn de liquidité récurrent, déclenché à chaque achat :

1. Un utilisateur achète un Boost ou mint un NFT Supporter NFT, en payant en BNB.
2. 100 % de ce BNB est apparié à du XNOVA et ajouté comme liquidité au pool XNOVA/BNB sur PancakeSwap V2.
3. Les tokens LP générés par ce dépôt sont envoyés vers une adresse de burn.
4. Cette position LP ne peut jamais être retirée — ni par l'équipe, ni par les développeurs, ni par un tiers quelconque — elle est mathématiquement inaccessible.

Ceci est distinct de — et plus robuste qu'— un verrouillage de liquidité limité dans le temps. Un verrouillage est une promesse assortie d'une date d'expiration. Un burn n'a ni expiration, ni propriétaire, ni clé.

*Remarque : la cadence exacte du burn (par transaction ou par lots) et le fait que celui-ci soit exécuté automatiquement par la logique du smart contract ou via une transaction manuelle publiquement vérifiable devraient être communiqués de manière transparente, avec des liens vers les transactions de burn sur BscScan au fur et à mesure qu'elles se produisent, afin de garantir une vérifiabilité complète.*

## 8. Écosystème

XNOVA constitue la couche de base d'un écosystème Web3 complet :

| Produit | Lien | Description |
|---|---|---|
| **XNOVA Core** | core.xnova.network | La plateforme principale de minage déflationniste — où les utilisateurs achètent des Boosts, minent du XNOVA, et déclenchent le mécanisme de burn de liquidité décrit dans ce document. |
| **xNovaSwap** | app.xnova.network | Agrégateur DEX multi-chaînes non custodial trouvant les meilleurs taux d'échange sur BNB Chain, Base et Polygon (PancakeSwap, QuickSwap, Uniswap, SushiSwap, BiSwap, et autres), en un clic. |
| **NOVAFUN** | fun.xnova.network | Plateforme de lancement équitable de meme tokens sur BNB Chain. Les tokens sont lancés via une bonding curve, sans prévente ; la liquidité bascule automatiquement vers PancakeSwap une fois un plafond de 1 BNB atteint, éliminant le risque de rug-pull par conception. |
| **Kovyn** | kovyn.store | Place de marché NFT multi-chaînes sur BNB Chain et Base. Mintez et listez n'importe quelle collection ERC-721, échangez en BNB, ETH, NOVA, TOSHI, BUSD ou USDC, et intégrez vos NFT n'importe où via un widget gratuit. |
| **XNEO Wallet** | xneo.xnova.network | Portefeuille sous forme d'extension navigateur, multi-chaînes, avec fonctionnalité de swap intégrée et agrégation des prix. |
| **XNova Chat** | chat.xnova.network | Plateforme de chat en temps réel propulsée par le Web3, destinée aux traders de cryptomonnaies, collectionneurs de NFT et communautés blockchain, avec accès conditionné à la connexion d'un portefeuille. |
| **XNOVA AI** | ai.xnova.network | Console IA à accès restreint, débloquée exclusivement pour les détenteurs du token XNOVA/NOVA sur BNB Smart Chain. |
| **XNova Chain** | xrpc.xnova.network (explorateur) · faucet.xnova.network (faucet) | Blockchain EVM propriétaire fonctionnant en PoA (Chain ID 778 pour le mainnet, 1156 pour le testnet, symbole natif NOVA), avec son propre explorateur de blocs, un faucet testnet, et un pont vers BSC. |

Cette approche écosystémique signifie que XNOVA n'est pas un actif spéculatif isolé, mais bien le token utilitaire et de récompense qui relie une suite de produits interopérables — augmentant ainsi les cas d'usage réels au-delà de la spéculation.

## 9. Architecture Technique

- **Standard du Token :** BEP-20 (BNB Chain), avec une expansion cross-chain via une infrastructure de pont vers XNova Chain et d'autres réseaux EVM.
- **Contrat de Minage :** Distribue les récompenses XNOVA proportionnellement aux détenteurs de Boost actifs, en fonction de la taille et de la durée du Boost.
- **Flux du Contrat de Liquidité :** Paiement Boost/NFT → appariement LP automatique sur PancakeSwap V2 → burn des tokens LP.
- **Pont XNova Chain :** Architecture de pont de type lock-and-mint entre BNB Chain et XNova Chain, avec un service de relayer et une protection anti-replay.
- **Couche NFT (NFT Supporter NFT) :** Génération SVG entièrement on-chain avec des palettes de couleurs basées sur un seed, garantissant que les métadonnées NFT ne peuvent être ni perdues ni altérées hors chaîne.

## 10. Sécurité et Confiance

- **Aucune fonction de mint** — l'offre totale est immuable et ne peut que diminuer.
- **Aucun chemin de retrait de la liquidité** — les tokens LP sont brûlés, non détenus par un portefeuille ou un contrat de verrouillage.
- **Vérifiabilité on-chain** — tous les burns, ajouts de liquidité et distributions de minage sont vérifiables via BscScan.
- **Allocation de l'équipe provenant uniquement de la taxe de vente** — l'équipe ne reçoit aucune allocation de tokens en amont, alignant ainsi les incitations sur la croissance à long terme de l'écosystème plutôt que sur une extraction précoce.

*Ajout recommandé : un rapport d'audit indépendant du smart contract devrait être commandé et lié ici avant toute démarche majeure de cotation sur un exchange, afin de renforcer davantage cette section.*

## 11. Feuille de Route

**Phase 1 — Terminée**
- Lancement du token sur BNB Chain
- Burn de 50 % de l'offre totale au lancement
- Ajout de la liquidité initiale

**Phase 2 — Terminée**
- Contrat de minage déployé et actif
- Lancement de la collection NFT Supporter NFT
- Lancement de l'expansion multi-chaînes (Polygon)

**Phase 3 — En cours**
- Cotations sur CoinGecko et CoinMarketCap
- Programme d'airdrop NFT
- Initiatives de croissance communautaire

**Phase 4 — À venir**
- Cotations sur des exchanges centralisés (CEX)
- Système de gouvernance pour les propositions communautaires
- Événements de burn supplémentaires programmés

## 12. Adresses des Contrats et Vérification

| Élément | Adresse / Lien |
|---|---|
| Token XNOVA (BNB Chain) | `0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69` |
| Contrat de Minage | `0x06fe516f7631983cbf15626263bbdd97671f7735` |
| Preuve du Burn au Lancement | TX BscScan : `0x52eefca1b21c0c2af0816597070aa885b5c64f397f0bbe09d4b1cf7079b0b42e` |
| Contrat xNovaSwap (BNB Chain) | `0xba10C405172cDA339B6dc898c151CB54Ac3a9fBD` |
| Contrat NFT Kovyn (BNB Chain) | `0x81c03f5c8747fbF775934ed327Af640674FA01bC` |
| Contrat NOVAFUN (BNB Chain) | `0x223733a3F2994FC554Ed90E8f62b653F9EB4E79A` |

Tous les chiffres et contrats mentionnés dans ce document doivent pouvoir être vérifiés de manière indépendante par tout détenteur, à tout moment, via BscScan.

## 13. Divulgation des Risques

- Les actifs cryptographiques et DeFi sont hautement volatils. La valeur du token peut diminuer de manière significative.
- Les smart contracts, bien que conçus avec soin, peuvent contenir des vulnérabilités imprévues ; les utilisateurs ne devraient engager que des fonds dont ils peuvent supporter la perte.
- Le traitement réglementaire des tokens, des récompenses de minage et des NFT varie selon les juridictions et peut évoluer.
- La croissance passée de l'écosystème ou les événements de burn antérieurs ne garantissent pas les performances futures.

## 14. Conclusion

L'innovation centrale de XNOVA est simple mais puissante : remplacer les verrouillages de liquidité fondés sur la confiance par des burns de liquidité mathématiquement permanents, financés entièrement par l'usage organique de la plateforme plutôt que par des émissions inflationnistes. Associé à une offre fixe et déflationniste ainsi qu'à un écosystème de produits en pleine croissance — XNOVA Core, xNovaSwap, NOVAFUN, Kovyn, XNEO Wallet, XNova Chat, XNOVA AI et XNova Chain — XNOVA est conçu pour aligner les incitations des détenteurs à long terme avec une valeur réelle et vérifiable on-chain.

---

*Ce document sera mis à jour à mesure que l'écosystème XNOVA évolue. Pour la dernière version, rendez-vous sur xnova.network.*
