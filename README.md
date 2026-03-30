# pns-urp

Dieses Verzeichnis repraesentiert das separate Environment-Repo.

- Die Root-Application bootstrapped die Cluster-spezifischen Child-Applications.
- Die Child-Applications zeigen auf das Paket-Repo `user-resources-pipeline/`.
- Promotion passiert durch Aenderung von `spec.source.targetRevision`.
- Die Clusterstruktur spiegelt die Overlay-Struktur des Paket-Repos, also `onprem/<stage>/<cluster>`.

Beispiel:

- `nop` zeigt auf `v1.2.3`
- `prd` kann spaeter auf denselben Tag `v1.2.3` gesetzt werden
- dafuer ist kein neuer Git-Tag im Paket-Repo noetig
# pns-urp
