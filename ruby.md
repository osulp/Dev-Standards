Ruby
=======

Summary
--------
 1. Use the [Ruby Style Guide](https://github.com/bbatsov/ruby-style-guide) and [validate](https://github.com/bbatsov/rubocop) style.
 

Managing Dependencies
----------------------

Use [bundler](http://gembundler.com/). Check in your Gemfile to source control.

### Gemfile Organization

When organizing your Gemfile, do the following:
 1. Provide a version for all gems. Prefer ~> to >=.
 2. Begin with gems for all groups. Provide a comment explaining the purpose of each gem.
 3. If using JRuby, follow with MRI-platform and then JRuby platform-specific gems.
 4. Follow with development only gems

    ```ruby
    group :development do
    end
    ```

 5. Follow with a combined development/test group. Be sure all gems need to be in both groups.

    ```ruby
    group :development, :test do
    end
    ```
    * This group is usually for dependencies that you would require to run developmental commands
      as well as the test suite, but which are not needed for production. Things like guard. or gems
      which have generators.

 6. Follow with test group. These are gems that would only be used in a test environment.
    * This group should be able to be excluded and developmental commands can run.
