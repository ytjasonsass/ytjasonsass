git clone https://github.com/YOUR_GITHUB_USER_NAME/whatsapp-heroku-bot
cd whatsapp-heroku-bot
npm install
heroku login
heroku create your-app-name
heroku buildpacks:set heroku/nodejs
heroku buildpacks:add jontewks/puppeteer
heroku git:remote -a your-app-name
git push heroku main
heroku logs
