Installation
============

Install Ruby
------------

OS X and most Linux systems come with Ruby pre-installed. 

For more information refer to [ruby-lang.org](https://www.ruby-lang.org/en/downloads/).

Install RVM
-----------

"[Ruby Virtual Manager] is a command-line tool which allows you to easily install, manage, and work with multiple ruby environments from interpreters to sets of gems."

    $ curl -L https://get.rvm.io | bash

For more information refer to [rvm.io](https://rvm.io/rvm/install)

Update RubyGems
---------------

RubyGems is a package management framework for Ruby.

    $ gem update --system 

For more information refer to [rubygems.org](http://rubygems.org/pages/download)

Install with RubyGems
---------------------

The best way to install Jekyll is via RubyGems.
At the terminal prompt, simply run the following command to install Jekyll

    $ gem install jekyll

For more information refer to [jekyllrb.com](http://jekyllrb.com/docs/installation/)

Running with Jekyll
-------------------

Basic Usage
The Jekyll gem makes a jekyll executable available to you in your Terminal window. You can use this command in a number of ways:

    $ jekyll build
    # => The current folder will be generated into ./_site

    $ jekyll build --destination <destination>
    # => The current folder will be generated into <destination>

    $ jekyll build --source <source> --destination <destination>
    # => The <source> folder will be generated into <destination>

    $ jekyll build --watch
    # => The current folder will be generated into ./_site,
    #    watched for changes, and regenerated automatically.

Jekyll also comes with a built-in development server that will allow you to preview what the generated site will look like in your browser locally.

    $ jekyll serve
    # => A development server will run at http://localhost:4000/

    $ jekyll serve --detach
    # => Same as `jekyll serve` but will detach from the current terminal.
    #    If you need to kill the server, you can `kill -9 1234` where "1234" is the PID.
    #    If you cannot find the PID, then do, `ps aux | grep jekyll` and kill the instance.

    $ jekyll serve --watch
    # => Same as `jekyll serve`, but watch for changes and regenerate

For more information refer to [jekyllrb.com](http://jekyllrb.com/docs/usage/)
