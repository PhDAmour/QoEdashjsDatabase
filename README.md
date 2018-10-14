Dans cette campagne de test, une base de données subjective a été construite avec la méthode "Note Absolue par Catégorie (ACR)" en utilisant le score d'évaluation MOS (Mean Opinion Score) afin de quantifier la QoE des usagers. 

En effet, les tests ont été effectués en utilisant un réseau local filaire (câblés) et/ou sans fil. Tous les dispositifs (ordinateurs de bureau/ ordinateurs personnels, Samsung S$5$, HTC X One, Samsung $4$ Mini et Samsung S$3$) sont connectés au réseau local (LAN) via une connexion Ethernet ou un point d'accès Wifi (AP). 
 
 

En résumé, notre campagne de test subjectif prend en compte plusieurs aspects suggérés par les recommandations de l'ITU et du rapport du groupe de recherche QUALINET. Nous citons ci-dessous quelques-uns.

01) Affichage}: Une application Javascript dédiée basée sur le lecteur vidéo "Dash.js" \footnote{\label{ulm} http://dashif.org/} a été développée pour l'expérimentation et l'ordre d'apparition des séquences vidéo est aléatoire. En effet, le lecteur vidéo développé propose des vidéos  avec différentes qualités allant de $144p$ au Full HD ($1080p$). À noter que lors des expériences, la règle d'adaptabilité de la vidéo (BOLA) a été désactivée (une seule qualité est affichée lors de chaque test).
   
   En pratique, la page principale de notre application de test contient le lecteur vidéo et deux boutons pour lire la vidéo et fournir les retours des utilisateurs en termes de valeur MOS. Le score MOS et les QoE IFs mesurés (conditions de réseau  et paramètres vidéo et dispositif) sont stockés dans la base de données MySQL à l'aide d'un script PHP. Les conditions du réseau pendant les tests sont émulées en utilisant l'émulateur de réseau (NetEm) \cite{2005hemminger_netem}. 
 
  02) Participants}: Un total de $42$ personnes ont participé aux tests. Ces personnes sont des étudiants et des chercheurs du laboratoire $LiSSi$. Leur âge est compris entre $21$ et $41$ avec peu ou pas d'expérience dans l'évaluation de la vidéo. $20\%$ des participants aux tests ont vu au moins $7$ vidéos pendant une session de test et $23\%$ des participants étaient des femmes.

   03) Questions}: Les questions sont simples comme suggéré par le rapport Qualinet ($02$) pour faciliter la procédure d'expérimentation. Par exemple: Notez la qualité globale de la vidéo .
    
   04) Réplication des séquences vidéo}: Les mêmes séquences vidéo ainsi que les mêmes paramètres sont présentés à plusieurs sujets (utilisateurs). Le nombre de séquences utilisées est de deux et elles ont une durée de $60$ secondes. Elles ont été extraites de la vidéo originale  "Big Buck Bunny" couramment utilisée. Les deux séquences vidéo sont encodées dans les mêmes représentations (débit binaire vidéo) à l'aide du codec H.$264$. La table (\ref{Lqualities}) présente les différentes représentations utilisées.


Qualité | Débit binaire vidéo | Résolution | Images/seconde | Codec|  
\hline
  6(1080p30) |   $4$ Mb/s | $1920$ x $1080$ | $15$/$25$/$30$ & H264

  5(720p30) |   $2$ Mb/s & $1280$ x $720$   | $15$/$25$/$30$ & H264
  
  4(480p30) |   $1$ Mb/s | $640$ x $480$   | $15$/$25$/$30$ & H264 

  3(360p30) |   $500$ Kb/s | $512$ x $360$  | $15$/$25$/$30$ & H264 

 2(240p30) |   $250$ Kb/s  | $320$ x $240$ | $15$/$30$ & H264 
 
 1(144p10) |  $125$ Kb/s   | $256$ x $144$  | $10$ & H264
