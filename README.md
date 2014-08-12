jobsdone
========

Sometimes you need to run a long command on your machine. Wouldn't it 
be nice to know when its finished? For me its with my ``vagrant up``
and ``vagrant provision`` statements. Maybe a ``brew install`` that
takes a long time to compile.

I saw on twitter to use the Mac's ``say`` command. So I started to 
``say jobs done``, which made me nostalgic for the days I used to
play WarCraft 2 and would hear my peons declare "Job's Done!"

So introducing the jobsdone command!

## Usage

It's pretty simple, you just have to add ``&& jobsdone`` to the end 
of your command:

```bash
vagrant up && jobsdone
```

You can also hear something else if the command fails:

```bash
vagrant up && jobsdone || uhoh
```

## Install

Clone this repository:

```bash
# Go where you like to clone your git stuff
cd /where/your/git/stuff/goes

# Clone!
git clone https://github.com/JustinCarmony/jobsdone.git

# Create Symlink
ln -s /full/path/to/jobsdone/jobsdone /usr/local/bin/jobsdone
ln -s /full/path/to/jobsdone/uhoh /usr/local/bin/uhoh
```

Enjoy!