# How to set up
1. install required packages
   - Ubuntu

     ```
     $ sudo apt install build-essential openssl libssl-dev zlib1g-dev
     ```

2. install rbenv

   ```
   $ git clone https://github.com/rbenv/rbenv.git ~/.rbenv
   $ cd ~/.rbenv && src/configure && make -C src
   $ echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
   $ rbenv init
   $ echo 'eval "$(rbenv init - bash)"' >> ~/.bash_profile
   ```

3. install ruby-build

   ```
   $ mkdir -p "$(rbenv root)"/plugins
   $ git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
   ```

4. install ruby

   ```
   $ rbenv install 3.0.1
   ```

5. (optional) run rbenv-doctor if you want to check or have some trouble


   ```
   $ curl -fsSL https://github.com/rbenv/rbenv-installer/raw/main/bin/rbenv-doctor | bash
   Checking for `rbenv' in PATH: /home/cyakarin/.rbenv/bin/rbenv
   Checking for rbenv shims in PATH: OK
   Checking `rbenv install' support: /home/cyakarin/.rbenv/plugins/ruby-build/bin/rbenv-install (ruby-build 20210526)
   Counting installed Ruby versions: 1 versions
   Checking RubyGems settings: OK
   Auditing installed plugins: OK

   ```
