# MiniProjet Flask

Ce projet est une application web basique développée avec le framework **Flask**. Elle inclut plusieurs pages interactives permettant de naviguer facilement entre les sections principales : Accueil, Services, et Contact.

---

## **Fonctionnalités**

- **Page d'accueil** : Présente une vue générale du site.
- **Page des services** : Détaille les services proposés.
- **Page de contact** : Fournit des informations de contact et un formulaire.

---

## **Structure du Projet**

- **app.py** : Contient le code principal de l'application.
- **templates/** : Dossier des fichiers HTML.
  - `accueil.html` : Page d'accueil.
  - `serv.html` : Page des services.
  - `contact.html` : Page de contact.
- **static/** : Dossier réservé aux images.
- **envir/** : (Non inclus dans le dépôt GitHub) Environnement virtuel recommandé pour isoler les dépendances.

---

## **Installation et Exécution**


### **Étapes d'installation**

1. **Clonez le dépôt GitHub :**
   ```bash
   git clone https://github.com/projet-ka-im/markelite.git
   cd miniprojet
   ```

2. **Créez et activez un environnement virtuel :**
   - Sur Windows :
     ```bash
     python -m venv envir
     envir\Scripts\activate
     ```
   - Sur macOS/Linux :
     ```bash
     python -m venv envir
     source envir/bin/activate
     ```

3. **Installez les dépendances :**
   ```bash
   pip install flask
   ```

4. **Lancez l'application :**
   ```bash
   python app.py
   ```

5. **Accédez à l'application dans votre navigateur :**
   ```
   http://127.0.0.1:5000/
   ```

---

## **Exemple de Code (app.py)**

Voici un aperçu du fichier `app.py` :

```python
from flask import Flask, render_template

app = Flask(__name__)

@app.route('/')
def accueil():
    return render_template('accueil.html')

@app.route('/services')
def services():
    return render_template('serv.html')

@app.route('/contact')
def contact():
    return render_template('contact.html')

if __name__ == '__main__':
    app.run(debug=True)
```

---

## **Captures d'Écran**

1. **Page d'accueil**  
   ![acl1](https://github.com/user-attachments/assets/7bde431d-3dea-4933-adfd-2e415a1150b7)

   
   ![acl2](https://github.com/user-attachments/assets/353bb6e6-4d4a-4237-9968-3b37422531f3)
  
  
   ![acl3](https://github.com/user-attachments/assets/f370bdfe-b705-4ae0-acc5-aa179a2ff608)
  
  
   ![acl4](https://github.com/user-attachments/assets/77d9fd0f-c393-42b5-b867-65e862d11d4c)
  
  
   ![acl5](https://github.com/user-attachments/assets/4125d6ff-7b41-4280-9d6f-dfbfef57ad70)


3. **Page des services**  
   ![srv1](https://github.com/user-attachments/assets/b019fd34-19eb-4e1e-b4c4-767d2fd437c3)


   ![srv2](https://github.com/user-attachments/assets/d8724586-2600-43a5-9e6f-133a83197748)


   ![srv3](https://github.com/user-attachments/assets/7f0b3a74-823f-4bf3-bd24-2a5c625b2fb7)


4. **Page de contact**  
   !![contact](https://github.com/user-attachments/assets/b779e3e9-508e-4464-b90d-53bbf3f16d70)

---

## **Auteur**


- Contact : [markeliteagence@gmail.com]

---

## **Remarques**

- L'environnement virtuel (`envir`) n'est pas inclus dans le dépôt pour éviter des problèmes lors de l'exécution..

