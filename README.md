Ce projet met en œuvre une solution MPLS (Multiprotocol Label Switching) pour établir un VPN (Virtual Private Network) sécurisé et performant. La solution permet une communication efficace entre plusieurs sites distants, en garantissant la qualité de service (QoS) et en optimisant l'utilisation de la bande passante. Grâce à une architecture robuste, cette solution facilite le transport de différents types de données, tout en offrant une segmentation et une sécurité améliorées. Les configurations incluent des routeurs CE et PE, avec des protocoles de routage adaptés pour assurer une connectivité fluide et fiable
1. Configuration des Interfaces
Dans cette première étape, nous configurons les interfaces des routeurs CE (Customer Edge) et PE (Provider Edge) pour assurer la connectivité de base entre les différents sites. Cela inclut l'attribution d'adresses IP appropriées et la vérification de la connectivité avec des pings.

2. Configuration OSPF
La deuxième partie consiste à mettre en place OSPF (Open Shortest Path First) comme protocole de routage interne. Nous configurons les routeurs pour permettre l'échange d'informations de routage et optimiser la convergence du réseau.

3. Configuration RIP
Nous ajoutons ensuite RIP (Routing Information Protocol) pour soutenir la redondance et offrir une alternative au routage. Cette configuration permet de gérer les chemins de manière dynamique, assurant ainsi une résilience accrue.

4. Configuration MPLS
La quatrième étape implique la mise en œuvre de MPLS pour améliorer l'efficacité du routage. Nous configurons les LSR (Label Switch Routers) pour permettre le transfert de paquets basé sur des labels, optimisant ainsi le trafic réseau.

5. VRF et BGP
Nous mettons en place des VRF (Virtual Routing and Forwarding) pour segmenter le trafic et assurer l'isolation entre différents clients ou services. BGP (Border Gateway Protocol) est également configuré pour gérer l'échange de routes entre différents systèmes autonomes.

6. Redistribution de Routes
Enfin, nous configurons la redistribution des routes entre OSPF, RIP, et BGP afin d'assurer une intégration fluide des différentes topologies de routage et d'optimiser la connectivité dans l'ensemble du réseau.
