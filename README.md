STEP Workflow
================================================================================

In summer of 2020, I interned at google, and this is my attempt at
autoformatting. My goal here is to comply with Google’s style guides.

There isn’t much organization to this repo. However, I have basic formatting for
java (via google-java-format), JavaScript (via clang-format), and HTML/CSS (via
js-beautify). If you use vim, I also have included my .vimrc and .vim directory
for you to explore.

Configuration
================================================================================

These instructions apply to Ubuntu-based machines.

To configure vim, copy the .vimrc file and the .vimrc directory to the root of
your home directory.

Copy the contents of the formatting-scripts directory to `/usr/local/bin`.

For java formatting to work, you must download google-java-format at
(https://github.com/google/google-java-format). Make sure to get the jar that
has all the dependencies included. Copy the jar file to `/usr/local/lib`.

For JavaScript, you need clang-format. Try `sudo apt-get install clang-format`
to install it.

For HTML/CSS, you need js-beautify. You can get this from the npm repositories.
If you don’t have npm installed, do `sudo apt-get install npm`. After
installing, you can do something like `sudo npm install -g js-beautify`

Usage
================================================================================

For formatting html and any xml-style files, run `fixhtml -r <file_name>`

For java, run `google-java-format -i <file_name>`

For JavaScript, do `clang-format -style=google -i <file_name>`

Feedback
================================================================================

I am sharing this because it took me a while to get this setup right. Feel free
to pull request if you wish to add more changes to this.

