Run the node
Command: docker compose --env-file ./.env -f ./docker-compose.yml up -d

Check the logs of the prysm service to monitor the synchronization progress:
Command: docker compose --env-file ./.env -f ./docker-compose.yml logs -f prysm --tail 20

Check the logs of the geth service to monitor the initial download and sync progress:
Command: docker compose --env-file ./.env -f ./docker-compose.yml logs -f geth --tail 20


Doc: https://docs.polygon.technology/zkEVM/get-started/deploy-zkevm/setup-goerli-node/#deploy
