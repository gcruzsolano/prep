# Configure GitHub Keys

Ok, so this one is likely going to require some help from your
instructor or teacher assistant, which is totally ok. It is not
really important that you memorize this, but it does not hurt to
understand what is being setup so you can come back to it
later—especially if you would ever like to become a teacher assistant,
instructor, or productive professional developer.

## Secret Decoder Rings

GitHub keys are sort of like a master magic message decoder ring and
a bunch of rings you could give others to communicate with you
secretly. 

![](/assets/ring.jpg)

You can send messages to anyone and they can read it and
know it is from you. Everyone else can be sure the message came from
you and send you secret messages. No one could read each others’
messages. Communication is just between you and each individual club
member.

## Secure Shell Keys

GitHub uses Secure Shell primarily for keys. There is a ***private***
key and a ***public*** key. You can give the public key to whomever
you want to know that a message is coming from you. The private key
you keep very secret.

In order to not have to use passwords to login to GitHub for every
time we want to save our work we need to give GitHub one of our public
keys. It is a little involved because first we have to make the keys,
but not too hard—especially if you have help from your instructor and
teacher assistants. Even though we only have to do this once for your
entire time at SkilStak™ it is worth understanding what is happening
so you can refer to it later when trying to do it for your own
machines, work computers, or other schools.

## Create a Key Pair with `ssh-keygen`

Enter the `ssh-keygen` command to create a key pair. Just accept
all the defaults by typing enter. (Later you can add a passphrase
if you like when you understand what that means.) The public and
private keys will be created in your `.ssh` directory in your home
directory.

![](/assets/ssh-keygen.gif)

## Copy Your Public Key

You can list your keys with `ls .ssh`. Notice one is `id_rsa.pub`.
That is the public one. We need to copy the content of that key into
the GitHub SSH Keys settings page. To copy first `cat .ssh/id_rsa.pub`
to the screen (or use the `pubkey` alias which does the same thing).
Then select it with your mouse and copy it by right-clicking the
selected text or using `⌘-c` keyboard shortcut.

![](/assets/copy-pubkey.gif)

## Paste Public Key into GitHub Settings

Now we have to give GitHub our public key by adding it to the SSH
section of our *Settings*.

![](/assets/keys-in-github.gif)

## Test

To test attempt to connect to github.com using ssh with `ssh
git@github.com`. You will get a polite denial letting your know there
is no command line access but that you are all set for `git clone`ing
and such.

![](/assets/ghping.gif)

## Clone a Repo

The process of getting a copy of a repo is called *cloning* in `git`
and GitHub. The URL is rather long, but thankfully GitHub makes it
easy to copy so we can paste it into our `git clone` command. If you
add another name after the URL it will create a clone with that name
instead of the one on GitHub. In our case this changes
`pyfun-youraccount` to just `pyfun` (since `youraccount` is rather
redundant).

![](/assets/git-clone.gif)

## Update Push Default

After you have made your changes inside the repo and are ready to save
them for the day you run `save`. However, the first time you do this
`git` needs a bit of information about how to do this. Just cut and
paste the simple like as the default.

![](/assets/pushdefault.gif)

## Update Profile Configuration

Now when you save you will be reminded to set the `user.name` and
`user.email` settings. These are used to give you that coveted green
square credit for your commits.

First make sure you have the right information to put in by going to
your GitHub profile.

![](/assets/github-profile.png)
![](/assets/github-account-name.png)

Now you can enter that information on the command line.

![](/assets/user-name-email.gif)

From now on all your commits will include that information and be
credited correctly.

You are all set.

---
[![home](/assets/home-bw.png)](/README.md)
[![cc-by-sa](/assets/cc-by-sa.png)][cc-by-sa]
[![skilstak](/assets/skilstak-logo-bw.png)][skilstak]
[cc-by-sa]: https://creativecommons.org/licenses/by-sa/4.0/
[skilstak]: http://skilstak.io

