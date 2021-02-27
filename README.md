# Writing Challenges App (back end)

Ever wanted a way for participants of your writing challenge to track each other's progress?

This is the Rails API for Writing Challenges App, a single page React app (in progress!) where users can create and join writing challenges and keep track of their projects with a word count tracker.


## Dependencies

This API was built with PostgreSQL, so you will need to have it installed on your computer to create the databases needed to run it. I found [this article](https://medium.com/@noordean/setting-up-postgresql-with-rails-application-357fe5e9c28) particularly helpful in that regard.


## Installation

1. Fork the repository
2. Clone the files to your computer
3. Navigate to `/writing-challenges-api` in your terminal
4. Create a `.env` file, and include this in it:
```
POSTGRES_USER='your_postgres_username'
POSTGRES_PASSWORD='your_postgres_password'
POSTGRES_HOST='localhost'
POSTGRES_DB='writing_challenges_api_db'
POSTGRES_TEST_DB='writing_challenges_api_test_db'
POSTGRES_DEVELOPMENT_DB='writing_challenges_api_development_db'
```
4. Run `bundle install`
5. Run `rails db:migrate`
6. Run `rails db:seed`. This step is very important as it loads badgetypes into the app!
7. Run `rails s` to start the server. Make sure to run the React app at the same time as well!

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License
[MIT](https://choosealicense.com/licenses/mit/)
