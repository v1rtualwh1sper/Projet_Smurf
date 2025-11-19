Ce projet utilise Python et Scapy pour simuler diverses attaques réseau par rebond, démontrant des techniques d'usurpation et d'amplification.

## Techniques Mises en Œuvre

Les scripts explorent plusieurs méthodes d'attaques par rebond en forgeant des paquets à différentes couches réseau :
*   **Couche 2 & 3 :** Usurpation d'adresses MAC et IP pour rediriger des réponses ICMP vers une victime (IP Spoofing).
*   **Amplification :** Utilisation d'adresses de broadcast (MAC et IP) pour tenter de générer des réponses multiples.
*   **Couche 4 :** Exploitation du service UDP "echo" en combinaison avec l'usurpation d'IP pour rediriger le trafic.

Le projet inclut également des sniffers ICMP et UDP pour analyser le trafic généré.

## Utilisation

**Prérequis :** `python3`, `scapy`, `sudo`

1.  Configurez les adresses IP/MAC dans les scripts (`src/`).
2.  Exécutez un script d'attaque : `sudo python src/nom_du_script.py`
3.  Utilisez `server.py` ou `udp_sniffer.py` pour observer les résultats.

*Ces outils sont destinés à un usage éducatif dans un environnement contrôlé.*