Part 1 - Even Driven Distributed Processing With Spring Cloud Stream Functions - KAFKA Broker

Tout dabord on commence par le démarrage de serveur zookeeper en ligne de commande (cmd) :
![image](https://user-images.githubusercontent.com/78086000/172024515-47950cee-c4a2-43ed-b5cb-32d528471384.png)

Une fois zookeeper est démarré on va démarrer le serveur KAFKA en ligne de commande (cmd) :
![image](https://user-images.githubusercontent.com/78086000/172024674-b8eb63ed-2126-47d3-bdf4-cc5219367c5d.png)

Puis on démarre l'outil kafka-console-consumer en ligne de commande (cmd) en spécifiant l'emplacement où il se trouve kafka avec l'option --bootstrap-server localhost:9092 et le nom de topic avec l'option --topic R1 :
![image](https://user-images.githubusercontent.com/78086000/172025081-5709602d-57bd-444e-a3b0-2a531376d855.png)

Pour envoyer des messages vers ce topic on va lancer kafka-console-producer :
![image](https://user-images.githubusercontent.com/78086000/172025268-37de7e47-e5a3-4c7c-9675-0305d22c4deb.png)

Maintenant on envoie des messages par le producer et on teste s'ils vont arrivés au consommateur via le broker kafka :
![image](https://user-images.githubusercontent.com/78086000/172025363-c4403311-649b-47c5-aa68-da3464edeaf0.png)

Après avoir tester le fonctionnement de broker kafka avec kafka-console-consumer et kafka-console-producer on passe à la création d'une application Spring Boot dans la quelle on va essayer de produire des messages dans un topic.

Dans la première partie on a publié des messages vers le topic kafka à travers un RestController :
![image](https://user-images.githubusercontent.com/78086000/172027212-4aa0e4e9-fbdf-4388-afd2-df512ea47ef6.png)



