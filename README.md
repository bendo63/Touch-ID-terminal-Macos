# Touch-ID-terminal-Macos

Source : https://www.macg.co/os-x/2017/11/comment-utiliser-touch-id-dans-le-terminal-commande-sudo-100446

Ouvrer votre terminal
#sauvegader votre fichier d'origine
sudo cp /etc/pam.d/sudo /etc/pam.d/sudo.bak

#modifier avec nano le fichier
sudo nano /etc/pam.d/sudo

#ajouter sous la ligne "# sudo: auth account password session"
auth       sufficient     pam_tid.so

![Capture d’écran 2022-04-03 à 20 16 21](https://user-images.githubusercontent.com/42283374/161442236-9158751d-b12c-4f7b-86cd-7fca5bc7ff81.png)

#fin!
[Capture d’écran 2022-04-03 à 20 16 12](https://user-images.githubusercontent.com/42283374/161442228-4a8bdd6e-53ce-45b0-9266-4945164b25bb.png)
