FROM ethereum/client-go:alltools-v1.8.19

COPY data root/.ethereum 
COPY password .
CMD swarm --bootnodes "enode://$BOOTNODE_ID@$BOOTNODE_IP:30301" --bzzaccount $ACCOUNT_ADDRESS --password password --bzzapi "0.0.0.0" --corsdomain "*" --httpaddr "0.0.0.0"

EXPOSE 8500
EXPOSE 30399