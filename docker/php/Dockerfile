FROM chekote/php:7.2.14-laravel5.7

RUN apt-get update && \
   apt-get install --no-install-recommends \
       --no-install-suggests -y \
       #
       # postgres requirements
       php${PHP_VERSION}-pgsql && \
       #
   # Cleanup
   apt-get remove -y && \
   apt-get autoremove -y && \
   apt-get clean && \
   rm -rf /var/lib/apt/lists/*

