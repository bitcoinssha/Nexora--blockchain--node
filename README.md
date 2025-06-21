README.md

# Nexora-Core Blockchain

Bienvenido al nodo local de Nexora Blockchain. Este entorno fue desarrollado para pruebas y visualización rápida de la red Nexora. Compatible con MetaMask y Trust Wallet mediante conexión local o vía túnel HTTPS.

## 🚀 Requisitos

- Ubuntu 20.04+ o compatible
- Node.js y npm (opcional para frontend)
- Go Ethereum (`geth`) instalado
- MetaMask (desktop o móvil)
- Ngrok (opcional para tunelado HTTPS)

## 📂 Archivos del Repositorio

- `start-nexora-node.sh` → Script para iniciar el nodo
- `genesis.json` → Configuración del bloque génesis de la blockchain
- `password.txt` → Contraseña para desbloqueo de la cuenta preminada

## 🔧 Instrucciones de uso

### 1. Instalar Go Ethereum

```bash
sudo add-apt-repository -y ppa:ethereum/ethereum
sudo apt-get update
sudo apt-get install ethereum -y

2. Clonar este repositorio

git clone https://github.com/tuusuario/Nexora-Core.git
cd Nexora-Core

3. Dar permisos al script

chmod +x start-nexora-node.sh

4. Iniciar el nodo

./start-nexora-node.sh

Esto:

Crea el directorio de datos nexora-data

Inicializa la blockchain con el genesis.json

Desbloquea la cuenta inicial con los fondos

Lanza el nodo con puerto RPC en http://127.0.0.1:8545


🧪 Probar la red

En MetaMask, añadir red personalizada:

Nombre: Nexora Mainnet (local)
RPC URL: http://127.0.0.1:8545
ID de cadena: 2025
Símbolo: NEX
Explorador de bloques: (vacío)

🔐 Cuenta Preminada

Puedes importar la cuenta con esta dirección (o usando el archivo keystore que se genera):

Dirección: 0xF09... (según lo generado)
Contraseña: 1234 (ver `password.txt`)

🌐 Acceso Externo (opcional)

Para acceder desde MetaMask móvil o Trust Wallet, puedes usar Ngrok:

ngrok http 8545

Luego toma el endpoint HTTPS y agrégalo como RPC en MetaMask.

📦 Versión

Nexora v1.0 - Nodo local de desarrollo

