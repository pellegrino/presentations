!SLIDE center

# Using Jackpot

!SLIDE 

Add jackpot and jquery-rails to your Gemfile

          gem 'jackpot'
          gem 'jquery-rails'

!SLIDE 

Add a initializer 

          Jackpot.configure do |c|
            c.gateway_type      :braintree
            c.gateway_login     'demo'
            c.gateway_password  'password'
            c.gateway_mode      :test
          end 

!SLIDE 

Copy jackpot's migrations to your project 

          bundle exec rake 
          jackpot:install:migrations
!SLIDE 

Mount the engine in your routes 

          mount Jackpot::Engine => "/billing"

!SLIDE 

Basic rails app powered by jackpot

[https://github.com/pellegrino/jackpot-demo](https://github.com/pellegrino/jackpot-demo)


!SLIDE 

# DEMO

