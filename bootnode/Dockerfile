FROM ethereum/client-go:alltools-v1.8.19

COPY bootnode.key .
CMD bootnode --nodekey=bootnode.key

EXPOSE 30301/udp
EXPOSE 30303/udp