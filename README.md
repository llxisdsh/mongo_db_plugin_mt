# mongo_db_plugin_mt

1.copy to eos\plugins\mongo_db_plugin\

2.eosio_build.sh

3.check
nodeos --help | grep mongodb-thread-size

4.edit config.ini, require mongodb-thread-size < maxPoolSize :
mongodb-thread-size = 90
mongodb-uri = mongodb://xxx.xxx.xxx.xxx:27017/EOS?maxPoolSize=100

5.nodeos start
