# XNOVA
### Ecosistema di Mining Deflazionistico DePIN su BNB Chain, Base & Polygon

**Whitepaper v1.0 — Luglio 2026**

---

## Disclaimer

Questo documento ha scopo puramente informativo e non costituisce consulenza finanziaria, di investimento o legale. XNOVA è un token di utilità guidato dalla community. Le criptovalute sono volatili e comportano rischi. Effettua sempre le tue ricerche (DYOR) prima di acquistare token, attivare Boost o coniare NFT.

---

## Indice

1. Sintesi
2. Introduzione
3. Il Problema
4. La Soluzione XNOVA
5. Come Funziona il Mining
6. Tokenomics
7. Il Meccanismo di Burn
8. Ecosistema
9. Architettura Tecnica
10. Sicurezza e Fiducia
11. Roadmap
12. Indirizzi dei Contratti e Verifica
13. Divulgazione dei Rischi
14. Conclusione

---

## 1. Sintesi

XNOVA è un ecosistema di mining deflazionistico ispirato al modello DePIN (Decentralized Physical Infrastructure Network), costruito su BNB Chain, con un'espansione in corso verso Base e Polygon. A differenza dei tradizionali modelli di yield farming o staking, che si basano sull'emissione di nuovi token per pagare le ricompense, il meccanismo di mining di XNOVA è finanziato interamente dall'acquisto di "Boost" e NFT da parte degli utenti. Ogni unità di BNB spesa per attivare un Boost o coniare un NFT viene convertita direttamente in liquidità permanente e irrecuperabile su PancakeSwap, con i relativi token LP bruciati immediatamente. Questo crea una base di liquidità in continua crescita, mai prelevabile — né dal team né da chiunque altro — abbinata a un supply fisso e non ulteriormente coniabile, di cui il 50% è stato bruciato al lancio.

XNOVA non è solo un token; è la base di un ecosistema più ampio che include un aggregatore DEX multi-chain (xNovaSwap), una piattaforma di lancio fair-launch per meme token (NOVAFUN), un marketplace NFT (Kovyn), un wallet come estensione browser (XNEO Wallet), una piattaforma di chat comunitaria Web3 (XNova Chat), una console AI riservata ai possessori del token (XNOVA AI), e una blockchain EVM proprietaria con il suo explorer e faucet (XNova Chain).

## 2. Introduzione

Il settore del mining e del "GameFi" nel Web3 è stato saturato da progetti che promettono rendimenti elevati finanziati da emissioni di token insostenibili, in cui i primi partecipanti guadagnano a spese di chi arriva dopo. La maggior parte di questi progetti condivide tre punti di debolezza:

- **Emissioni di ricompense inflazionistiche** che diluiscono il valore per i possessori nel tempo
- **Liquidità sbloccata o bloccata solo temporaneamente**, prelevabile dal team in futuro
- **Tokenomics opache**, non verificabili on-chain

XNOVA è stato progettato specificamente per eliminare fin dal primo giorno tutti e tre questi punti di debolezza.

## 3. Il Problema

La maggior parte delle piattaforme di "mining" o "Boost" nel Web3 oggi opera secondo uno di due modelli difettosi:

1. **Modelli di emissione in stile Ponzi** — i depositi dei nuovi utenti vengono usati per pagare i rendimenti degli utenti precedenti, senza creazione di valore reale, finché il modello non collassa.
2. **Liquidità bloccata (non bruciata)** — i team bloccano i token LP per una durata fissa (es. 100 giorni, 1 anno, persino 100 anni), ma un blocco non è permanente. I blocchi possono scadere, essere estesi in modo fraudolento, o essere aggirati se il contratto di blocco stesso viene compromesso o è un proxy controllato dal team.

Entrambi i modelli dipendono dalla fiducia nel team o in un servizio di lock esterno. XNOVA elimina completamente questa dipendenza.

## 4. La Soluzione XNOVA

XNOVA sostituisce la liquidità "bloccata" con liquidità "bruciata" — una garanzia fondamentalmente più forte.

