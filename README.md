# Formulaire de contact simple avec PHPMailer

Un simple formulaire de contact avec PHPMailer, reCAPTCHA et Bootstrap.

Utilisez-le pour fournir un simple formulaire de contact sur votre propre site Web et envoyer les messages avec SMTP. Ou utilisez-le comme base ou exemple pour créer votre propre formulaire de contact.

## Commencer

1. Téléchargez la dernière version du formulaire de contact: https://github.com/InfinityFreeHosting/contactform/releases
2. Extrayez l'archive sur votre propre ordinateur.
3. Copiez ou renommez le `config.example.php` pour `config.php`et modifier les paramètres requis.
4. Envoyez les fichiers extraits dans un sous-répertoire de votre compte d'hébergement (par exemple `htdocs/contact/`).
5. Accédez à http://your-domain.epizy.com/contact/ et essayez le formulaire!

### Comment obtenir vos informations d'identification SMTP

Pour pouvoir envoyer des messages avec ce formulaire de contact, vous aurez besoin d'un service SMTP fonctionnel. InfinityFree ne fournit pas cela avec un hébergement gratuit, mais vous pouvez utiliser des services SMTP tiers.

Gmail est une option simple et gratuite à utiliser. Vous pouvez utiliser Gmail pour envoyer vos messages comme suit:

1. Ouvrez un compte Gmail gratuit.
2. Activez l'authentification à deux facteurs sur le compte Google: https://myaccount.google.com/signinoptions/two-step-verification
3. Générez un mot de passe spécifique à l'application pour le compte: https://myaccount.google.com/apppasswords
4. Dans le fichier de configuration, définissez le nom d'hôte SMTP `smtp.gmail.com`, entrez votre adresse Gmail complète dans le champ Nom d'utilisateur SMTP et entrez le mot de passe spécifique à l'application dans le champ Mot de passe SMTP.

### Comment obtenir vos informations d'identification reCAPTCHA

Pour empêcher les spammeurs de pouvoir abuser de votre formulaire de contact, reCAPTCHA a été intégré par défaut. reCAPTCHA est un service gratuit de Google qui peut empêcher les scripts automatisés d'utiliser votre formulaire.

Ce formulaire de contact a été intégré à reCAPTCHA v2 avec le challenge Checkbox. Pour l'utiliser, vous devrez configurer votre site dans reCAPTCHA comme ceci:

1. Accédez à la console d'administration reCAPTCHA: https://www.google.com/recaptcha/admin/create
2. Saisissez une étiquette que vous pouvez utiliser pour identifier votre site Web.
3. Choisissez le type reCAPTCHA "reCAPTCHA v2" et la version "Case à cocher 'Je ne suis pas un robot'".
4. Sous Domaines, entrez le nom de domaine de votre site Web.
5. Acceptez les termes reCAPTCHA et cliquez sur Envoyer.
