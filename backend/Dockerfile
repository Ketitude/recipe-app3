FROM node:14 
#Koristimo node:14 kao osnovni imidž koji dolazi sa Node.js verzijom 14 i NPM (Node Package Manager).

WORKDIR /app
#Postavljamo radni direktorijum unutar kontejnera na /app.

COPY package*.json ./
#Kopiramo package.json i package-lock.json iz radnog direktorijuma na lokalnu mašinu u radni direktorijum unutar kontejnera (/app)

RUN npm install
#Pokrećemo npm install kako bismo instalirali sve zavisnosti definisane u package.json

COPY . .
#Kopiramo sve fajlove i direktorijume iz vašeg radnog direktorijuma na vašu lokalnu mašinu u radni direktorijum unutar kontejnera (/app).

EXPOSE 5000
#Deklarišemo port 5000 koji će aplikacija koristiti za komunikaciju.

CMD ["node", "server.js"]
#Definišemo komandnu liniju koja će se izvršiti kada kontejner počne sa radom. 
#U ovom slučaju, pokrećemo aplikaciju pomoću Node.js i startujemo server.js.
