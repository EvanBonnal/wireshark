# 🚀 Lab d'Administration Système & Analyse Réseau
> **Titre :** Nas_Debian   
> **Auteur :** Evan Bonnal, Natalia Giraldo, Ludovic Dos Santos    
> **Formation :**  Bachelor IT en Cyber     
> **Période :** 11 mai 2026 – 18 mai 2026 (1 semaine)  
> **Établissement :** La plateforme_


---

Ce dépôt documente la mise en place d'une infrastructure de déploiement réseau sécurisée (PXE) et l'analyse approfondie du trafic réseau à l'aide d'outils de capture de paquets. Ce projet a été réalisé dans un environnement de laboratoire virtualisé.

## 🔍 Analyse de Trafic & Sécurité des Protocoles (Wireshark / Tshark)

Cette partie est dédiée à l'audit réseau, en comparant la sécurité des protocoles en clair avec leurs équivalents chiffrés, et en démontrant la maîtrise du filtrage en ligne de commande.

### Fonctionnalités implémentées
* **Audit de sécurité FTP (Cleartext) :** Capture de trafic FTP classique démontrant la vulnérabilité du protocole (interception de requêtes `USER` / `PASS` et de données sensibles en clair).
* **Validation du chiffrement (SSL/TLS) :** Comparaison avec un flux sécurisé démontrant l'opacité des paquets (Application Data chiffrée) et la protection contre l'écoute flottante (Sniffing).
* **Filtrage avancé avec `tshark` :** Maîtrise des différentes approches d'écoute réseau sous Linux :
    * **Filtres de capture (`-f`) :** Filtrage matériel BPF directement sur les ports (ex: `udp port 53` pour optimiser les performances).
    * **Filtres d'affichage (`-Y`) :** Analyse protocolaire par le moteur de tshark (ex: `tls.handshake.version == 0x0304` pour cibler TLS 1.3).
    * **Redirection (`| grep`) :** Traitement du flux en temps réel avec les outils natifs Linux.
* **Protocoles isolés et analysés :** DHCP, DNS, mDNS, FTP, SMB, HTTP, TLSv1.2, TLSv1.3.

---

## 🤝 Équipe

<table>
  <thead>
    <tr>
      <th>Avatar</th>
      <th>Membre</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">
         <img src="https://github.com/evanbonnal.png?size=32" alt="Evan Bonnal" style="width:40px; height:40px; border-radius:4px;" />
      </td>
      <td><strong><a href="https://github.com/evanbonnal">Evan Bonnal</a></strong></td>
    </tr>
    <tr>
      <td align="center">
        <img src="https://github.com/Natalia-Giraldo.png?size=32" alt="Natalia Giraldo" style="width:40px; height:40px; border-radius:4px;" />
      </td>
      <td><strong><a href="https://github.com/Natalia-Giraldo">Natalia Giraldo</a></strong></td>
    </tr>
    <tr>
      <td align="center">
        <img src="https://github.com/ludovicdos-santos-io.png?size=32" alt="Alexandre Berdejo" style="width:40px; height:40px; border-radius:4px;" />
      </td>
      <td><strong><a href="https://github.com/ludovicdos-santos-io">Ludovic Dos Santos</a></strong></td>
    </tr>
    <tr>
  </tbody>
</table>

---


## 🎓 Contexte
Projet réalisé dans le cadre de la formation d'Administration Système / Cybersécurité à **La Plateforme**.
