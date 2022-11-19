# Aleo Client & Prover Node

<p align="center">
  <img width="460" height="300" src="https://pbs.twimg.com/media/FhKBJarXoAIaFnA?format=jpg&name=large">
</p>

## Hardware Specifications

| Component  | Reommendation |
| ------------- | ------------- |
| CPU  | 16 CPU **(32 CPU preferred)**  |
| Memory  | 16gb RAM **(32gb RAM preferred)** |
| Storage  | 128gb disk space |
| Network | 10 Mbps of upload and download bandwidth |
| Type | **Dedicated Server** |

# How to Run Aleo Client and Prover Node

## **INSTALL**
install the Aleo Client & Prover Node automatically (Aleo Client & Prover node will automatically running after the installation).

```
wget -q -O aleo_snarkos3.sh https://api.nodes.guru/aleo_snarkos3.sh && chmod +x aleo_snarkos3.sh && sudo /bin/bash aleo_snarkos3.sh
```

## Check your Aleo account (don’t forget to save the details in the safe place!)

```
cat $HOME/aleo/account_new.txt
```

## Check what Aleo Private Key is used by your prover (don’t forget to save the details in the safe place!)

```
grep "prover" /etc/systemd/system/aleo-prover.service | awk '{print $5}'
```

## Check aleo prover logs

```
journalctl -u aleo-prover -f -o cat
```

## Check the aleo client logs if it is running

```
journalctl -u aleo-client -f -o cat
```
