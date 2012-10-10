# rabbitmq-service-rails-sample

This is a very simple Rails 3 application demonstrating the use of the
RabbitMQ Bigwig add-on on Heroku.

To try out the sample for yourself, clone the repository and, in its base directory, run the following:

    $ heroku create
    Creating hollow-mountain-815... done, stack is bamboo-mri-1.9.2
    http://hollow-mountain-815.heroku.com/ |
    git@heroku.com:hollow-mountain-815.git
    Git remote heroku added
    $ git push heroku master
    Counting objects: 64, done.
    Delta compression using up to 2 threads.
    Compressing objects: 100% (49/49), done.
    Writing objects: 100% (64/64), 86.59 KiB, done.
    Total 64 (delta 2), reused 0 (delta 0)
    
    -----> Heroku receiving push
    -----> Ruby/Rails app detected
    -----> Detected Rails is not set to serve static_assets
           Installing rails3_serve_static_assets... done
    -----> Configure Rails 3 to disable x-sendfile
           Installing rails3_disable_x_sendfile... done
    -----> Configure Rails to log to stdout
           Installing rails_log_stdout... done
    -----> Gemfile detected, running Bundler version 1.0.7
           Unresolved dependencies detected; Installing...
           Using --without development:test
           Fetching source index for http://rubygems.org/
           [...]
           Your bundle is complete! It was installed into ./.bundle/gems/
    -----> Compiled slug size is 4.1MB
    -----> Launching... done, v4
           http://hollow-mountain-815.heroku.com deployed to Heroku
    
    To git@heroku.com:hollow-mountain-815.git
    * [new branch]      master -> master

Your own application will get a name different from `hollow-mountain-815`. You can change this name in your [Heroku web console](https://api.heroku.com/myapps) if you'd like.

Then provision a RabbitMQ Bigwig instance:

    $ heroku addons:add rabbitmq-bigwig

And visit your sample application!