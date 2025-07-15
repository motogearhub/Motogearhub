unzip motogearhub_website.zip
cd motogearhub_website
index.html  style.css  shop.html  reviews.html  blog.html  about.html  contact.html
git init
git add .
git commit -m "Initial commit – MotoGearHub website"
gh repo edit --add-topic affiliate,motorcycle,gear
gh api -X PUT repos/:owner/motogearhub/pages --input - <<< '{"source":{"branch":"main","path":"/"}}'
