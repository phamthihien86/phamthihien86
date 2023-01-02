Build:
- yarn build:client
- yarn build:admin

Release:
- node release.js client
- node release.js admin

pm2 start npm --name "client" -- run "start:client"
pm2 start npm --name "admin" -- run "start:admin"