| Modello | La liquidità può mai essere prelevata? |
|---|---|
| Liquidità sbloccata | Sì, in qualsiasi momento |
| Liquidità bloccata a tempo (es. 100 anni) | Sì, una volta scaduto il blocco, o se il contratto di lock viene compromesso |
| **Token LP bruciati (modello XNOVA)** | **No — mai, in nessuna circostanza** |

Quando i token LP vengono inviati a un indirizzo di burn (un wallet senza chiave privata nota, es. `0x000...dEaD` o un indirizzo nullo equivalente), diventano permanentemente e matematicamente irrecuperabili. Non si tratta di una policy o di una promessa — è una garanzia crittografica imposta dalla stessa blockchain che protegge il token.

Ogni volta che un utente acquista un Boost di mining o conia un NFT Supporter NFT, il 100% del BNB ricevuto viene convertito in liquidità XNOVA/BNB su PancakeSwap V2, e i token LP risultanti vengono bruciati. Questo significa:

- La profondità del pool di liquidità cresce soltanto — non si riduce mai.
- Non esiste alcuno scenario, malevolo o meno, in cui quella liquidità possa essere rimossa.
- Ogni singolo acquisto sulla piattaforma rafforza direttamente e permanentemente il floor di prezzo del token.

## 5. Come Funziona il Mining

```
1. Acquista un Boost con BNB
   Gli utenti attivano il mining acquistando pacchetti Boost in BNB.

2. Mina Token XNOVA
   I Boost generano ricompense in XNOVA nel tempo, in base
   all'investimento effettuato.

3. BNB → Liquidità
   Il 100% del BNB da ogni acquisto di Boost viene convertito
   in liquidità XNOVA/BNB su PancakeSwap V2.

4. Token LP Bruciati
   I token LP generati da quella liquidità vengono bruciati
   immediatamente e in modo permanente — non bloccati, non vestiti.
   Spariti per sempre.

5. Supply Deflazionistico
   Insieme al burn del 50% del supply al lancio, la circolazione
   e la liquidità di XNOVA si muovono in un'unica direzione:
   verso il basso e verso una maggiore sicurezza permanente.
```

Le ricompense di mining vengono distribuite dall'allocazione dedicata "Mining Rewards" (20% del supply totale) tramite lo smart contract ufficiale di mining, nel tempo, in base alla dimensione e alla durata del Boost attivo dell'utente.

## 6. Tokenomics

**Supply Totale:** Fisso — nel contratto non esiste alcuna funzione di minting. Il supply può solo diminuire.

| Allocazione | % del Supply Totale | Scopo |
|---|---|---|
| 🔥 Bruciato al Lancio | 50% | Rimosso permanentemente dal supply al TGE. Verificabile su BscScan. |
| 💧 Liquidità (continua) | 25% | Inizialmente creata e continuamente rafforzata dagli acquisti di Boost/NFT. LP bruciata a ogni aggiunta. |
| ⛏️ Ricompense di Mining | 20% | Distribuita nel tempo ai miner attivi tramite il contratto di mining ufficiale. |
| 👨‍🚀 Team | 5% | Proveniente esclusivamente dalla tassa di vendita del 5% — non da un'allocazione anticipata. Vestito/bloccato per lo sviluppo continuo. |

**Indirizzo del Contratto (BNB Chain):**
`0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69`

**Contratto di Mining:**
`0x06fe516f7631983cbf15626263bbdd97671f7735`

## 7. Il Meccanismo di Burn

Il principio fondamentale di fiducia di XNOVA è il suo burn di liquidità ricorrente, attivato a ogni acquisto:

1. Un utente acquista un Boost o conia un NFT Supporter NFT, pagando in BNB.
2. Il 100% di quel BNB viene abbinato a XNOVA e aggiunto come liquidità al pool XNOVA/BNB su PancakeSwap V2.
3. I token LP generati da quel deposito vengono inviati a un indirizzo di burn.
4. Questa posizione LP non può mai essere prelevata dal team, dagli sviluppatori o da terze parti — è matematicamente inaccessibile.

