# JAX-RS-Jersey


Vidéo de Démonstration
Pour une démonstration complète, veuillez consulter la vidéo suivante :[Uploading 4e68e117-8d3b-4d6d-a511-b2bce417a302.webm…]()


1. Récupérer tous les comptes
curl -X GET "http://localhost:8082/banque/comptes" -H "Accept: application/xml"
2. Récupérer un compte par ID
curl -X GET "http://localhost:8082/banque/comptes/1" -H "Accept: application/xml"

4. Ajouter un compte
curl -X POST "http://localhost:8082/banque/comptes" -H "Content-Type: application/xml" -d '<?xml version="1.0" encoding="UTF-8"?>
<compte>
    <solde>1000.0</solde>
    <dateCreation>2024-01-01</dateCreation>
    <type>EPARGNE</type>
</compte>'

6. Mettre à jour un compte existant
curl -X PUT "http://localhost:8082/banque/comptes/1" -H "Content-Type: application/xml" -d '<?xml version="1.0" encoding="UTF-8"?>
<compte>
    <solde>1500.0</solde>
    <dateCreation>2024-01-01</dateCreation>
    <type>EPARGNE</type>
</compte>'
7. Supprimer un compte
curl -X DELETE "http://localhost:8082/banque/comptes/2"


