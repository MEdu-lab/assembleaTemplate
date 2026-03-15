# {{titolo}}

## 1. Dati della riunione

L'anno **{{data-anno}}**, il giorno **{{data-giorno}}** del mese di **{{data-mese}}**, 
alle ore **{{ora_inizio}}**, presso **{{luogo}}**, si è riunito il **{{tipo_riunione}}** 
dell'associazione **{{associazione}}**.

## 2. Partecipanti

**Risultano presenti:**
{{#presenti}}
- {{.}}
{{/presenti}}

**Risultano assenti:**
{{#assenti}}
- {{.}}
{{/assenti}}

Assume la presidenza il Sig. **{{presidente}}**, che invita il Sig. **{{segretario}}** 
a svolgere le funzioni di segretario verbalizzante.

## 3. Ordine del giorno

{{#ordine_del_giorno}}
1. {{.}}
{{/ordine_del_giorno}}

## 4. Svolgimento

### 4.1 {{ordine_del_giorno.0}}

Il Presidente dà lettura del verbale della seduta precedente...

### 4.3 Votazione

- **Voti favorevoli:** {{n_favorevoli}}
- **Voti contrari:** {{n_contrari}}
- **Astenuti:** {{n_astenuti}}

## 5. Chiusura

Non essendovi altri argomenti, il Presidente dichiara chiusa la seduta alle ore **{{ora_fine}}**.

{{luogo}}, lì {{data}}

_________________________          _________________________
Il Presidente                       Il Segretario
({{presidente}})                    ({{segretario}})