Questo è diverso da — e più forte di — un blocco di liquidità a tempo. Un blocco è una promessa con una data di scadenza. Un burn non ha scadenza, non ha proprietario, e non ha chiave.

*Nota: la cadenza esatta del burn (per singola transazione o in batch) e se il burn venga eseguito automaticamente dalla logica dello smart contract o tramite una transazione manuale e pubblicamente verificabile, dovrebbero essere comunicate in modo trasparente, con link alle transazioni di burn su BscScan man mano che avvengono, per mantenere piena verificabilità.*

## 8. Ecosistema

XNOVA è lo strato di base di un ecosistema Web3 completo:

| Prodotto | Link | Descrizione |
|---|---|---|
| **XNOVA Core** | core.xnova.network | La piattaforma principale di mining deflazionistico — dove gli utenti acquistano Boost, minano XNOVA e attivano il meccanismo di burn della liquidità descritto in questo documento. |
| **xNovaSwap** | app.xnova.network | Aggregatore DEX multi-chain non-custodial che trova i migliori tassi di swap su BNB Chain, Base e Polygon (PancakeSwap, QuickSwap, Uniswap, SushiSwap, BiSwap e altri), con un click. |
| **NOVAFUN** | fun.xnova.network | Piattaforma di lancio fair-launch per meme token su BNB Chain. I token vengono lanciati tramite una bonding curve senza prevendita; la liquidità passa automaticamente a PancakeSwap una volta raggiunto un tetto di 1 BNB, eliminando per progettazione il rischio di rug-pull. |
| **Kovyn** | kovyn.store | Marketplace NFT multi-chain su BNB Chain e Base. Conia ed elenca qualsiasi collezione ERC-721, scambia con BNB, ETH, NOVA, TOSHI, BUSD o USDC, e integra gli NFT ovunque tramite un widget gratuito. |
| **XNEO Wallet** | xneo.xnova.network | Wallet multi-chain come estensione browser, con funzionalità di swap integrata e aggregazione dei prezzi. |
| **XNova Chat** | chat.xnova.network | Piattaforma di chat in tempo reale basata su Web3 per trader di criptovalute, collezionisti NFT e community blockchain, con accesso vincolato alla connessione del wallet. |
| **XNOVA AI** | ai.xnova.network | Console AI riservata, sbloccata esclusivamente per i possessori del token XNOVA/NOVA su BNB Smart Chain. |
| **XNova Chain** | xrpc.xnova.network (explorer) · faucet.xnova.network (faucet) | Blockchain EVM proprietaria basata su PoA (Chain ID 778 mainnet, 1156 testnet, simbolo nativo NOVA), con explorer proprio, faucet testnet e bridge verso BSC. |

Questo approccio a ecosistema significa che XNOVA non è un singolo asset speculativo, ma il token di utilità e ricompensa che collega una suite di prodotti interoperabili — aumentando i casi d'uso reali oltre la speculazione.

## 9. Architettura Tecnica

- **Standard del Token:** BEP-20 (BNB Chain), con espansione cross-chain tramite infrastruttura bridge verso XNova Chain e altre reti EVM.
- **Contratto di Mining:** Distribuisce le ricompense XNOVA proporzionalmente ai possessori di Boost attivi, in base a dimensione e durata del Boost.
- **Flusso del Contratto di Liquidità:** Pagamento Boost/NFT → abbinamento LP automatico su PancakeSwap V2 → burn dei token LP.
- **Bridge di XNova Chain:** Architettura bridge lock-and-mint tra BNB Chain e XNova Chain, con un servizio relayer e protezione anti-replay.
- **Livello NFT (Supporter NFT NFT):** Generazione SVG completamente on-chain con palette di colori basate su seed, garantendo che i metadati NFT non possano essere persi o alterati off-chain.

## 10. Sicurezza e Fiducia

