# Kanban

It's just a Kanban board made with Ruby on Rails, but it's pretty. More information in [this blog post](http://wedontneedroads.net/post/15571399433/kaban-web-app).

![Kanban](http://f.cl.ly/items/0k031R2Q1r0R3B1E063Z/tumblr_lxcacrE1PR1qzze81o1_r3_1280.png)

# Installation

## February 28, 2014

```bash
$ ruby --version
ruby 1.9.2p320 (2012-04-20 revision 35421) [x86_64-darwin12.5.0]

$ git clone https://github.com/KevinBongart/Kanban.git
$ cd Kanban/

$ gem install --local gems/coffee-script-source-1.1.3.gem 
Successfully installed coffee-script-source-1.1.3
Parsing documentation for coffee-script-source-1.1.3
Installing ri documentation for coffee-script-source-1.1.3
Done installing documentation for coffee-script-source after 0 seconds
1 gem installed

$ bundle install

$ rake db:setup
db/test.sqlite3 already exists
db/development.sqlite3 already exists
-- create_table("attached_copies", {:force=>true})
   -> 0.0184s
-- create_table("attached_images", {:force=>true})
   -> 0.0021s
-- create_table("comments", {:force=>true})
   -> 0.0019s
-- create_table("projects", {:force=>true})
   -> 0.0017s
-- create_table("states", {:force=>true})
   -> 0.0017s
-- create_table("stories", {:force=>true})
   -> 0.0413s
-- create_table("tasks", {:force=>true})
   -> 0.0023s
-- create_table("users", {:force=>true})
   -> 0.0021s
-- initialize_schema_migrations_table()
   -> 0.0030s
-- assume_migrated_upto_version(20111128060848, ["/path/to/Kanban/db/migrate"])
   -> 0.0186s

$ rails server
=> Booting WEBrick
=> Rails 3.1.2 application starting in development on http://0.0.0.0:3000
=> Call with -d to detach
=> Ctrl-C to shutdown server
[2014-02-28 10:50:04] INFO  WEBrick 1.3.1
[2014-02-28 10:50:04] INFO  ruby 1.9.2 (2012-04-20) [x86_64-darwin12.5.0]
[2014-02-28 10:50:04] INFO  WEBrick::HTTPServer#start: pid=73773 port=3000
```
