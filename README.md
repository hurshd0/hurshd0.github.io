## 🚀 Explorers path finding site 👨‍🚀 🚀

### Theme based on Start bootstrap Jekyll https://github.com/volny/creative-theme-jekyll

### How to install on Ubuntu or WSL if you are on windows?

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

### How to add portfolio projects ?

Edit below snippet to customize your project thumbnail, and add it to `portfolio.html`

```html
       <a href="#portfolioModal1" class="portfolio-link" data-toggle="modal">
          <div class="portfolio-hover">
            <div class="portfolio-hover-content">
              <i class="fa fa-flask fa-3x"></i>
            </div>
          </div>
          <img src="img/portfolio/thumbnails/<YOUR_THUMBNAIL>.png" class="img-responsive" alt="<PROJECT INFO>" />
        </a>
        <div class="portfolio-caption">
          <h4>PROJECT NAME</h4>
          <p class="text-muted">
            PROJECT INFO
          </p>
        </div>
      </div>
```

Than add Portfolio Modal snippet to `modals.html`

```html
<div class="portfolio-modal modal fade" id="portfolioModal1" tabindex="-1" role="dialog" aria-hidden="true"
  style="display: none;">
  <div class="modal-dialog">
    <div class="modal-content">
      <div class="close-modal" data-dismiss="modal">
        <div class="lr">
          <div class="rl"></div>
        </div>
      </div>
      <div class="container">
        <div class="row">
          <div class="col">
            <div class="modal-body">
              <!-- Project Details Go Here -->
              <h2>PROJECT NAME</h2>
              <p class="item-intro text-muted">
                ONE LINE PROJECT INFO
              </p>
              <!-- ADD YOUTUBE VIDEO -->
              <div class="youtube-player center-block" data-id=""
                style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);"></div>
              <!-- OR IMG/GIF LINK -->
              <img class="img-responsive center-block" src="img/portfolio/"
                alt="SHOWCASE OF MY APP"
                style="box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);" />
              <hr />
              <p>
                MY APP INFO
              </p>
              <p>
                👇 Check out my app and code below. 👇
              </p>
              <p>
                <button class="btn btn-secondary btn-responsive"
                  onclick=" window.open('https://github.com/<INSERT PROJECT REPO LINK>','_blank')">
                  <i class="fa fa-github"></i> View Github
                </button>
                <button type="button" class="btn btn-primary btn-responsive" data-dismiss="modal">
                  <i class="fa fa-times"></i> Close Project
                </button>
                <button class="btn btn-info btn-responsive" onclick=" window.open('https://myapp.app','_blank')">
                  <i class="fa fa-cog"></i> View App
                </button>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</div>
```

### How to customize styling?

Under `css` folder  look for `styles.css` add your custom classes there, this theme uses bootstrap styling. 






