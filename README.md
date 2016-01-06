# tumblr-downloader
Tumblr photo and video downloader with mail reporting

# features
- crawl tumblr and download photos and video
- skip already downloaded files
- crawn completly the tumblr the first time
- auto stop when parsing alrady indexed files

# technichal stack
- java 6
- jsoup 1.8 for html parsing
- velocity for mail reporting
- xuggle 5.2 for video thumbnailing

# execute
- download the jar [TumblrDownloader-1-jar-with-dependencies.jar](dist/TumblrDownloader-1-jar-with-dependencies.jar)
- create a config file like below
- execute the batch and pass the config file folder location :
Exemple if your config file is in the same folder than your jar :
java -jar TumblrDownloader-1-jar-with-dependencies.jar "."

# config file example
\# destination of downloaded files
destination.folder=/volume1/photo/tumblrs

\# list of tumblr to download
tumblr.list.download=http://awesomecatvideos.tumblr.com/
tumblr.list.download=http://cat-shaming.tumblr.com/
tumblr.list.download=http://unimpressedcats.tumblr.com/
tumblr.list.download=http://iheartcatgifs.tumblr.com/
tumblr.list.download=http://catsof.tumblr.com/

\# for synology nas only :
\# index downloaded media file (execute synoindex -a [file] on all files)
tumblr.execute.synoindex=true
\# number of page to index before stoping for
tumblr.deep.page.number=10

\# Mail configuration
\# notes : to work, you need to configure gmail to activate less secure apps :
\# https://www.google.com/settings/security/lesssecureapps
gmail.username=[yourmail]@gmail.com
gmail.password=[your password]
mail.destination=[destination mail]

# source code
Because the code source is not yet ready to be published, I will only publish it in a few day or week.
