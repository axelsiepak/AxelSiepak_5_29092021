
# P5-Kanap - Construisez un site e-commerce en JavaScript

<p align="center">
  <img src="https://user.oc-static.com/upload/2021/09/29/16329291678171_image2.png">
</p>

## Backend
Le dossier back permet de faire tourner l'api contenant les donn�es des produits.
### Installation
Il suffit de se positionner dans le dossier backend avec un terminal et de saisir la commande ```npm install```
### Lancement du serveur
Il suffit de se positionner dans le dossier backend avec un terminal et de saisir la commande ```node start```
Par d�faut le serveur sera lanc� sur le port 3000 ( http://localhost:3000 )
### Route api
Il y a 3 routes disponibles sur le serveur : 

#### GET /api/products/
Permet de r�cup�rer l'ensemble des produits disponibles
#### GET /api/products/{id}
{id} : identifiant unique d'un produit
Permet de r�cup�rer un produit par son identifiant
#### POST /api/products/order
Envoie une commande pour l'enregistrer
La commande envoy� doit �tre au format JSON suivant : 

    {
	    contact{
		    firstName: <string>,
		    lastName: <string>,
		    address: <string>,
		    city; <string>,
		    email: <string>
		},
		products: [<string>]
	}
	
products �tant un tableau d'id produit.

## Frontend
Le frontend pr�sente la partie utilisateur de l'application. Il doit �tre lanc� avec un serveur local (live server avec vscode par exemple), et n�cessite que le backend soit lanc� lui aussi pour fonctionner correctement.

### Config
Le fichier de config permet de d�finir l'adresse de base du server, avec son host, port et si un certificat ssl est utilis� ou non.