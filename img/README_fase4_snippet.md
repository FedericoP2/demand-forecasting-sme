
## 📊 Risultati della Simulazione di Business (Fase 4)

> **Metodologia economica**: ricavo = `checkout_price` (prezzo reale del dataset),
> costo = `base_price × 40%` (food cost standard ristorazione).
> Parametri dichiarati come ipotesi di simulazione, non dati aziendali reali.

Applicando il modello al test set (4 settimane, 13,113 osservazioni centro-piatto),
la simulazione in **Shadow Mode** confronta tre scenari:

| Scenario | Profitto Simulato | vs Baseline |
|---|---|---|
| 🔵 Oracolo (domanda perfetta) | € 498,601,847 | +88.5% |
| 🟢 **LightGBM (nostro modello)** | **€ 310,991,531** | **+17.5%** |
| 🔴 Baseline (settimana scorsa) | € 264,566,274 | — |

**Il modello AI ha generato € 46,425,258 di profitto aggiuntivo** rispetto al metodo tradizionale,
riducendo i pasti sprecati di **148,096 unità** e gli stockout di **78,500 unità**.

Rimane un gap del **37.6%** rispetto all'oracolo teorico — margine di miglioramento
raggiungibile con feature più ricche (es. dati LLM sulle ricette, festività locali).

![Business Impact](img/business_impact.png)
