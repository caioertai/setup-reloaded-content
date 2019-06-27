# Installing some gems

> We're going to install some gems. Gems are libraries written in ruby and published on a website that we can download and use using a tool called bundler, that you alread have ;) Once a gem exists in this website, we just have to run `gem install gem_name` in the terminal to download it.

⚠️ If you are in **China** 🇻🇳, you should update the way we'll install gem with the following commands. If you are not in China, well just skip this and go directly to the next `gem install` command!

```bash
# China only!
gem sources --remove https://rubygems.org/
gem sources -a https://gems.ruby-china.com/
gem sources -l
# *** CURRENT SOURCES ***
# https://gems.ruby-china.com/
# Ruby-china.com must be in the list now
```

---

All, please run the following line:

```bash
gem install rake bundler rspec rubocop rubocop-performance pry pry-byebug hub colored octokit
```

**Never** install a gem with `sudo gem install`! Even if you stumble upon a Stackoverflow answer
(or the Terminal) telling you to do so.
