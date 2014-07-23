# Codespeak Kit

[Speaking in Code][codespeak] was an [NEH][neh]-funded symposium and
summit. On November 4–5, 2013, thirty-two software developers and
practitioners active in the digital humanities met at the [Scholars'
Lab][slab] in the [University of Virginia][uva] [Library][uva-lib]. They
gathered with the intent of exploring and making explicit the kinds of
tacit knowledge that inform and underlie software development,
especially in the context of DH projects. The purpose was to reflect on
the context of our work, discuss the transmission of tacit knowledge and
whether our practices and communication patterns contribute to an
ongoing disconnect between developers and humanities scholars, and to
interrogate DH code itself, *as practitioners*. We were particularly
interested in welcoming and listening to developers who could speak from
perspectives that have traditionally been marginalized in software
development.

In the end, in part due to our success in bringing together an unusually
diverse group of developers and participants' shared sense of the
specialness of that opportunity, the focus of the meeting diverged from
code critique and conversation about tacit knowledge transmission in the
act of software development. Participants instead spent the most of the
two days identifying and discussing ways to dismantle social barriers,
both explicit and implicit, spoken and tacit — barriers to access to
digital humanities communities and conversations, and internal barriers
dividing the DH community. These might range from  knowledge acquisition
required to perform technical work, to the way the field's structures of
review and reward primarily address the needs of traditionally-employed
scholars rather than all members of digital humanities teams.
Participants also examined the working conditions, social and power
structures, and (lack of) diversity found in technical environments in
general and in DH work in particular.

## Additional Materials

* [Planning](planning.md)
* [Logistics](logistics.md)
* [Schedule](schedule.md)
* [Bibliography](bibliography.md)

## Instructions

The Codespeak Kit is a [Jekyll][jekyll] application that can run in
[Github Pages][pages]. There are a couple ways to get a copy of this
up-and-running, so pick the one that fits your needs.

### Fork It

1. Create a [fork][fork] of this repository.
2. [Clone][clone] your fork of the repository.
3. Install [Jekyll][jekyll] and its dependencies.
3. Check out the `gh-pages` branch of the repository.
4. Make modifications to the site as needed. The main file is
   `index.html`.
5. Push the `gh-pages` branch to your Github remote.

```shell
$ mkdir -p ~/projects
$ cd ~/projects
$ git clone git@github.com:scholarslab/codespeakkit.git
$ cd codespeakkit
$ git checkout gh-pages
$ bundle install
```

### Yeoman Scaffold
If you have [node][node] installed, you can use the [yeoman][yeoman] as
well. Simply install the `codespeak` generator from `npm` and then run
the generator.

```shell
$ npm install -g yo generator-codespeak
$ yo codespeak
```

Once installed, you can preview changes to the content with the built in
web server that ships with `jekyll`.

```shell
$ jekyll serve --watch
```


The scaffolding will take care of installing dependencies and setting up
a development environment. When you're ready to deploy to github, simply
create a new repository and push to the `gh-pages` branch.

### Publishing

Once you have updated the site the way you want it, you can push this to
the special [gh-pages][pages] branch (assuming you have a Github remote
configured).

If you have a custom domain for your #codespeak, create a file in your
project directory named `CNAME` that contains the domain name you
registered and push it to your `gh-pages` branch.

```shell
$ echo "custom.domain.org" >> CNAME
$ git add CNAME
$ git commit -m "Add custom domain"
$ git push origin gh-pages
```

In your DNS settings, create a CNAME entry that points to the github
pages. For more detailed instructions, see [Tips for configuring a CNAME
record with your DNS provider][gh-pages-dns].

## What happens next?

Discussions at [Speaking in Code][codespeak] were challenging,
thought-provoking, open, heartfelt, and compelling — and we want to
share. We put together this kit to amplify voices, to continue
conversations, and to enable more DH and digital library software
developers and members of our larger digital humanities community to
join in.

This kit is your key to hosting conversations of your own.

But there are no step-by-step instructions. In fact, your Speaking in
Code will — and should! — look different from the one held in November
2013. This is a loose set of suggestions, priorities, and practices to
encourage the type of discussion that the Scholars' Lab attendees
found transformative. Nevertheless it will be *your* Speaking in Code.
It will grow out of your context and address the concerns of your
participants.

The main concrete tool in this kit is a website template. It includes
basic styling, slots for necessary information, an application for
interested practitioners, and the *You are Welcome Here* statement. You
can fork this git repository, use the styles and overall design we
created, and customize the template as you wish to jumpstart your own
Speaking in Code summit.

However, you don't have to wait to join in the conversation. We are
committed to continuing the discussion online:

* [#codespeak][twitter] (Twitter)
* [#speakingincode][irc] (IRC)

Use the hashtag on Twitter or join the Speaking in Code IRC channel to
bring new voices into the mix — and to call on the experience and
goodwill of participants and organizers from the inaugural event.

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
[irc]: http://webchat.freenode.net/?channels=%23speakingincode&uio=d4
[fork]: https://help.github.com/articles/fork-a-repo#step-1-fork-the-spoon-knife-repository
[clone]: https://help.github.com/articles/fork-a-repo#step-2-clone-your-fork
[jekyll]: http://jekyllrb.com/
[node]: http://nodejs.org/
[yeoman]: http://yeoman.io/
[pages]: https://pages.github.com/
[gh-pages]: https://help.github.com/articles/creating-project-pages-manually
[gh-pages-dns]: https://help.github.com/articles/tips-for-configuring-a-cname-record-with-your-dns-provider
