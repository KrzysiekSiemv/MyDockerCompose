Dodatkowo do php'a należy dorzucić dodatki takie jak:
```
sudo docker exec -it local_php apt-get update && apt-get install -y \
        libfreetype6-dev \
        libjpeg62-turbo-dev \
        libpng-dev \
    && docker-php-ext-configure gd --with-freetype --with-jpeg \
    && docker-php-ext-install gd mbstring mysqli pdo iconv bz2 bcmath xsl xml xmlreader zip readline pgsql intl json session
```
