# NFHS Network Interview Prep
### Blog Challenge - Rails (API Only)

This challenge is designed to assess your skills in setting up a basic blog API using Ruby on Rails. You will be implementing various aspects of a typical Rails application, including CRUD operations, controller security, ActiveRecord associations, data validation, and model callbacks.

### Important Note
This is an **API-only** challenge. There is no need to implement any application views or templates. You should use Rails in **API mode** and focus on building the backend logic for a blog API.

If you encounter any questions or issues while getting started, please feel free to reach out.

### Prerequisites
- This project uses Devise for authentication, which has already been preconfigured.

- A default user has been provisioned already and can be passed to the API via basic auth for this challenge.

  ```bash
  dev@example.com
  abc@123
  ```

### Submission

Once finished, please upload your submission to github and provide a link through the communication channel you have been using thus far.


## Getting Started

```bash
# install dependencies
bundle install

# setup the database
rails db:create
rails db:migrate

# serve the application
rails s

# run tests
bundle exec rspec
```

## Requirements

### 1. Generate Models

#### Post Model
- Use the Rails command line to generate a model named `Post`.
- Include attributes for `title` and `content`.
- Also, include a reference to the `User` model.

#### Comment Model
- Use the Rails command line to generate a model named `Comment`.
- Add attributes for `body`, and references to both `User` and `Post`.

### 2. Generate Controllers
- Use the Rails command line to generate API-only controllers for `Posts` and `Comments`.

### 3. Model Callback
- Implement a callback in the Post model that generates a URL-friendly slug based on the post's `title` before saving.

### 4. Setup Basic CRUD
- Implement basic CRUD (Create, Read, Update, Delete) operations for `Posts`.
- Ensure that these actions follow RESTful conventions.

### 5. Controller Security
- Utilize Devise for authentication. Ensuring only signed_in users can create, edit, and delete posts.
- There should be no restrictions for viewing posts and comments (read-only access).
- Set up authorization rules to ensure that users can only update or delete their own resources.

### 6. Data Validation
- Implement validations where necessary.

