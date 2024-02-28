# Dusk-ITN-Node
#1 siapkan node https://docs.dusk.network/getting-started/node-setup/node-requirements

#2 ``` sudo apt update && sudo apt upgrade ```

#3 ``` sudo ufw allow 9000/udp
sudo ufw allow 8080/tcp 
sudo ufw enable 
suufw allow 22 
sudo ufw enable ```

#4 Instal Rusk ``` curl --proto '=https' --tlsv1.2 -sSfL https://github.com/dusk-network/itn-installer/releases/download/v0.1.4/itn-installer.sh | sudo sh ```
cek update Rusk https://github.com/dusk-network/itn-installer/

#5 ``` rusk-wallet restore ``` Huruf Kecil semua

#6 ``` rusk-wallet export -d /opt/dusk/conf -n consensus.keys ```

#7 ``` sh /opt/dusk/bin/setup_consensus_pwd.sh ```

#8 ``` service rusk start ```

#9 ``` tail -F /var/log/rusk.log ```

# Staking

#1 ``` rusk-wallet stake --amt 1000 ``` Sesuaikan 

#2 ``` rusk-wallet stake-info ```

#3 ``` grep "execute_state_transition" /var/log/rusk.log | tail -n 5 ```
