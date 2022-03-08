FROM python:3  
#Puxando a imagem do python 3

RUN apt-get update -y && \ 
    #Comando para executar todos os repositórios de pacotes*/ 
    apt-get install -y python3-pip python-dev    
    #pacote necessários para rodar a API Flask 

WORKDIR /app

RUN pip install Flask
RUN pip install requests
#Pacotes necessários para rodar a API

COPY . ./
#Copiando todo o diretório para o diretório de trabalho 

EXPOSE 5000
#Expondo a porta 5000 para acesso ao projeto

CMD ["python", "./app.py"]
#Comando que vai executar o projeto


