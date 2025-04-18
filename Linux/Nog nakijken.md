
- sudo dnf install -y git-credential-libsecret
	- Hiermee install je een git helper genaamd 'libsecret'
	  Libsecret kan gebruikt worden om wachtwoorden en gebruikersnamen op te slaan. Zonder deze, zal git elke keer om een username en wachtwoord vragen nadat er een 'git push' acties uitgevoerd wordt

- `git init`
	- Starts / "Initializes" git through terminal

- `echo ".obsidian/workspace" >> .gitignore`
	- Door ".obsidian/workspace" toe te voegen aan .gitignore, zal git de workspace file negeren.
	  In deze file word o.a. de layout instellingen van de obsidian workspace bewaard. Hiermee voorkom je dat er geen ongewenste veranderingen aan jouw obsidian workspace layout plaats vind.