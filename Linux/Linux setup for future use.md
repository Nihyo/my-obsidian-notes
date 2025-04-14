- Obsidian
	- Installeer Obsidian (`flatpak run md.obsidian.Obsidian`)
	- Definieer vault locatie (`cd ~/Documents/"Obsidian Vault"`) via terminal
	  
	- Git
		- Install Git (`sudo dnf install git`) / Check of git is already installed (`git --version`)
		- Koppeling naar github (michaeldiehart@hotmail.com)
		- install git
		- Autoinlog mogelijkheid met git (libsecret)
	- Script maken om auto git push acties uit te voeren bij afsluiting
		  Script ex.
			`#!/bin/bash`
			`#Start Obsidian (aangenomen dat het zo geïnstalleerd is)`
			`flatpak run md.obsidian.Obsidian  &`
		  
			#Wacht tot Obsidian afgesloten is`
			`obsidian_pid=$!`
			`wait $obsidian_pid`
			
			#`Vraag of je wil pushen`
			`read -p "Wil je je Obsidian-notities naar GitHub pushen? (j/n) " antwoord`
			`if [[ "$antwoord" == "j" || "$antwoord" == "J" || "$antwoord" == "y" || "antwoord" == "Y" ]]; then`
				`###### cd ~/Documents/Obsidian\ Vault`
				`###### git add .`
				`###### git commit -m "Update op $(date)"`
				`###### git push`
			`else`
				`###### echo "Push overgeslagen."`
			`fi`
		


		  
		  