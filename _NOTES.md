# Important Notes

rails - t :: running all test
s time da se mora modificirati i Rake file kao što je ovdje navedeno

# Default: Run all spec files (i.e., those matching spec/**/*_spec.rb)
$ bundle exec rspec

# Run all spec files in a single directory (recursively)
$ bundle exec rspec spec/models

# Run a single spec file
$ bundle exec rspec spec/controllers/accounts_controller_spec.rb

# Run a single example from a spec file (by line number)
$ bundle exec rspec spec/controllers/accounts_controller_spec.rb:8

# See all options for running specs
$ bundle exec rspec --help

RSpec DSL Basics (or, how do I write a spec?)
In RSpec, application behavior is described first in (almost) plain English, then again in test code, like so:

RSpec.describe 'Post' do           #
  context 'before publication' do  # (almost) plain English
    it 'cannot have comments' do   #
      expect { Post.create.comments.create! }.to raise_error(ActiveRecord::RecordInvalid)  # test code
    end
  end
end

# Rubocop

Code Quality checks

#JS Routes
Neće se generirati ako se ne postavi path u config/initializers

# Instalation UI
shadcn/ui and bits with tailwindcss

# Auth

