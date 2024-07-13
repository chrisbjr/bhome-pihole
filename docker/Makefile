up:
	@docker-compose up -d

up-recreate:
	@docker-compose up --force-recreate -d

down:
	@docker-compose down

destroy:
	@docker-compose down --rmi all --volumes --remove-orphans

shell:
	@docker compose exec -it pihole /bin/bash

update-whitelists:
	@docker exec pihole sh -c 'awk "{gsub(/^[[:space:]]+|[[:space:]]+$/, \"\"); if (NF) print}" /etc/pihole/whitelists.txt | xargs -I {} pihole -w {}'

update-adlists:
	@docker exec pihole pihole -g
