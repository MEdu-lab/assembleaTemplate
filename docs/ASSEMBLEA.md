# {{titolo}}

## 1. Dati della riunione

L'anno **{{data | date: '%Y'}}**, il giorno **{{data | date: '%d'}}** del mese di **{{data | date: '%B'}}**, alle ore **{{ora_inizio}}**, presso **{{luogo}}**, si è riunito il **{{tipo_riunione}}** dell'associazione **{{associazione}}**.

La riunione è stata regolarmente convocata nei modi previsti dallo statuto.

## 2. Partecipanti

**Risultano presenti:**
{% for persona in presenti %}
- {{persona}}
{% endfor %}

**Risultano assenti:**
{% for persona in assenti %}
- {{persona}}
{% endfor %}

Assume la presidenza il Sig. **{{presidente}}**, che invita il Sig. **{{segretario}}** a svolgere le funzioni di segretario verbalizzante.

Il Presidente, accertata la validità della riunione, dichiara aperta la seduta ponendo in discussione il seguente ordine del giorno:

## 3. Ordine del giorno

{% for punto in ordine_del_giorno %}
{{loop.index}}. {{punto}}
{% endfor %}

## 4. Svolgimento della riunione

### 4.1 {{ordine_del_giorno[0]}}

Il Presidente dà lettura del verbale della seduta precedente del {{data_precedente}}.

Il Consiglio/Dell'Assemblea **approva all'unanimità** il verbale così come redatto.

### 4.2 {{ordine_del_giorno[1]}}

Il Presidente comunica che...

*(inserire qui il riassunto della discussione)*

### 4.3 {{ordine_del_giorno[2]}}

Il Presidente illustra la proposta di...

Dopo ampia discussione, si procede alla votazione:

- **Voti favorevoli:** {{n_favorevoli}}
- **Voti contrari:** {{n_contrari}}
- **Astenuti:** {{n_astenuti}}

**Delibera:** Il {{tipo_riunione}} approva la realizzazione dell'evento dal titolo "[titolo]" che si terrà il giorno [data] presso [luogo], con un budget massimo di [importo] Euro.

### 4.4 {{ordine_del_giorno[3]}}

Nessun altro chiedendo la parola, si passa alle varie ed eventuali.

Viene discussa la proposta di...

## 5. Chiusura

Non essendovi altri argomenti da trattare, il Presidente dichiara chiusa la seduta alle ore **{{ora_fine}}**.

Letto, approvato e sottoscritto.

{{luogo}}, lì {{data}}

_________________________          _________________________
Il Presidente                       Il Segretario
({{presidente}})                    ({{segretario}})

---
*Questo verbale è stato redatto e firmato digitalmente ai sensi di legge.*
