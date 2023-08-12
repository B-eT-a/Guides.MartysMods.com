Local Build using Windows.
Windows 11 22H2 22621.2070

# Notes
* Jekyll - https://jekyllrb.com
* Just The Docs - https://github.com/just-the-docs/just-the-docs
* Just The Docs Documentation - https://just-the-docs.com
* Markdown Extension - Kramdown https://kramdown.gettalong.org/quickref.html#extensions

# Installing Jekyll and Builder via RubyInstaller - Windows
1. Install Dependancies - `https://rubyinstaller.org/downloads/` Using 3.2.2-1 x64 + Devkit.
    * Run `ridk install`from CMD. **Requires Admin**.
    * Choose `MSYS2 and MINGW development tool chain`.
    * If you mess up, run `ridk install` from the CMD again and select the proper choice.
2. Open CMD/Terminal so that `PATH` Envs changes become effective.
    * Check path in CMD with `path`.
    * Default path is `PATH=C:\Ruby32-x64\bin;`.
3. Instal Jekyl and builder `gem install jekyll bundler`.
    * Will take a bit... Took ~7 minutes on my machine.
4. Check Jekyll install via `jekyll -v`.
    * If error occurs, restart your machine and try again.

# Building Locally
1. Clone GitHub Repository.
2. CD To Location Repo exists within.
3. CMD Run `bundle install` - Only needs to be done once.
4. CMD Run `bundle exec jekyll serve` You can add the argument `--livereload` so that changes happen on the fly.
5. Site will be hosted on `http://127.0.0.1:4000/` for local viewing.

# Editing Markdown
* Just The Docs uses a mixture of Kramdown and Markdown in order to allow users to better create documentation/guides.

    Above I have listed the Kramdown site, which holds a ton of information on Kramdown's syntax

    However, there is also more provided on the Just The Docs documentation website as well.
    
1. Simply fork the :dev: branch of the GitHub repository using the GitHub website, and then downlolad GitHub Desktop (as it makes things easier in the long run)
2. In GitHub Desktop, Clone your forked repository, and make changes to the location that is local to your machine.
3. View the changes by building the site using the building locally guide above.
4. Once changes are made and you are happy with them, push your commits to your :dev: branch, and merge them with the :dev: branch of the official repository when you are done!