# unofficial-ekool-python-api

## Getting the creds (idk if its legal to post api keys from the app publicly)
step 1: decompile the ekool app and get the CLIENT_ID and the CLIENT_SECRET from sources/eu/ekool/app/BuildConfig.java

## getting actual stuff from thge api
step 0: replace the {{}} stuff with the values you got in the thingy

step 1: go to this url, log in and copy everything after "code=" in the new link
https://login.ekool.eu/oauth/authorize?client_id={{CLIENT_ID}}&redirect_uri=https%3A%2F%2Flogin.ekool.eu%2Fcallback&response_type=code&scope=mkool-api

step 2: put code after the "code=" in this link and get a refresh token
https://login.ekool.eu/oauth/token/grant_type=authorization_code&client_id={{CLIENT_ID}}&client_secret={{CLIENT_SECRET}}&redirect_uri=https%3A%2F%2Flogin.ekool.eu%2Fcallback&code=

atp you can follow the docs
https://api-docs-public.ekool.eu/

ill write an actual api later lol
