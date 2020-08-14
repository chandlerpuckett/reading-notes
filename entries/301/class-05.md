# Heroku

## CHEATSHEET

chandlerpuckett~$ brew install heroku/brew/heroku
Updating Homebrew...
==> Auto-updated Homebrew!
Updated 2 taps (homebrew/core and homebrew/services).
==> New Formulae
acl2                 charge               empty                microplane           sqlite-utils         ugrep
cbc                  datasette            gostatic             osm                  staticcheck
cgl                  eleventy             kondo                pandocomatic         terraform@0.12
==> Updated Formulae
Updated 281 formulae.
==> Deleted Formulae
wpscan

Warning: heroku/brew/heroku 7.42.6 is already installed and up-to-date
To reinstall 7.42.6, run `brew reinstall heroku`
chandlerpuckett~$ heroku login
heroku: Press any key to open up the browser to login or q to exit: 
Opening browser to https://cli-auth.heroku.com/auth/cli/browser/87a44afb-414d-4374-9b00-ce74f8b8e8d4?requestor=SFMyNTY.g3QAAAACZAAEZGF0YW0AAAAMNjcuMTcwLjYzLjc4ZAAGc2lnbmVkbgYA6CqC7XMB.N8hDv1t2avX3rwFRjxt_ozq0i8OOBlETWiR5akrahfQ
Logging in... done
Logged in as chandler.puckett1@gmail.com
chandlerpuckett~$ node --version
v14.7.0
chandlerpuckett~$ npm --version
6.14.7
chandlerpuckett~$ git --version
git version 2.26.2
chandlerpuckett~$ cd documents/projects/codefellows/301
chandlerpuckett~/documents/projects/codefellows/301$ ls
CHEATSHEETS			lab-01				portfolio
JQUERY				lab-02				seattle-301d65
code-review			lab-03
data-structures-and-algorithms	lab-04
chandlerpuckett~/documents/projects/codefellows/301$ mkdir heroku
chandlerpuckett~/documents/projects/codefellows/301$ ls
CHEATSHEETS			heroku				lab-04
JQUERY				lab-01				portfolio
code-review			lab-02				seattle-301d65
data-structures-and-algorithms	lab-03
chandlerpuckett~/documents/projects/codefellows/301$ cd heroku
chandlerpuckett~/documents/projects/codefellows/301/heroku$ git clone https://github.com/heroku/node-js-getting-started.git
Cloning into 'node-js-getting-started'...
remote: Enumerating objects: 571, done.
remote: Total 571 (delta 0), reused 0 (delta 0), pack-reused 571
Receiving objects: 100% (571/571), 259.31 KiB | 979.00 KiB/s, done.
Resolving deltas: 100% (114/114), done.
chandlerpuckett~/documents/projects/codefellows/301/heroku$ ls
node-js-getting-started
chandlerpuckett~/documents/projects/codefellows/301/heroku$ heroku create
Creating app... done, ⬢ agile-anchorage-26997
https://agile-anchorage-26997.herokuapp.com/ | https://git.heroku.com/agile-anchorage-26997.git
chandlerpuckett~/documents/projects/codefellows/301/heroku$ git push heroku master
fatal: not a git repository (or any of the parent directories): .git
chandlerpuckett~/documents/projects/codefellows/301/heroku$ ;s
-bash: syntax error near unexpected token `;'
chandlerpuckett~/documents/projects/codefellows/301/heroku$ ls
node-js-getting-started
chandlerpuckett~/documents/projects/codefellows/301/heroku$ cd node-js-getting-started
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ ls
Procfile	app.json	package.json	test.js
README.md	index.js	public		views
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ heroku create
Creating app... done, ⬢ ancient-shore-60631
https://ancient-shore-60631.herokuapp.com/ | https://git.heroku.com/ancient-shore-60631.git
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ git push heroku master
Enumerating objects: 522, done.
Counting objects: 100% (522/522), done.
Delta compression using up to 8 threads
Compressing objects: 100% (393/393), done.
Writing objects: 100% (522/522), 240.74 KiB | 120.37 MiB/s, done.
Total 522 (delta 94), reused 522 (delta 94), pack-reused 0
remote: Compressing source files... done.
remote: Building source:
remote: 
remote: -----> Node.js app detected
remote:        
remote: -----> Creating runtime environment
remote:        
remote:        NPM_CONFIG_LOGLEVEL=error
remote:        NODE_ENV=production
remote:        NODE_MODULES_CACHE=true
remote:        NODE_VERBOSE=false
remote:        
remote: -----> Installing binaries
remote:        engines.node (package.json):  12.x
remote:        engines.npm (package.json):   unspecified (use default)
remote:        
remote:        Resolving node version 12.x...
remote:        Downloading and installing node 12.18.3...
remote:        Using default npm version: 6.14.6
remote:        
remote: -----> Installing dependencies
remote:        Installing node modules (package.json)
remote:        
remote:        > ejs@2.7.4 postinstall /tmp/build_da7f3fea/node_modules/ejs
remote:        > node ./postinstall.js
remote:        
remote:        added 120 packages from 106 contributors and audited 120 packages in 4.797s
remote:        
remote:        23 packages are looking for funding
remote:          run `npm fund` for details
remote:        
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build
remote:        
remote: -----> Caching build
remote:        - node_modules
remote:        
remote: -----> Pruning devDependencies
remote:        removed 69 packages and audited 51 packages in 1.432s
remote:        found 0 vulnerabilities
remote:        
remote:        
remote: -----> Build succeeded!
remote: -----> Discovering process types
remote:        Procfile declares types -> web
remote: 
remote: -----> Compressing...
remote:        Done: 22.8M
remote: -----> Launching...
remote:        Released v3
remote:        https://ancient-shore-60631.herokuapp.com/ deployed to Heroku
remote: 
remote: Verifying deploy... done.
To https://git.heroku.com/ancient-shore-60631.git
 * [new branch]      master -> master
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ heroku ps:scale web=1
Scaling dynos... done, now running web at 1:Free
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ heroku open
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ heroku logs --tail:
 ›   Error: Unexpected argument: --tail:
 ›   See more help with --help
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ heroku logs --tail
2020-08-14T15:10:42.371397+00:00 app[api]: Initial release by user chandler.puckett1@gmail.com
2020-08-14T15:10:42.371397+00:00 app[api]: Release v1 created by user chandler.puckett1@gmail.com
2020-08-14T15:10:42.698711+00:00 app[api]: Enable Logplex by user chandler.puckett1@gmail.com
2020-08-14T15:10:42.698711+00:00 app[api]: Release v2 created by user chandler.puckett1@gmail.com
2020-08-14T15:10:57.000000+00:00 app[api]: Build started by user chandler.puckett1@gmail.com
2020-08-14T15:11:14.925528+00:00 app[api]: Release v3 created by user chandler.puckett1@gmail.com
2020-08-14T15:11:14.925528+00:00 app[api]: Deploy a8ca3c56 by user chandler.puckett1@gmail.com
2020-08-14T15:11:14.946507+00:00 app[api]: Scaled to web@1:Free by user chandler.puckett1@gmail.com
2020-08-14T15:11:15.000000+00:00 app[api]: Build succeeded
2020-08-14T15:11:16.926625+00:00 heroku[web.1]: Starting process with command `node index.js`
2020-08-14T15:11:19.028264+00:00 app[web.1]: Listening on 17884
2020-08-14T15:11:19.264011+00:00 heroku[web.1]: State changed from starting to up
2020-08-14T15:11:43.289482+00:00 heroku[router]: at=info method=GET path="/" host=ancient-shore-60631.herokuapp.com request_id=f60da064-4f1b-4488-9115-6ec90eaf238c fwd="67.170.63.78" dyno=web.1 connect=0ms service=27ms status=200 bytes=7074 protocol=https
2020-08-14T15:11:43.447215+00:00 heroku[router]: at=info method=GET path="/stylesheets/main.css" host=ancient-shore-60631.herokuapp.com request_id=65d3ce11-8032-492f-aae6-8d8f3c821802 fwd="67.170.63.78" dyno=web.1 connect=0ms service=6ms status=200 bytes=908 protocol=https
2020-08-14T15:11:43.662544+00:00 heroku[router]: at=info method=GET path="/lang-logo.png" host=ancient-shore-60631.herokuapp.com request_id=a5d6b92f-81af-4bb5-a7bb-8d7b71a10951 fwd="67.170.63.78" dyno=web.1 connect=0ms service=3ms status=200 bytes=2567 protocol=https
2020-08-14T15:11:44.343937+00:00 heroku[router]: at=info method=GET path="/favicon.ico" host=ancient-shore-60631.herokuapp.com request_id=e0e42149-866c-4f2b-aab8-305d732700d3 fwd="67.170.63.78" dyno=web.1 connect=0ms service=4ms status=404 bytes=394 protocol=https
^C
chandlerpuckett~/documents/projects/codefellows/301/heroku/node-js-getting-started[master]$ 

