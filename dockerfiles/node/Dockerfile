FROM node:16-alpine

# instale o bash no container pois alpine vem sem o bash
RUN apk add --no-cache bash

WORKDIR /app

RUN npm install -g nodemon

COPY . .

# obs o bind da pasta com o projeto so acontece depois do container construido
# os comandos abaixo foram movidos para script que este é executado apos o bind da pasta estar pronto
CMD ["/bin/bash", "start.sh"]


#RUN ls -la

#COPY package*.json ./

#RUN npm install -g @angular/cli@14.2.13

#RUN npm install  // vai rodar no scrpit start.sh

# Ou, se preferir instalar localmente:
# RUN npm install --save-dev nodemon  

#CMD [ "npm", "start" ]

# Comando para manter um container online
#ENTRYPOINT ["/bin/bash"]
#CMD ["-c", "tail -f /dev/null"]
