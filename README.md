# LLM Pruebas
Repositorio de proyectollm



# 1. Instalación

Como primer paso descargamos [Ollama](https://ollama.com/library) de su pagina WEB

```` bash
$ curl -fsSL https://ollama.com/install.sh | sh 

````

## 2. Ejecutar el Servidor
Ejecutar el servidor API REst de ollama con el siguiente comando.
```` bash
$ ollama serve

````

## 3. Descargar un Modelo
En la página WEB [Ollama](https://ollama.com/library) Utilizando el siguiente comando:

```` bash
$ ollama pull tinyllama

````
Se debe abrir primero una terminal
ollama run gemma2
ollama list



## 4. Visualizar APIS
En la página WEB [APIS](https://github.com/ollama/ollama/blob/main/docs/api.md) Utilizando el siguiente comando:

curl http://localhost:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt": "Why is the sky blue?"
}'

curl http://localhost:11434/api/generate -d '{
  "model": "ollama3",
  "prompt": "Why is the sky blue?"
}'


curl http://localhost:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt": "Why is the sky blue?"
}' -o salida.md

curl http://localhost:11434/api/generate -d '{
  "model": "tinyllama",
  "prompt": "Why is the sky blue?",
  "stream": false
}'


## 5. Indexar
Comandos:
git add .
git commit -m "UPDTED README.md"
git push -u origin 
