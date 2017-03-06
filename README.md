#Stormpath is Joining Okta
We are incredibly excited to announce that [Stormpath is joining forces with Okta](https://stormpath.com/blog/stormpaths-new-path?utm_source=github&utm_medium=readme&utm-campaign=okta-announcement). Please visit [the Migration FAQs](https://stormpath.com/oktaplusstormpath?utm_source=github&utm_medium=readme&utm-campaign=okta-announcement) for a detailed look at what this means for Stormpath users.

We're available to answer all questions at [support@stormpath.com](mailto:support@stormpath.com).

# stormpath-mailchimp

*Enrich your Mailchimp lists with Stormpath, instantly!*


![Monkey Sketch][]


## Purpose

If you use [Stormpath][] to store and manage your user accounts,
`stormpath-mailchimp` can be used to easily populate your [Mailchimp][] email
lists magically.

Currently, `stormpath-mailchimp` will go through your chosen Stormpath, and
subscribe all new users to your [Mailchimp][] mailing list of choice.  We'll
automatically handle adding your user's:

- Email
- Given Name (*first name*)
- Surname (*last name*)

This is useful because in many cases, you want all new users you get to be
automatically subscribed to your company mailing list.  `stormpath-mailchimp`
makes this integration as painless as possible.


# Install

You can install `stormpath-mailchimp` through [npm][] by
running:

```console
$ npm install -g stormpath-mailchimp
```

**NOTE**: Depending on how you have `npm` installed, you might need to run the
above command with `sudo`.


## Setup

Once you have `stormpath-mailchimp` installed, you can configure it by running:

```console
$ stormpath-mailchimp --configure
```

This will prompt you for your [Stormpath][] and [Mailchimp][] API keys (which
are both required).

Don't have a Stormpath or Mailchimp account yet?

- Create your [Stormpath][] account [here][].
- Create your [Mailchimp][] account [over here][].

**Both of these services are free to use!**


## Usage

Using `stormpath-mailchimp` is easy!  All you do is tell the program what
Stormpath Directory to grab users from, and what Mailchimp list to sync your
users with.

Here's how to do it:

```console
$ stormpath-mailchimp --directory test --list test
```

The above command will sync all of your users from the Stormpath Directory
`test` into your Mailchimp List, also named `test`.

This might take a while, depending on how many user accounts you have.

If you'd like to see the available help options, you can run:

```console
$ stormpath-mailchimp --help
```

**NOTE**: For best results, consider running `stormpath-mailchimp` on a cron job --
this way, any user accounts you have will be automatically updated with the
latest information possible, and you'll continuously have an up-to-date
directory of users!


  [Monkey Sketch]: https://github.com/rdegges/stormpath-mailchimp/raw/master/assets/monkey-sketch.jpg "Monkey Sketch"
  [Stormpath]: https://stormpath.com/ "Stormpath"
  [Mailchimp]: http://eepurl.com/bgsmgr "Mailchimp"
  [here]: https://api.stormpath.com/register "Create a Stormpath Account"
  [over here]: http://eepurl.com/bgsmgr "Create a Mailchimp Account"
  [npm]: https://www.npmjs.org/ "npm"
