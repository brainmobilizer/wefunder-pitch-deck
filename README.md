# Pitch Deck Uploader

## Prerequisites

* Ruby version `2.7.2`

- Rmagick:

  For ubuntu: https://github.com/rmagick/rmagick#ubuntu

  For macOs: https://github.com/rmagick/rmagick#macos

## How To Run

1. Install bundle
```
  bundle install --path vendor/bundle
```

2. Setup DB and seed data
  ```
    bundle exec rails db:drop db:create db:migrate db:seed
  ```

3. Run the app
```
### Rails server
bundle exec rails s

### Sidekiq server
bundle exec sidekiq default mailers

### Mailcatcher server
bundle exec mailcatcher
```

4. Browse the app at http://localhost:3000

5. Either login by existing emails that are in the format: test_#{i}@example.com, where i is a number of 0 to 9. Password is `12345678`, or sign up with your email.

*Note: To check email please go to http://127.0.0.1:1080/*
