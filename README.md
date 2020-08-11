## 🚀 Explorers path finding site 👨‍🚀 🚀


### How to install on Ubuntu ?

Step 1. Get required dependencies for jekyll `sudo apt-get install ruby-full build-essential zlib1g-dev`
Step 2. Add paths for running Ruby Gems on user account 

NOTE: If you are using zsh than replace `.bashrc` to `.zshrc`
```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```
Step 3. Install Jekyll `gem install jekyll bundler`

### How to run the app ?
Simply run `bundle exec jekyll serve`