- **Nessuna funzione di minting** — il supply totale è immutabile e può solo diminuire.
- **Nessun percorso di prelievo della liquidità** — i token LP sono bruciati, non detenuti da alcun wallet o contratto di lock.
- **Verificabilità on-chain** — tutti i burn, le aggiunte di liquidità e le distribuzioni di mining sono verificabili tramite BscScan.
- **Allocazione del team proveniente solo dalla tassa di vendita** — il team non riceve alcuna allocazione anticipata di token, allineando gli incentivi con la crescita a lungo termine dell'ecosistema piuttosto che con l'estrazione anticipata.

*Aggiunta consigliata: un report di audit indipendente dello smart contract dovrebbe essere commissionato e collegato qui prima di qualsiasi grande spinta verso una quotazione su exchange, per rafforzare ulteriormente questa sezione.*

## 11. Roadmap

**Fase 1 — Completata**
- Lancio del token su BNB Chain
- Burn del 50% del supply totale al lancio
- Aggiunta della liquidità iniziale

**Fase 2 — Completata**
- Contratto di mining distribuito e attivo
- Lancio della collezione NFT Supporter NFT
- Avvio dell'espansione multi-chain (Polygon)

**Fase 3 — In Corso**
- Quotazioni su CoinGecko e CoinMarketCap
- Programma di airdrop NFT
- Iniziative di crescita della community

**Fase 4 — In Arrivo**
- Quotazioni su exchange centralizzati (CEX)
- Sistema di governance per le proposte della community
- Ulteriori eventi di burn programmati

## 12. Indirizzi dei Contratti e Verifica

| Elemento | Indirizzo / Link |
|---|---|
| Token XNOVA (BNB Chain) | `0x291FdaF5E4a0D6c27E84A3242E4dD2c0720b9c69` |
| Contratto di Mining | `0x06fe516f7631983cbf15626263bbdd97671f7735` |
| Prova del Burn al Lancio | TX BscScan: `0x52eefca1b21c0c2af0816597070aa885b5c64f397f0bbe09d4b1cf7079b0b42e` |
| Contratto xNovaSwap (BNB Chain) | `0xba10C405172cDA339B6dc898c151CB54Ac3a9fBD` |
| Contratto NFT Kovyn (BNB Chain) | `0x81c03f5c8747fbF775934ed327Af640674FA01bC` |
| Contratto NOVAFUN (BNB Chain) | `0x223733a3F2994FC554Ed90E8f62b653F9EB4E79A` |

Tutte le cifre e i contratti citati in questo documento devono essere verificabili in modo indipendente da qualsiasi possessore tramite BscScan, in qualsiasi momento.

## 13. Divulgazione dei Rischi

- Gli asset crypto e DeFi sono altamente volatili. Il valore del token può diminuire significativamente.
- Gli smart contract, per quanto progettati con attenzione, possono contenere vulnerabilità impreviste; gli utenti dovrebbero investire solo ciò che possono permettersi di perdere.
- Il trattamento normativo di token, ricompense di mining e NFT varia in base alla giurisdizione e può cambiare.
- La crescita passata dell'ecosistema o gli eventi di burn precedenti non garantiscono performance future.

## 14. Conclusione

L'innovazione fondamentale di XNOVA è semplice ma potente: sostituire i blocchi di liquidità basati sulla fiducia con burn di liquidità matematicamente permanenti, finanziati interamente dall'uso organico della piattaforma anziché da emissioni inflazionistiche. Unito a un supply fisso e deflazionistico e a un ecosistema di prodotti in crescita — XNOVA Core, xNovaSwap, NOVAFUN, Kovyn, XNEO Wallet, XNova Chat, XNOVA AI e XNova Chain — XNOVA è costruito per allineare gli incentivi dei possessori a lungo termine con un valore reale e verificabile on-chain.

---

*Questo documento verrà aggiornato man mano che l'ecosistema XNOVA si evolve. Per la versione più recente, visita xnova.network.*
