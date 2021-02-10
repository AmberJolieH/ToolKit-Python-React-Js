# GENERAL KNOWLEDGE 

## creating secret for web apps 

### uuid
 npm install -g uuid-cli 
just type uuid to create secret

### JWT secret
 - Recommendation to genereate a strong secret: create a random string using openssl (a library that should be installed in your Ubuntu/MacOS shell already). Run openssl rand -base64 10 to generate a random JWT secret.
