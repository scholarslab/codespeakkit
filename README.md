# Codespeak Kit

This is work-in-progress by the [Scholars' Lab][slab] at [UVa Library][uva-lib], toward a "starter kit" for holding events and continuing conversations under the banner of [Speaking in Code][codespeak]. The original event was an [NEH][neh]-funded summit for digital humanities software developers held at the [University of Virginia][uva] in November of 2013.

## Instructions

1. Create a [fork][fork] of this repository.
2. [Clone][clone] your fork of the repository.
3. Install [Jekyll][jekyll] and its dependencies.
3. Check out the `gh-pages` branch of the repository.
4. Make modifications to the site as needed. The main file is
   `index.html`.
5. If you have a custom domain, add a new file named `CNAME` with the
   domain.
5. Push the `gh-pages` branch to your Github remote.

```shell
$ mkdir -p ~/projects
$ cd ~/projects
$ git clone git@github.com:scholarslab/codespeakkit.git
$ cd codespeakkit
$ git checkout gh-pages
$ bundle install
$ cat "custom.domain.org" >> CNAME
$ git add CNAME
$ git commit -m "Add custome domain"
$ git push origin gh-pages
```

If you have [node][node] installed, you can use the [yeoman][yeoman] as
well. Simply install the `codespeak` generator from `npm` and then run
the generator.

```shell
$ npm install yo generator-codespeak
$ yo codespeak
$ grunt
```

The scaffolding will take care of installing dependencies and setting up
a development environment. When you're ready to deploy to github, simply
create a new repository and push to the `gh-pages` branch.

## Additional Materials
* [Planning](planning.md)
* [Logistics](logistics.md)
* [Schedule](schedule.md)
* [Bibliography](bibliography.md)

[codespeak]: http://codespeak.scholarslab.org/
[neh]: http://www.neh.gov/divisions/odh
[slab]: http://www.scholarslab.org/
[uva]: http://www.virginia.edu/
[uva-lib]: http://www.library.virginia.edu/
[twitter]: https://twitter.com/search?q=%23codespeak
[irc]: http://webchat.freenode.net/?channels=%23codespeak&uio=d4
[fork]: https://help.github.com/articles/fork-a-repo#step-1-fork-the-spoon-knife-repository
[clone]: https://help.github.com/articles/fork-a-repo#step-2-clone-your-fork
[jekyll]: http://jekyllrb.com/
[node]: http://nodejs.org/
[yeoman]: http://yeoman.io/
[gh-pages]: https://help.github.com/articles/creating-project-pages-manually
