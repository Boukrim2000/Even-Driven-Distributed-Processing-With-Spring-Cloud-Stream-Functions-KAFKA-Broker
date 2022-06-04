Part 1 - Even Driven Distributed Processing With Spring Cloud Stream Functions - KAFKA Broker

Tout dabord on commence par le démarrage de serveur zookeeper en ligne de commande (cmd) :
![image](https://user-images.githubusercontent.com/78086000/172024515-47950cee-c4a2-43ed-b5cb-32d528471384.png)

Une fois zookeeper est démarré on va démarrer le serveur KAFKA en ligne de commande (cmd) :
![image](https://user-images.githubusercontent.com/78086000/172024674-b8eb63ed-2126-47d3-bdf4-cc5219367c5d.png)

Puis on démarre l'outil kafka-console-consumer en ligne de commande (cmd) en spécifiant l'emplacement où il se trouve kafka avec l'option --bootstrap-server localhost:9092 et le nom de topic avec l'option --topic R1 :
![image](https://user-images.githubusercontent.com/78086000/172025081-5709602d-57bd-444e-a3b0-2a531376d855.png)
